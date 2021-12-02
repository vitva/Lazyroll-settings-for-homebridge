# Lazyroll-settings-for-homebridge


Motorized roller blinds drive

Настройка Моторизированного привода LazyRoll для рулонных штор
используя Homebridge и MQTT. 

### Ссылка

Проект: https://github.com/ACE1046/LazyRolls

```javascript 

{
            "accessory": "mqttthing",
            "type": "windowCovering",
            "name": "Name",
            "topics": {
                "getOnline": "lazyroll/%HOSTNAME%/alive",
                "getCurrentPosition": "lazyroll/%HOSTNAME%/state",
                "setTargetPosition": "lazyroll/%HOSTNAME%/command"
            },
            "onlineValue": "online",
            "offlineValue": "offline",
            "positionStateValues": [
                "decreasing-value",
                "increasing-value",
                "stopped-value"
            ]
        }

