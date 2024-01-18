# mqtt-kura-utils
This repository have some basic utility scripts for testing MQTT messages between Kura and Kapua.

The connection to the broker is not with TLS, it may will be added in feature developments.

## Setup

To execute the scripts in an identical environment:

1) Install Miniconda from the [online documentation](https://docs.conda.io/projects/miniconda/en/latest/miniconda-install.html).

2) Create the mqtt environment from a `linux-64` only machine: 
    `$ conda create --name mqtt --file requirements.txt`

    Or from a generic machine with:
    `$ conda env create -f conda_mqtt_env.yml`

## MQTT credentials

The MQTT credentials must be stored locally in a _config.ini_ file: 

Create a `config.ini` file with the following properties:

```
[MQTTSection]
mqtt.url=broker-sbx.test.io
mqtt.clientid=clientid
mqtt.user=user
mqtt.password=password
mqtt.topic=account/clientid/test
```
