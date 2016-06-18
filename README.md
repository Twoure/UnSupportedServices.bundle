UnSupported Services
====================

This is a plugin that creates a new system _Services_ channel in [Plex Media Server](https://plex.tv/) (PMS) to supplement the current official [Services.bundle](https://github.com/plexinc-plugins/Services.bundle).  The intent of this channel is to keep a centralized list of host available to multiple channels just as the current Services bundle does, with the key difference that this channel updates/installs separately from the main Services bundle and will be avaialbe outside of PMS releases.

I plan to make a few channels that will require this UnSupported Services channel.  Since PMS service code is delegated via alphanumeric listing, this will solve the issue created when making channels that require the same video host.

> **Note:** the author of this plugin has no affiliation with any of the video host provided by this channel nor the owners of the content that they host.

## Install

#### Auto
- Install via [UnSupportedServicesTools.bundle](https://github.com/Twoure/UnSupportedServicesTools.bundle)

#### Manual

- [Download](https://github.com/Twoure/UnSupportedServices.bundle/releases) the latests release and install by following the Plex [instructions](https://support.plex.tv/hc/en-us/articles/201187656-How-do-I-manually-install-a-channel-) or the instructions below.
  - Unzip and rename the folder to **UnSupportedServices.bundle**
  - Copy **UnSupportedServices.bundle** into the PMS [Plug-ins](https://support.plex.tv/hc/en-us/articles/201106098-How-do-I-find-the-Plug-Ins-folder-) directory
  - Restart PMS

## Upgrade

#### Auto
- Use the [UnSupportedServicesTools.bundle](https://github.com/Twoure/UnSupportedServicesTools.bundle) to upgrade the **UnSupportedServices.bundle**

#### Manual
- Delete current **UnSupportedServices.bundle** from PMS [Plug-ins](https://support.plex.tv/hc/en-us/articles/201106098-How-do-I-find-the-Plug-Ins-folder-) directory
- Continue by following the [Manual Install](#manual) directions
- **Important:** make sure to restart PMS after manually installing

## Issues

- **FileNuke** / **ShareSix**
  - If the Video Thumb is black or looks like [this](http://i.imgur.com/GEKTJP3.png) then the video/thumb host domain is down
  - Basically if the video thumb is from the video, then the video should play
- **Zalaa** / **Uploadc** _not active code_
  - Video URL needs `User-Agent` and `Referer` to work.  I have included them in the code, but Plex still cannot play them.
- **NeoDrive** / **CloudZilla** _not active code_
  - Able to parse and download the Video URL, but Plex will not play the stream
  - Think it has to do with a missing header value, not sure
- **Vid.ag** _not active code_
  - The host is down for _"maintenance"_
  - Will see if they come back, not sure
- **PromptFile** / **Briskfile**
  - The host does not like Kodi parsing them, and has started to implement some obfuscation
  - Currently works, but may be susceptible to breaking later
- **MightyUpload** _not active code_
  - The server they use is currently offline so videos cannot load
- **GorillaVid**
  - Thumbs redirect to DaClips, but do not exist there either
  - Added fallback thumb for now
- **Openload**
  - Started kodi anti-scrape measures.  Works for now, kinda.

## [Changelog](Changelog.md#changelog)
