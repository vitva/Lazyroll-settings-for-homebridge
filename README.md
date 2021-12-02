
# LazyRolls settings for Homebridge


#### Motorized roller blinds drive LazyRolls

Setting up a LazyRolls drive using Homebridge and MQTT.

#### Моторизированный привод для рулонных штор LazyRolls
Настройка привода LazyRolls
используя Homebridge и MQTT. 

### Example config.json:

```
{
   "accessory": "mqttthing",
   "type": "windowCovering",
   "name": "<name of device>",
   "topics": 
   {
       "getOnline": "lazyroll/%HOSTNAME%/alive",
       "getCurrentPosition": "lazyroll/%HOSTNAME%/state",
       "setTargetPosition": "lazyroll/%HOSTNAME%/command"
   },
   "onlineValue": "online",
   "offlineValue": "offline",
   "positionStateValues": ["decreasing-value", "increasing-value", "stopped-value"]
}
```

• The optional `minPosition` and `maxPosition` allow the minimum and maximum position values to be changed from their defaults of 0 and 100 respectively.

• Необязательно `minPosition` и `maxPosition` позволяют изменять минимальное и максимальное значения позиции по сравнению с их значениями по умолчанию 0 и 100 соответственно.

```
"minPosition":0,
"maxPosition":100
```

### Ссылка на проект LazyRolls:
https://github.com/ACE1046/LazyRolls
