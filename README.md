# TikTok-Api
TikTok Api wrapper without authentication


# This is not finished, i will be updating this repo regularly


###FYP
```py
from TTApi import TikTokApi

tiktok = TikTokApi(debug=True)

# Params are region, count & cursors
fyp_videos = tiktok.feed.for_you()

for video in fyp_videos:
    tiktok.video.download_video(video["video_url"])
```

DL video
```py
from TTApi import TikTokApi


tiktok = TikTokApi(debug=True)

tiktok.video.download_video("https://www.tiktok.com/t/ZTRf85djY/", watermark=True) # Watermarked
tiktok.video.download_video("https://vm.tiktok.com/ZMNnX3Q4q/", watermark=False) # No watermark
```
