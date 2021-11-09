# esphome-AirGradient

esphome config for AirGradient air quality sensor

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/ajfriesen)




The AirGradient DIY Air Quality Sensor can be found here: https://www.airgradient.com/diy/

This repository is only for using with ESPHome and Home Assistant.

Requirement:

- Already setup and running [Home Assistant](https://www.home-assistant.io/installation/)

1. Add ESPHome addon

<a href="https://my.home-assistant.io/redirect/supervisor_addon/?addon=a0d7b954_esphome" target="_blank"><img src="https://my.home-assistant.io/badges/supervisor_addon.svg" alt="Open your Home Assistant instance and show the dashboard of a Supervisor add-on." /></a>

2. Download whatever font you feel fancy. [ESPHome font docs](https://esphome.io/components/display/index.html#drawing-static-text)
3. Add your secrets (You can also hardcode them in the `air-gradient.yaml` but I would recommend to split these)

You can either create a separate `secrets.yaml` with your secrets in this file like so:

```YAML
# WIFI
wifi_ssid: ""
wifi_password: ""

# OTA
ota_password: ""

#AP
fallback_ssid_password: ""
```

or you can just include your Home Assistant `secrets.yaml`:
[How do I use my Home Assistant secrets.yaml?](https://esphome.io/guides/faq.html?highlight=secret#how-do-i-use-my-home-assistant-secrets-yaml)

3. Plug in your AirGradient

You can either plug it in the device running Home Assistant or your laptop/PC.

4. Add a new device

ESPHome will ask you for a name and your WiFi credentials.
You can put in anything you want and change the later steps.

5. Edit your device and change the config

Now you just need to copy thte content of the `air-gradient.yaml` into the editor

6. Save and install

This will take a minute or two. ESPHome will compile the binary for your AirGradients ESP8266.

7. Add your device to Home Assistant

Go to Home Assistant: <a href="https://my.home-assistant.io/" target="_blank"><img src="https://my.home-assistant.io/badges/supervisor_addon.svg" alt="Open your Home Assistant instance." /></a>

In the notification panel should be an new device available to set up.
Your new AirGradient Sensor.

8. Your turn

Now it is your turn to do something silly or usefull with the air quality sensor.

