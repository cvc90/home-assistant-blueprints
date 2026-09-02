# Home Assistant Blueprints

Automation blueprints for SONOFF devices in Home Assistant.

## Import a blueprint

### Option 1: Open the import dialog in Home Assistant

Select an **Import** button below. It opens the Blueprint import dialog in your Home Assistant instance; review the blueprint and select **Import Blueprint**.

### Option 2: Import manually

1. Open the GitHub link for the blueprint you want below.
2. In Home Assistant, go to **Settings > Automations & scenes > Blueprints**.
3. Select **Import Blueprint**, paste the GitHub link, select **Preview**, then select **Import Blueprint**.

## SONOFF blueprints

All SONOFF blueprints are under [`automation/sonoff`](automation/sonoff).

### Sync Remote Sensor to SNZB-02DR2

Synchronizes an external temperature reading and an optional humidity reading with a SONOFF SNZB-02DR2. Supports ZHA and Zigbee2MQTT.

[![Import Sync Remote Sensor to SNZB-02DR2](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fviys%2Fhome-assistant-blueprints%2Fblob%2Fmaster%2Fautomation%2Fsonoff%2Fremote_source_link_snzb02dr2.yaml)

[GitHub blueprint link](https://github.com/viys/home-assistant-blueprints/blob/master/automation/sonoff/remote_source_link_snzb02dr2.yaml)

[Download YAML](https://raw.githubusercontent.com/viys/home-assistant-blueprints/master/automation/sonoff/remote_source_link_snzb02dr2.yaml)

### Sync Remote Temperature to TP-WGZBA

Synchronizes an external temperature reading with a SONOFF TP-WGZBA thermostat. Supports ZHA and Zigbee2MQTT.

[![Import Sync Remote Temperature to TP-WGZBA](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fviys%2Fhome-assistant-blueprints%2Fblob%2Fmaster%2Fautomation%2Fsonoff%2Fremote_temperature_link_tp_wgzba.yaml)

[GitHub blueprint link](https://github.com/viys/home-assistant-blueprints/blob/master/automation/sonoff/remote_temperature_link_tp_wgzba.yaml)

[Download YAML](https://raw.githubusercontent.com/viys/home-assistant-blueprints/master/automation/sonoff/remote_temperature_link_tp_wgzba.yaml)

### Sync Remote Temperature to TRV-ZBL

Synchronizes an external temperature reading with a SONOFF TRV-ZBL thermostatic radiator valve. Supports ZHA.

[![Import Sync Remote Temperature to TRV-ZBL](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fviys%2Fhome-assistant-blueprints%2Fblob%2Fmaster%2Fautomation%2Fsonoff%2Fremote_temperature_link_trv_zbl.yaml)

[GitHub blueprint link](https://github.com/viys/home-assistant-blueprints/blob/master/automation/sonoff/remote_temperature_link_trv_zbl.yaml)

[Download YAML](https://raw.githubusercontent.com/viys/home-assistant-blueprints/master/automation/sonoff/remote_temperature_link_trv_zbl.yaml)

### Sync Remote Temperature to TRVZB

Synchronizes an external temperature reading with a SONOFF TRVZB thermostatic radiator valve. Supports ZHA and Zigbee2MQTT.

[![Import Sync Remote Temperature to TRVZB](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fviys%2Fhome-assistant-blueprints%2Fblob%2Fmaster%2Fautomation%2Fsonoff%2Fremote_temperature_link_trvzb.yaml)

[GitHub blueprint link](https://github.com/viys/home-assistant-blueprints/blob/master/automation/sonoff/remote_temperature_link_trvzb.yaml)

[Download YAML](https://raw.githubusercontent.com/viys/home-assistant-blueprints/master/automation/sonoff/remote_temperature_link_trvzb.yaml)

### Link TP-WGZBA Target Temperature to TRVs

Synchronizes the target temperature of a SONOFF TP-WGZBA thermostat with one or more SONOFF TRV-ZBL or TRV-ZBT devices.

[![Import Link TP-WGZBA Target Temperature to TRVs](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fviys%2Fhome-assistant-blueprints%2Fblob%2Fmaster%2Fautomation%2Fsonoff%2Ftrv_target_temperature_link_tp_wgzba.yaml)

[GitHub blueprint link](https://github.com/viys/home-assistant-blueprints/blob/master/automation/sonoff/trv_target_temperature_link_tp_wgzba.yaml)

[Download YAML](https://raw.githubusercontent.com/viys/home-assistant-blueprints/master/automation/sonoff/trv_target_temperature_link_tp_wgzba.yaml)

## Notes

- Importing a blueprint installs its definition. Create and configure an automation from the imported blueprint before it can run.
- Requirements vary by blueprint. Read the input descriptions in Home Assistant before creating the automation.
