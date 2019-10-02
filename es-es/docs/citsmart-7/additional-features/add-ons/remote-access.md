Title: Implementar Acceso Remoto

# Implementar Acceso Remoto

La funcionalidad de acceso remoto permite que los equipos se tengan acceso de forma remota desde su instancia de CITSmart. En este sentido, utilizamos los recursos del protocolo VNC (Virtual Network Computing) a través del Apache Guacamole - Gateway de acceso remoto basado en la web - para hacer esta operación viable. Además de poder acceder remotamente a un elemento de configuración, todas las sesiones se guardan y se ponen a disposición de la información del EC. Esto garantiza un mejor control sobre las acciones realizadas, proporcionando un ambiente confiable y auditable.

Esta funcionalidad es un complemento (add-on) a la Gestión de Configuración y depende del proceso de inventarios para hacer el acceso remoto viable a un EC.


## Antes de empezar

Los siguientes requisitos antecede el uso efectivo de esta funcionalidad:

* [x] Tener un proceso de inventario definido y funcional utilizando el CITSmart Inventory;
* [x] Tener los elementos de configuración inventariados;

## Procedimiento

1. Instalar el GuaCD utilizando la [documentación oficial][1] o descargar el contenedor disponible por CITSmart. No es necesario 
instalar el guacamole-client, ya que el CITSmart utiliza sólo la daemon del Guacamole, o sea, el GuaCD;

2. Después de la instalación, configurar el punto de logs; 

    ```sh
    /usr/local/sbin/guacd -b 0.0.0.0 > /var/log/guacd.log 2>&1
    ```

3. Descargar el binario (.jar) del encoder de vídeo (en el centro de descargas del portal de socios) - que tiene la función de compilar los vídeos provenientes de las sesiones;

4. Copiar el encoder de vídeo al servidor;

5. Realizar la configuración reemplazando las variables por la información de su servidor;

    ```java
    java -Durl=${CITSMART_PROTOCOL}://${CITSMART_URL}/citsmart -DcontainerIdentifier=${CITSMARTGUACD_ID} -DuserName=citsmart.local\\${CITSMART_LOGIN} -Dpassword=${CITSMART_PASSWORD} -jar /citsmart-guacd-encoder.jar &
    ```

6. Definir el directorio para la grabación de los vídeos (por ejemplo: /mp4);

    !!! Abstract "Grabación de vídeos"
   
        Después del cierre de la sesión de acceso remoto, el vídeo generado entra en una cola de compilación para entonces, estar               disponible en la plataforma. El tiempo de compilación dependerá del tiempo de la sesión, además, el inicio de la compilación se         vincula a la rutina cron definida en la conexión de acceso remoto.

7. En el elemento de configuración que se tiene acceso de forma remota (por ejemplo: Ordenador Windows), instale un cliente de acceso 
remoto compatible con el protocolo VNC (por ejemplo: [TightVNC][3]) y establezca una contraseña de acceso. Guardar esta contraseña ya 
que se utilizará en el siguiente paso;

8. Realizar el registro de conexiones de acceso remoto en su instancia [según el documento][4].
    
## Lo que hacer después

Con el servicio del GuaCD activo y comunicable, el siguiente paso es acceder remotamente al EC configurado

## Relacionado

[Gestión de Configuración][5]

[Implementar el CITSmart Inventory][6]

[1]:https://guacamole.apache.org/doc/gug/installing-guacamole.html
[2]:images/citsmart-guacd-encoder.jar.zip
[3]:https://www.tightvnc.com/
[4]:/es-es/citsmart-7/processes/configuration/configuration/configure-remote-access.html
[5]:/es-es/citsmart-7/processes/configuration/overview.html
[6]:https://docs-7.citsmart.com/es-es/citsmart-7/additional-features/add-ons/inventory.html
