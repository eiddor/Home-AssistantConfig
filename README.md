# Home-Assistant Config by [@eiddor](http://www.twitter.com/eiddor) (layout ideas stolen from [@ccostan](http://www.twitter.com/ccostan))
[Home Assistant](https://home-assistant.io/) configuration files (YAMLs)

Welcome to my Home Assistant Configuration.  It's more or less complete for now, but I tend to tinker with things as I learn more about it.

Home Assistant runs on my [Raspberry Pi 3](http://amzn.to/2e3DOBY) with [Aeon Labs Z Wave Stick (GEN 5)](http://amzn.to/2eAiAP0). 

Software on the Pi : [Home Assistant](https://home-assistant.io/) , [OpenZwave Control Panel](https://github.com/OpenZWave/open-zwave-control-panel)

**List of devices :**

* [Amazon Echo](http://amzn.to/2dSVbK4)
* [Amazon Dash Buttons](http://amzn.to/2dPKZhM)
* [Philips Hue Starter Kit Gen 3](http://amzn.com/B01KJYSO68)
* [GE Z-Wave On/Off Switch](http://amzn.com/B0035YRCR2)
* [GE Z-Wave Smart Dimmer Switch](http://amzn.com/B006LQFHN2)
* [GE Z-Wave Outdoor Module](http://amzn.com/B0013V8K3O)
* [GE Z-Wave Fan Control Switch](http://amzn.com/B00PYMGVVQ)
* [GE Z-Wave Receptacle](http://amzn.com/B0013V1SRY) [not yet installed]
* [Aeotec DSB45 Water Sensor](http://amzn.com/B00H3TJ3P4)
* [Aeotec ZW096 Smart Switch](http://amzn.com/B00VQISOCG)
* [Aeotec ZW100 Multisensor](http://amzn.com/B0151Z8ZQY)
* [Rokus](http://amzn.to/2dpn89c) [not currently added my Home Assistant]
* [Plex Media Server](https://www.plex.tv/)
* [Logitech Harmony Smart Control](http://amzn.com/B00BQ5RYI4)
* [Garadget](http://garadget.com)


**Automations:**

* Turn on Porch Lights at Sunset, off at Sunrise 
* Turn on Christmas Lights at Sunset, off at Midnight
* Check for Home Assistant Releases and notify via [Pushbullet](https://www.pushbullet.com/)
* Turn On/Off Bedroom lamp when Dash Button event is called via API [script running on different host]
* Turn theater lights on in Media Room on motion detection if no one is watching something via the Logitech Harmony Hub
* Local backup of all configuration files at 1 AM

![Screenshot Home View](http://i.imgur.com/nYWUbht.png)
![Screenshot of Information View](http://i.imgur.com/Qa9Y5m6.png)
![Screenshot of Entertainment View](http://i.imgur.com/plN6vGW.png)


**Time Based Automation TimeLine** (a WIP)
```
SUNRISE:
     Turn off Porch Lights

SUNSET: 
     Turn on Christmas Lights
     Turn on Porch Lights

11:59 PM Turn off Christmas Lights
01:01 AM Backup HASS Configuration Files
02:31 AM Heal ZWave Network
```

#Todo List

* Install GE Z-Wave Outlets
* ~~Enhance the Media Room motion sensor to turn off lights after a period and check for Lux condition [changed this to detect when there is activity via the Harmony Hub]~~
* ~~Add Harmony Hub when it arrives~~
* Configure a clever automation for when the Water Sensor is triggered (it's in a closet with my water heaters)
* Add more sophisticated control of my Hue lights
* Buy some Hue LED strips
* Install the third Hue bulb 
* Setup my two remaining Amazon IoT buttons to do something
* Purchase some kind of doorbell/camera
* Purchase some Z-Wave compatible thermostats
* ~~Purchase a Z-wave compatible garage door opener/sensor [Garadget](http://garadget.com)~~
* Add a couple more Aeotec Multisensors around the house and mess with the family
* https://github.com/thundergreen/home-assistant/wiki/Add-OZWCP-in-HASS
* Taking suggestions!!!
