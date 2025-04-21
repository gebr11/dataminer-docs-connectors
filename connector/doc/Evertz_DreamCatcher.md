---
uid: Connector_help_Evertz_DreamCatcher
---

# Evertz DreamCatcher

**Evertz DreamCatcher** is a scheduling system for generating “growing files” for the customer workflow to schedule events. To retrieve the data, the connector uses a Serial connection.

## About

### Version Info

|Range  |Features  |Based on  |System Impact  |
|---------|---------|---------|---------|
|1.0.0.x [SLC Main]     |<ul><li>Initial version.</li></ul>         |-         |-         |

### Product Info

|Range  |Supported Firmware  |
|---------|---------|
|1.0.0.x     |2.9.2.r1.588         |

### System Info


|Range  |DCF Integration  |Cassandra Compliant  |Linked Components  |Exported Components   |
|---------|---------|---------|---------|---------|
|1.0.0.x    |No       |Yes         |Yes       |   |

## Configuration

### Connections

#### Serial Connection

This connector uses a serial connection and requires the following input during element creation:

SERIAL CONNECTION:

- Direct connection:

  - **Port**: 5001

### Initialization

To start using the connector, the user needs to configure the username and the version (both parameters are on General page). 

After those values are set, the connector automatically tries the connection and the user can see if the connection was successful or not on the Status parameter (General page).

### Redundancy

There is no redundancy defined.

### Web Interface

The web interface is only accessible when the client machine has network access to the product.

## How to use

After the initialization process is completed, the user can see all tables filled in with the device information.

- To create a **task**, the user can find the Create Task pagebutton on Tasks page, which deploys a popup window with the required data to create a task.
- To create a **schedule**, the user can find the Create Schedule pagebutton on Schedules page, which deploys a popup window with the required data to create a schedule.
