## HomeAssistant Configuration

Having fun with HomeAssistant a home automation platform running on Python 3.  You can learn more about [Home Assistant](https://home-assistant.io/) at their website.

My instance of HomeAssistant is running the HASSbian image on a Raspberry Pi 2.  Below is a list of devices currently integrated with HomeAssistant.

 - [Cisco Meraki MX64](#meraki)
 - [Google Home](#google)
 - [Netgear Nighthawk](#netgear)
 - [Samsung Smartthings](#smartthings)


#### <a name="meraki"></a>Cisco Meraki MX64

The MX64 is a cloud managed security gateway and router.  The amazing thing about the Merki is it's onboard REST API.  This provides the unique ability to query devices, as well as log traffic patterns using HomeAssistant on a per devices basis.

#### <a name="google"></a>Google Home

The Google Home is used for TTS (Text to Speech) providing for audible notifications of events in the home.  In addition the Google Home is leveraged as a music streaming device, allowing for the easy sharing of streaming MP3 media via the HomeAssistant interface.

#### <a name="netgear"></a>Netgear Nighthawk

The Nighthawk is the home's primary wireless router.  It is used for both 2.4Ghz (N) and 5Ghz (AC) wireless access.  In addition to the NightHawk an Asus RT-66U is used for sharing wireless with smart devices which require access to cloud services so as to not share the same primary network as personal devices.

#### <a name="smartthings"></a>Samsung SmartThings

The Samsung SmartThings Home Automation HUB is used as a gateway to Zigbee and Z-Wave devices.  I never use the SmartThings application except for adding or removing devices.  Because SmartThings relies on the Samsung cloud this will most likely be phased out for a USB dongle approach using the PI as a hub.  Currently the SmartThings HUB is connected to HomeAssistant via the [MQTT Bridge](https://github.com/stjohnjohnson/smartthings-mqtt-bridge).


> This is by no means an exhaustive list of  devices, and integrations currently in use with HomeAssistant, but I wanted to get code checked in.  This will be updated in the future as time allows.
