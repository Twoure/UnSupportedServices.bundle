# ChangeLog

##### 1.0.2
- _07/04/16_
- **Fixes:**
  - MP4Upload - site added a fake blank.mp4 file, local var error
  - ShareSix - `go_next` changed
  - FlashX - dictionary error
  - Vidgg - `id` issue
  - WholeCloud - regex ignore case
  - Openload:
    - header, title, embed url, and redirect errors
    - improved title matching
  - VShare - fixed for site changes, no longer uses jspacker code, and now requires referer in header to get proper video host IP
  - Vidto - fixed url norm, thumb, duration, source_title
  - Zalaa - update code for site changes, and found the final video URL needs the referer set in headers
    - Disabled due it Plex Framework inability to set referer value in video stream
  - HappyStreams - removed MP4 container, sometimes it's FLV
  - Nos(video/locker) - MP4 IP Hash wrong, so using RTMP stream for now
- **Updates:**
  - Improved Regex for all sites, and added Fallback Thumb for all active code
  - New Host:
    - VideoNest, VidWatch, Uploadx, Bestream, VidSpot, StreamMoe, TusFiles, HappyStreams
    - Cloudy, VideoRaj, VideoMega, iDoWatch, LetWatch, GoodVideoHost, YourVideoHost, WatchOnline
    - Exashare, Ajihezo, PicStream, SpeedVid, AllVid, FastStream, WatchVideo, VidBull, NosLocker
    - TheVideos
  - NeoDrive - Re-enabled, seems to work for now
  - FileNuke - Disabled, site offline
  - XFileShare:
    - Better error handling, and added url error check
    - Removed force transcoding from AllMyVidoes, DaClips, and Movpod because they do not have IP specific hashes
    - Cleaned regex and if/else statements
    - Updated embed url regex, simplified source_title code
  - WholeCloud:
    - Improved URL error handling
    - Updated Vidgg to match old url Vid.gg too
    - NormalizeURL() now catches URL redirects
    - Updated source_title code
    - Added ssl check, redirect to http when https fails on ssl error
    - Updated regex to match old embed url types
  - VShare and Uploadx - changed post data to values
  - FlashX - Moved sleep into HTML.ElementFromURL, cleand code
  - VidWatch - simplified duration value
  - VidUp - regex to ignore vidup.org, not same site
    - added fallback thumb, simplified source_title
    - added more try/except code when requesting URLs
  - TheVideoBee - Disabled due to SSL error
  - VidSpot - imporoved code for URL variations
  - ShareRepo - Disabled, host server offline for most videos, and/or timesout Plex Client
  - Faststream.in - included in official Services.bundle, so using regex trick to allow my code to work when url prefixed with `uss/`
  - Added Global Search for the following host:
    - VidWatch, Cloudy, VideoRaj, VidSpot

##### 1.0.1
- _06/17/16_
- **Fixes:**
  - Openload - site changes
  - Promptfile - maintenace warning issue
- **Updates:**
  - Added new host - MP4Upload
  - Added new host/search - XVIDSTAGE
  - Added DaClips back, no longer behind anti-cloudflare code

##### 1.0.0
- _06/17/16_
- Initial Version
- Dummy place holder for testing new install service

##### 0.0.0
- _05/27/16_
- Initial push of local code
- No internal updater, so for now no release is planned
  - May do a release later, once bundle becomes more stable, not sure yet
