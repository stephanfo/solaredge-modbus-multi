## SolarEdge Modbus Multi Device

A Home Assistant integration for SolarEdge inverters using Modbus/TCP.

It supports single inverters, multiple inverters, meters, and batteries.

Many improvements over other integrations that didn't work well with a multi-device setup.

Simple single inverter setups are fully supported - multiple devices is a feature, not a requirement.

{% if installed %}
{% if version_installed.replace("v", "").replace(".","") | int < 220 %}
### Recommended Update Procedure to v2.2.0

1. Delete integration from Settings -> Devices & Services.
2. Update to v2.2.0 release (manually or through HACS).
3. Re-Add the integration under Settings -> Devices & Services.
{% endif %}
{% endif %}

## Features
* Inverter support for 1 to 32 SolarEdge inverters.
* Meter support for 1 to 3 meters per inverter.
* Battery support for 1 or 2 batteries per inverter.
* Automatically detects meters and batteries.
* Supports Three Phase Inverters with Synergy Technology.
* Polling frequency configuration option (1 to 86400 seconds).
* Configurable starting inverter device ID.
* Connects using Modbus/TCP - no cloud dependencies.
* Informational sensor for device and its attributes
* Supports status and error reporting sensors.
* User friendly configuration through Config Flow.

Requires Home Assistant 2022.8.0 and newer.

Read about more features on the wiki: [WillCodeForCats/solaredge-modbus-multi/wiki](https://github.com/WillCodeForCats/solaredge-modbus-multi/wiki)
