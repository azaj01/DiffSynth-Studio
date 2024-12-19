# HunyuanVideo

HunyuanVideo is a video generation model trained by Tencent. We provide advanced VRAM management for this model, including three stages:

|VRAM required|Example script|Frames|Resolution|Note|
|-|-|-|-|-|
|80G|[hunyuanvideo_80G.py](hunyuanvideo_80G.py)|129|720*1280|No VRAM management.|
|24G|[hunyuanvideo_24G.py](hunyuanvideo_24G.py)|129|720*1280|The video is consistent with the original implementation, but it requires 5%~10% more time than [hunyuanvideo_80G.py](hunyuanvideo_80G.py)|
|6G|[hunyuanvideo_6G.py](hunyuanvideo_6G.py)|129|512*384|The base model doesn't support low resolutions. We recommend users to use some LoRA ([example](https://civitai.com/models/1032126/walking-animation-hunyuan-video)) trained using low resolutions.|

## Gallery

Video generated by [hunyuanvideo_80G.py](hunyuanvideo_80G.py) and [hunyuanvideo_24G.py](hunyuanvideo_24G.py):

https://github.com/user-attachments/assets/48dd24bb-0cc6-40d2-88c3-10feed3267e9

Video generated by [hunyuanvideo_6G.py](hunyuanvideo_6G.py) using [this LoRA](https://civitai.com/models/1032126/walking-animation-hunyuan-video):

https://github.com/user-attachments/assets/2997f107-d02d-4ecb-89bb-5ce1a7f93817