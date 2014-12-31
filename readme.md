# Using Webm as cover images

**the ultimate goal here is to be able to use webm videos in place of static images when picking a cover image for a website **

## Requirements, APIs, and Gems
this only uses pure CSS to accomplish the task, nothing special required.

## To use
1. require webmcover.css in html file
```
<link rel="stylesheet" type="text/css" href="webmcover.css">
```
- contents of webmcover.css
```
#bgmotion {
  position: fixed;
  top: -50%;
  left: -50%;
  width: 200%;
  height: 200%;
}
#bgmotion video {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  margin: auto;
  min-width: 50%;
  min-height: 50%;
}
```

- place div in html file
```
<div id="bgmotion">
<video autoplay loop
         src="http://i.imgur.com/j5V01xY.webm">
</video>
</div>
```

## Reasons for this:
- Below is a screenshot of a gif that was uploaded to http://gfycat.com

  - Video file was 1080p, pulled from youtube.

  - Link to gfycat - <a href=http://gfycat.com/DefenselessInstructiveCrocodileskink target=_blank>http://gfycat.com/DefenselessInstructiveCrocodileskink</a>

 <a href=images/shot.png target=_blank>
<img src=images/shot.png width=400>
</a>


- By enlarging the image, you can see the specs regarding the conversion to WebM:
  - Original Gif file was 13mb in size
  - WebM video file is 363k
  - 19.2:1 compression ratio
- Considerable load time instantly becomes zero.
- You can now utilize large, high resolution animations as cover images- with zero negative effects.
