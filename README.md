UnSupported Services
====================

This plugin creates a new system _Services_ channel within [Plex Media Server](https://plex.tv/) (PMS) to supplement the current official [Services.bundle](https://github.com/plexinc-plugins/Services.bundle).  The intent of this channel is to keep a centralized list of host available to multiple channels just as the current Services bundle does, with the key difference that this channel updates/installs separately from the main Services bundle and will be avaialbe outside of PMS releases.

I plan to make a few channels that will require this UnSupported Services channel.  Since PMS service code is delegated via alphanumeric listing, this will solve the issue created when making channels that require the same video host.

> **Note:** the author of this plugin has no affiliation with any of the video host provided by this channel nor the owners of the content that they host.

## Install

#### Auto
- Install via [UnSupportedServicesTools.bundle](https://github.com/Twoure/UnSupportedServicesTools.bundle)

#### Manual

- [Download](https://github.com/Twoure/UnSupportedServices.bundle/archive/master.zip) the channel and install it by following the Plex [instructions](https://support.plex.tv/hc/en-us/articles/201187656-How-do-I-manually-install-a-channel-) or the instructions below.
  - Unzip and rename the folder to **UnSupportedServices.bundle**
  - Copy **UnSupportedServices.bundle** into the PMS [Plug-ins](https://support.plex.tv/hc/en-us/articles/201106098-How-do-I-find-the-Plug-Ins-folder-) directory
  - Unix based platforms need to `chown plex:plex -R UnSupportedServices.bundle` after moving it into the Plug-ins directory _(`user:group` may differ by platform)_
  - **Restart PMS**

## Upgrade

#### Auto
- Use the [UnSupportedServicesTools.bundle](https://github.com/Twoure/UnSupportedServicesTools.bundle) to upgrade the **UnSupportedServices.bundle**

#### Manual
- Delete current **UnSupportedServices.bundle** from PMS [Plug-ins](https://support.plex.tv/hc/en-us/articles/201106098-How-do-I-find-the-Plug-Ins-folder-) directory
- Continue by following the [Manual Install](#manual) directions
- **Important:** make sure to restart PMS after manually installing

## [Issues](https://github.com/Twoure/UnSupportedServices.bundle/wiki/Issues)

## [Host List](https://github.com/Twoure/UnSupportedServices.bundle/wiki/Host-list)

## [Changelog](Changelog.md#changelog)
