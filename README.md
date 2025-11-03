# Home Assistant add-on repository for Casnic

This repository allows you to install the Homeassistant Addon package for the Casnic Controller: <https://gitlab.com/bitsii/CasCon>

[![Open your Home Assistant instance and show the add add-on repository dialog with this repository pre-filled.](https://my.home-assistant.io/badges/supervisor_add_addon_repository.svg)](https://my.home-assistant.io/redirect/supervisor_add_addon_repository/?repository_url=https%3A%2F%2Fgithub.com%2Fbitsii%2Faddons-casnic)

You will need the MQTT configuration and a configured broker to use CasCon.  If you do not yet have MQTT setup for Home Assistant, please first install the Mosquitto addon <https://github.com/home-assistant/addons/blob/master/mosquitto/README.md>.  After installation install the MQTT Integration as well - it will show as an auto-discovered service under Notifications / New Devices Discovered.

After your MQTT integration is ready, add this repository with the above button, and then go to Settings / Addons and search for and install this addon, Casnic Controller.

After installation go to Settings / Addons / Casnic and Start the Addon, and set it to Start on boot.  The addon will automatically configure itself to use your MQTT integration.

Once started you can click on Open Web UI, you can login using your Home Assistant account info, and you will be ready to add devices configured via the Casnic Controller mobile application (IOS) <https://apps.apple.com/us/app/cascon/id6458984046> (Android)<https://play.google.com/store/apps/details?id=casnic.control>

Further help is available here - <https://gitlab.com/bitsii/CasCon/-/wikis/Casnic>

Further detail about the addon and how it works is available here - <https://github.com/bitsii/addons-casnic/wiki>

**If you have difficulties with the plugin** you could consider using the Integration Hub instead.  Check [here](https://gitlab.com/bitsii/CasCon/-/wikis/Working-with-other-home-automation-hubs) for more information.

## Add-ons

This repository contains the following add-ons

### [Casnic Controller](./casnic)

![Supports aarch64 Architecture][aarch64-shield]
![Supports amd64 Architecture][amd64-shield]
![Supports armhf Architecture][armhf-shield]
![Supports armv7 Architecture][armv7-shield]
![Supports i386 Architecture][i386-shield]

<!-- from https://github.com/hassio-addons/addon-debian-base -->
<!--

Notes to developers after forking or using the github template feature:
- While developing comment out the 'image' key from 'example/config.yaml' to make the supervisor build the addon
  - Remember to put this back when pushing up your changes.
- When you merge to the 'main' branch of your repository a new build will be triggered.
  - Make sure you adjust the 'version' key in 'example/config.yaml' when you do that.
  - Make sure you update 'example/CHANGELOG.md' when you do that.
  - The first time this runs you might need to adjust the image configuration on github container registry to make it public
  - You may also need to adjust the github Actions configuration (Settings > Actions > General > Workflow > Read & Write)
- Adjust the 'image' key in 'example/config.yaml' so it points to your username instead of 'home-assistant'.
  - This is where the build images will be published to.
- Rename the example directory.
  - The 'slug' key in 'example/config.yaml' should match the directory name.
- Adjust all keys/url's that points to 'home-assistant' to now point to your user/fork.
- Share your repository on the forums https://community.home-assistant.io/c/projects/9
- Do awesome stuff!
 -->

[aarch64-shield]: https://img.shields.io/badge/aarch64-yes-green.svg
[amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg
[armhf-shield]: https://img.shields.io/badge/armhf-yes-green.svg
[armv7-shield]: https://img.shields.io/badge/armv7-yes-green.svg
[i386-shield]: https://img.shields.io/badge/i386-yes-green.svg
