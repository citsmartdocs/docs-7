Title: Collecting hardware data from MIB (SNMP)

# Collecting hardware data from MIB (SNMP)

It's possible to collect hardware asset data using the SNMP protocol - via MIB collection - and add to the information of a configuration item in the Configuration Management process.

## What to do beforeO que fazer antes

- [X] It's necessary to have deployed the CITSmart Inventory Version 1.2.1.9 or higher (see [Perform installation][1]);
- [X] In the standalone-full.xml file, add the property `snmp.oid.repository.directory` with the path of the folder where it'll be the files xml with the layout (see [System Properties Configuration][2]);
- [X] Have an inventory process defined via Configuration Management (see [Implement CITSmart Inventory][3]);
- [X] Inventory the SNMP configuration item for collecting MIB (see [Configuring inventory connection][4]);


## Creating Model

Model:

```xml
<ITS-TYPE-ITEM oid-validator="(OID of a specific property that will allow the rest of the file to be interpreted. If no value is returned, the TYPE-ITEM is not created.)">
                <ITS-CHARACTERISTIC>(OID of the information you want)</ITS-CHARACTERISTIC>
                <CHARACTERISTIC-IN-HEXA type="hex">(OID of the information that the returned value needs to be converted from HEXADECIMAL)</CHARACTERISTIC-IN-HEXA>
</ITS-TYPE-ITEM>
```

Example:

```xml
<PRINTER oid-validator=".1.3.6.1.2.1.43.5.1.1.16.1">
                <NAME>.1.3.6.1.2.1.43.5.1.1.16.1</NAME>
                <DESCRIPTION type="hex">.1.3.6.1.2.1.43.5.1.1.16.1</DESCRIPTION>
                <NUMBER-PAGES-PRINTED>.1.3.6.1.2.1.43.10.2.1.4.1.1</NUMBER-PAGES-PRINTED>
                <CAPACITY-TOTAL-TONER>.1.3.6.1.2.1.43.11.1.1.8.1.1</CAPACITY-TOTAL-TONER>
                <CAPACITY-CURRENT-TONER>.1.3.6.1.2.1.43.11.1.1.9.1.1</CAPACITY-CURRENT-TONER>
</PRINTER>
```

## Deploying Model

After creating the model, it's necessary to save it in the folder indicated in the parameter  `snmp.oid.repository.directory` of the application server. After the model deployment, at the time of inventory execution, the application will check the CI that have the indicated MIB and will automatically update the assets with the collected information.


!!! danger "DANGER"

    1. Layout files can have any name. All files in the folder will be interpreted, so there can only be XML files inside it;
    2. If there is more than one layout, it can be placed within the same file or in different files. It's only necessary to respect the XML format;

!!! example "USEFUL LINKS"

    1. http://www.oidview.com/mibs/ - Repository containing thousands of MIB separated by the manufacturers.
    2. http://ireasoning.com/mibbrowser.shtml - MibBrowser tool that can assist in OID collection.

[1]:/en-us/citsmart-7/get-started/installation-and-upgrade/perform-installation.html
[2]:/en-us/citsmart-7/get-started/installation-and-upgrade/perform-installation.html#configuracao-do-system-properties
[3]:/en-us/citsmart-7/additional-features/add-ons/inventory.html
[4]:/en-us/citsmart-7/processes/event/configuration/set-inventory-connection.html
