# ChangeLog

##### 1.0.2
 - _06/25/16_
   - Fixes:
     - MP4Upload - site added a fake blank.mp4 file, local var error
     - ShareSix - `go_next` changed
     - FlashX - dictionary error
     - Vidgg - `id` issue
     - WholeCloud - regex ignore case
     - Openload - header, title, embed url, and redirect errors
     - VShare - fixed for site changes, no longer uses jspacker code, and now requires referer in header to get proper video host IP
   - Updates:
     - New Host: VideoNest, VidWatch, Uploadx, Bestream, VidSpot, StreamMoe, TusFiles, NosVideo (but disabled due to issues Playing final URL)
     - NeoDrive - Re-enabled, in testing phase, very unstable
     - XFileShare:
       - Better error handling
       - Removed force transcoding from AllMyVidoes, DaClips, and Movpod because they do not have IP specific hashes
       - Cleaned regex and if/else statements
     - WholeCloud:
       - Improved URL error handling
       - Updated Vidgg to match old url Vid.gg too
       - NormalizeURL() now catches URL redirects
     - VShare and Uploadx - changed post data to values
     - FlaseX - Moved sleep into HTML.ElementFromURL, cleand code
     - VidWatch - simplified duration value
     - VidUp - regex to ignore vidup.org, not same site
     - TheVideoBee - Disabled due to SSL error

##### 1.0.1
 - _06/17/16_
   - Fixes:
     - Openload - site changes
     - Promptfile - maintenace warning issue
   - Updates:
     - Added new host - MP4Upload
     - Added new host/search - XVIDSTAGE
     - Added DaClips back, no longer behind anti-cloudflare code

##### 1.0.0
 - _06/17/16_
   - Initial Version
   - Dummy place holder for testing new install service

##### 05/27/16
- Initial push of local code
- No internal updater, so for now no release is planned
  - May do a release later, once bundle becomes more stable, not sure yet
