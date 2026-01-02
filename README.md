# Tdarr-Flow-for-Normal-People
A generalised set of Tdarr flows that will suit normal people - please ignore all you 850TB harddrive owners.

My goal was to create a flow that will transform large movie/tv show files into manageable, decent looking and easily streamable file sizes for remote viewing by jellyfin/emby/plex.
Will convert any files you point it at into 1080p 265x hevc/H.265 mp4 files with 256kbps AAC audio. It will try and strip out any extra language/subtitle files. I've used the hvc1 codec tag so files will play well on apple devices.

This flow was heavily based on the video flow by Primal Curve (https://gist.github.com/primalcurve) and the audio element of this flow by Nexus (https://www.reddit.com/r/Tdarr/comments/1okb7af/my_h264_aac_mp4_flow_direct_play_everywhere/)

Please note that this flow will frequently remove all subtitle files on older codecs - this seems unfortunately necessary for the transcoding to work. 

## Installation guide
**You need both the flows in the repository for these flows to function**.
Copy and paste each into the import JSON section of the flows. You will need to add your own api information and the location of your sonarr/radarr server if you want to have this functionality - otherwise just delete or disable these modules in the flow. 

Create a library and set the "HEVC (Balanced Quality) + AAC (256k) Flow" as the transcode method. 

I'm using this set up on my Ugreen NAS which has an intel GPU.
