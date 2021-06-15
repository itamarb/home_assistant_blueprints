# Device state based on consumption

Blueprint to set the state of a device which needs to be turned off or on by IR/RF and not by powering down the socket i.e: AC or TV.

**Prequisists: **
1. Power metering device

  a. If you are using Tuya devices, in order to get the power consumption in HA, use the localtuya integration - https://github.com/rospogrigio/localtuya  (great tutorial - https://www.youtube.com/watch?v=vq2L9c5hDfQ&list=WL&index=3)

  b. If using Shelly 1pm, the consumption is a different entity, please see this blueprint.

2. IR/RF universal remote (i.e: Broadlink) - https://www.home-assistant.io/integrations/broadlink/
3. input_boolean helper for the state of the device
4. An automations to trigger the on/off IR/RF command upon hepler state change - you can use this blueprint - https://github.com/itamarb/home_assistant_blueprints/blob/main/broadlink/send_on_off_IR_commands.yaml


