# Home Assistant Add-on: AMR2MQTT

[![GitHub Release][releases-shield]][releases]
![Project Stage][project-stage-shield]
[![License][license-shield]](LICENSE)

![Supports aarch64 Architecture][aarch64-shield]
![Supports amd64 Architecture][amd64-shield]
![Supports armhf Architecture][armhf-shield]
![Supports armv7 Architecture][armv7-shield]
![Supports i386 Architecture][i386-shield]

[![Github Actions][github-actions-shield]][github-actions]
![Project Maintenance][maintenance-shield]
[![GitHub Activity][commits-shield]][commits]
[![Community Forum][forum-shield]][forum]

_Runs rtlamr to read meter data and send to MQTT broker._

[![Open your Home Assistant instance and show the add add-on repository dialog
with a specific repository URL pre-filled.][add-repo-shield]][add-repo]
[![Open your Home Assistant instance and show the dashboard of a Supervisor add-on.][add-addon-shield]][add-addon]

## About

Allows you to use an rtl-sdr dongle to listen for signals from ERT compatible
smart meters using [rtlamr][rtlamr]. This runs as a daemon by launching rtl-tcp
and rtlamr, parsing the output and pushing it into MQTT so Home Assistant can
consume it.

This began as a port of ragingcomputer's [amridm2mqtt][amridm2mqtt] to a Home
Assistant add-on in order to make it easier to use in HAOS and supervised setups.
There are a number of other modifications as well such as support for other formats
like `scm` and a wider variety of MQTT configurations. Big thanks to ragingcomputer's
for their work as well as all the info in the `rtlamr` repo.

## Support

Got questions?

You have several ways to get them answered:

- The Home Assistant [Community Forum][forum]. I am
  [CentralCommand][forum-centralcommand] there.
- The Home Assistant [Discord Chat Server][discord-ha]. Use the #add-ons channel,
  I am CentralCommand#0913 there.

You could also [open an issue here][issue] on GitHub.

## Authors & contributors

The original setup of this repository is by [Mike Degatano][mdegat01].

For a full list of all authors and contributors,
check [the contributor's page][contributors].

[aarch64-shield]: https://img.shields.io/badge/aarch64-yes-green.svg
[add-addon-shield]: https://my.home-assistant.io/badges/supervisor_addon.svg
[add-addon]: https://my.home-assistant.io/redirect/supervisor_addon/?addon=39bd2704_amr2mqtt
[add-repo-shield]: https://my.home-assistant.io/badges/supervisor_add_addon_repository.svg
[add-repo]: https://my.home-assistant.io/redirect/supervisor_add_addon_repository/?repository_url=https%3A%2F%2Fgithub.com%2Fmdegat01%2Fhassio-addons
[amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg
[amridm2mqtt]: https://github.com/ragingcomputer/amridm2mqtt
[armhf-shield]: https://img.shields.io/badge/armhf-yes-green.svg
[armv7-shield]: https://img.shields.io/badge/armv7-yes-green.svg
[commits-shield]: https://img.shields.io/github/commit-activity/y/mdegat01/addon-amr2mqtt.svg
[commits]: https://github.com/mdegat01/addon-amr2mqtt/commits/main
[contributors]: https://github.com/mdegat01/addon-amr2mqtt/graphs/contributors
[discord-ha]: https://discord.gg/c5DvZ4e
[forum-centralcommand]: https://community.home-assistant.io/u/CentralCommand/?u=CentralCommand
[forum-shield]: https://img.shields.io/badge/community-forum-brightgreen.svg
[forum]: https://community.home-assistant.io/t/home-assistant-add-on-amr2mqtt/378196
[mdegat01]: https://github.com/mdegat01
[github-actions-shield]: https://github.com/mdegat01/addon-amr2mqtt/workflows/CI/badge.svg
[github-actions]: https://github.com/mdegat01/addon-amr2mqtt/actions
[i386-shield]: https://img.shields.io/badge/i386-no-red.svg
[issue]: https://github.com/mdegat01/addon-amr2mqtt/issues
[license-shield]: https://img.shields.io/github/license/mdegat01/addon-amr2mqtt.svg
[maintenance-shield]: https://img.shields.io/maintenance/yes/2022.svg
[project-stage-shield]: https://img.shields.io/badge/project%20stage-production%20ready-brightgreen.svg
[ragingcomputer]: https://github.com/ragingcomputer
[releases-shield]: https://img.shields.io/github/release/mdegat01/addon-amr2mqtt.svg
[releases]: https://github.com/mdegat01/addon-amr2mqtt/releases
[rtlamr]: https://github.com/bemasher/rtlamr
