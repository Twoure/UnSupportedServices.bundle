UnSupported Services
====================

This is a plugin that creates a new system _Services_ channel in [Plex Media Server](https://plex.tv/) (PMS) to supplement the current official [Services.bundle](https://github.com/plexinc-plugins/Services.bundle).  The intent of this channel is to keep a centralized list of host available to multiple channels just as the current Services bundle does, with the key difference that this channel updates/installs separately from the main Services bundle and will be avaialbe outside of PMS releases.

I plan to make a few channels that will require this UnSupported Services channel.  Since PMS service code is delegated via alphanumeric listing, this will solve the issue created when making channels that require the same video host.

> **Note:** the author of this plugin has no affiliation with any of the video host provided by this channel nor the owners of the content that they host.

## Install

#### Auto
- ~~Install via [WebTools.bundle](https://github.com/dagalufh/WebTools.bundle)~~  _(Not yet added to UASv2)_
- ~~Restart PMS~~

#### Manual

- [Download](https://github.com/Twoure/UnSupportedServices.bundle/archive/master.zip) and install by following the Plex [instructions](https://support.plex.tv/hc/en-us/articles/201187656-How-do-I-manually-install-a-channel-) or the instructions below.
  - Unzip and rename the folder to **UnSupportedServices.bundle**
  - Copy **UnSupportedServices.bundle** into the PMS [Plug-ins](https://support.plex.tv/hc/en-us/articles/201106098-How-do-I-find-the-Plug-Ins-folder-) directory
  - Restart PMS

## Issues

- **FileNuke** / **ShareSix**
  - If the Video Thumb is black then the video/thumb host domain is down
  - Basically if the video thumb is not black, then the video should play
- **Zalaa** / **Uploadc**
  - Video URL needs `User-Agent` and `Referer` to work.  I have included them in the code, but Plex still cannot play them.
  - Still looking into, but might have to scrap for now
- **NeoDrive** / **CloudZilla**
  - Able to parse and download the Video URL, but Plex will not play the stream
  - Think it has to do with a missing header value, not sure, still working on this one
- **Vid.ag**
  - The host is down for _"maintenance"_
  - Will see if they come back, not sure
- **PromptFile** / **Briskfile**
  - The host does not like Kodi parsing them, and has started to implement some obfuscation
  - Currently works, but may be susceptible to breaking later
- **MightyUpload**
  - The server they use is currently offline so videos cannot load
- **DaClips**
  - Normally included within XFileShare code, but is now behind cloudflare anit scrape bot
  - Would need to implement cfscrape and require JavaScript to parse souce
- **GorillaVid**
  - Thumbs redirect to DaClips, but do not exist there either

## [Changelog](Changelog.md#changelog)
