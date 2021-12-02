# Lazyroll-settings-for-homebridge


Motorized roller blinds drive

Настройка Моторизированного привода LazyRoll для рулонных штор
используя Homebridge и MQTT. 

### Settings:

```
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
```

#### Ссылка на проект

https://github.com/ACE1046/LazyRolls
