## Commands

### Url

#### How to get the url

1. Open the Threads app and copy the profile link.
2. Paste the link into any browser and select a video.
![Image](sc)
3. Click on the three dots in the right corner.
4. Choose the option to copy the link.
5. The url will look like this `https://www.threads.net/@foodnetwork/post/Cu19A2IrEug`

#### Single Url

To specify video url you need to use `--url` or `-u` command

```markdown
py app.py --url video_url
```

#### Multiple Url

1. To use multiple url you need to have a text file with urls separated with newline. `e.g.`

```txt
url1
url2
url3
....
```

2. To use this file you need to `--input` or `-i` command.

```markdown
py app.py -d -i path_of_the_text file --url video_url 
```

`e.g.`

```markdown
py app.py -d -i ./url.txt file --url video_url 
```

### Downloading 

For downloading videos use `-d` command.

```markdown
py app.py -d --url video_url
```

### Saving The File

#### Specify the file name (Only single url)

The path of video saving the video `--output` or `-o`. `e.g.`
```bash
py app.py -d --url video_url --output path/file_name.ext
```

`note : --output is optional by default ./videos/file_name.ext`

#### Specify the Saving directory (Both single and multiple url)

The directory of video saving directory of video  `-dir` 
```bash
py app.py -d --url video_url --dir path/
```

`note : --dir is optional by default ./videos/`


[sc]:https://github.com/Tonmoy-abc/threads-video-downloader/blob/main/img/sc.png?raw=true