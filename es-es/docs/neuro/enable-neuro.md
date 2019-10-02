Title: Enable Neuro

# Enable Neuro

For CITSmart/Neuro integration to work:

- The CITSmart version is 7.0.0.0 or higher
- CITSmart configured for HTTPS access: //
- The integration parameters are configured in the CITSmart

![Neuro Conection][1]

- **Parameter 309:**

    ```sh
    Value: Yes
    ```

- **Parameter 310:**

    ```sh
    https://localhost:8443/cit-esi-web
    ```

- **Parameter 311:**

    ```sh
    citsmart.local\neuro.user
    ```

[1]:images/neuro-conection.png
