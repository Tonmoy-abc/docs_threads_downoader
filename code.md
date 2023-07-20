## Use in python codes

1. After installing everything import the Video class form `video.py`
```python
from video import Video
```

2. For downloading video you need to call the Video object and call the download method. Video object has 4 parameters.

| Name        | Type                   | Used for                         |
| ----------- | ---------------------- | -------------------------------- |
| url         | str                    | url of video                     |
| session     | requests.Session       | session                          |
| savePath    | str (optional) \| None | path of the video (default None) |
| saveDir     | str                    | directory of saving video (default ./videos)|

`Note: if savePath==None then savePath will be video author name+caption+currentTime.extension`
Example:

```python
video = Video(url, session, savePath, saveDir)
video.download()
```