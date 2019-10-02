Title: Recopilar datos de hardware desde los MIB (SNMP)

# Recopilar datos de hardware desde los MIB (SNMP)

Se puede recopilar datos de activos de hardware utilizando el protocolo SNMP - a través de recopilación MIB - y agregar a la información de un elemento de configuración en el proceso de Gestión de Configuración.

## Lo qué hacer antes

- [X] Es necesario implementar la versión CITSmart Inventory 1.2.1.9 o posterior (ver [Hacer la instalación][1]);
- [X] En el archivo standalone-full.xml se debe agregar la propriedad `snmp.oid.repository.directory` que contiene la ruta de la carpeta donde estarán los archivos xml con el diseño (Ver [Configuración del System Properties][2]);
- [X] Tener un proceso de inventario definido a través de la Gestión de Configuración (ver [Implementar CITSmart Inventory][3]);
- [X] Inventariar el elemento de configuración, vía SNMP para la colección del MIB (ver [Configurar conexión inventory][4]);


## Crear Modelo

Modelo:

```xml
<SU-TIPO-ELEMENTO oid-validator="(OID de una propiedad específica que permitirá interpretar el resto del archivo. Si no se devuelve ningún valor, no se crea el TIPO-ELEMENTO.)">
                <SU-CARACTERISTICA>(OID de la información deseada)</SU-CARACTERISTICA>
                <CARACTERISTICA-EN-HEXA type="hex">(OID de la información de que el valor devuelto debe convertirse de HEXADECIMAL)</CARACTERISTICA-EN-HEXA>
</SU-TIPO-ELEMENTO>
```

Ejemplo:

```xml
<IMPRESORA oid-validator=".1.3.6.1.2.1.43.5.1.1.16.1">
                <NOMBRE>.1.3.6.1.2.1.43.5.1.1.16.1</NOMBRE>
                <DESCRIPCION type="hex">.1.3.6.1.2.1.43.5.1.1.16.1</DESCRIPCION>
                <CANTIDAD-PAGINAS-IMPRESAS>.1.3.6.1.2.1.43.10.2.1.4.1.1</CANTIDAD-PAGINAS-IMPRESAS>
                <CAPACIDAD-TOTAL-TONER>.1.3.6.1.2.1.43.11.1.1.8.1.1</CAPACIDAD-TOTAL-TONER>
                <CAPACIDAD-ACTUAL-TONER>.1.3.6.1.2.1.43.11.1.1.9.1.1</CAPACIDAD-ACTUAL-TONER>
</IMPRESORA>
```

## Implementar Modelo

Después de crear el modelo, se debe guardarlo en la carpeta indicada en el parámetro   `snmp.oid.repository.directory` del servidor de la aplicación. Después de la implementación del modelo, en el momento de la ejecución del inventario, la aplicación verificará los EC que tienen las MIB indicadas y actualizará automáticamente los activos con la información recopilada.


!!! danger "CUIDADO"

    1. Los archivos de diseño pueden tener cualquier nombre. Se interpretarán todos los archivos de la carpeta, por lo que solo puede haber archivos XML dentro de ella;
    2. Si hay más de un diseño, se puede colocar dentro del mismo archivo o en archivos diferentes. Solo respeta el formato XML;

!!! exemple "ENLACES ÚTTILES"

    1. http://www.oidview.com/mibs/ - Repositorio que contiene miles de MIB separados por fabricantes.
    2. http://ireasoning.com/mibbrowser.shtml - Herramienta MibBrowser que puede ayudar a recopilar las OID.

[1]:/es-es/citsmart-7/get-started/installation-and-upgrade/perform-installation.html
[2]:/es-es/citsmart-7/get-started/installation-and-upgrade/perform-installation.html#configuracao-do-system-properties
[3]:/es-es/citsmart-7/additional-features/add-ons/inventory.html
[4]:/es-es/citsmart-7/processes/event/configuration/set-inventory-connection.html
