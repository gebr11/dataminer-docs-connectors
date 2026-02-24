---
uid: Connector_help_Raisecom_ISCOM_2900_Technical
---

# Raisecom ISCOM 2900

## About

The **Raisecom ISCOM 2900** connector is a specialized connector designed to integrate Raisecom devices into monitoring platforms using the SNMP protocol. It supports both the **ISCOM 29XX** and **RAX 7XX** series, providing access to system metrics, hardware health, and optical transceiver data.

The connector includes full **SNMP trap handling** for real‑time event notifications and organizes monitoring information into distributed pages based on data type. Users can view detailed insights such as the optical Tx/Rx power, Tx bias current, and temperature readings, alongside system resources like CPU, memory, and voltage.

Configuration requires setting the device IP for SNMP and trap connections, defining get/set community strings, and selecting the appropriate device type to ensure the correct monitoring pages are displayed.

## Configuration

### Connections

#### SNMP Connection - Main

This connector uses a Simple Network Management Protocol (SNMP) connection and requires the following input during element creation:

SNMP CONNECTION:

- **IP address/host**: The polling IP or URL of the destination.

SNMP Settings:

- **Port number**: The port of the connected device, by default 161. For Trap Connection, the default port value is 162.
- **Get community string**: The community string used when reading values from the device (default: *public*).
- **Set community string**: The community string used when setting values on the device (default: *private*).

### Initialization

To start retrieving data with the Raisecom SNMP Connector, a few simple steps are required:

1. **Configure Connections**: Set the device’s IP address for both SNMP and trap communication.
1. **Define Communities**: Enter the appropriate get and set community strings for the SNMP connection.
1. **Select Device Type**: Choose the correct option in the Device Type parameter — either ISCOM 29XX or RAX 27XX — to automatically display the corresponding monitoring pages.

Once configured, the connector organizes the data into intuitive pages, giving you clear visibility into metrics such as *Optical Tx/Rx Power*, *Tx Bias Current*, and *Temperature*.
