---
layout: post
title: VideoProcessing — LSDVE OpenCV Video Annotation Tool
date: 2015-01-01 00:00:00 +0300
description: OpenCV-based video annotation tool (LSDVE) that lets users interactively draw and remove lines on video frames, saving annotated results to a custom .lsd file format.
img: # no image in README
tags: [computer-vision, video, opencv, annotation]
---

LSDVE (LSD Video Editor) is an OpenCV-based video annotation tool that makes video editing and annotation easier. It allows users to interactively draw and remove lines on video frames, saving the annotated results to a custom `.lsd` file format.

## Supported Operations

- **Right-click** — pause/resume the video
- **Left-click** — select two points for a line (press down and press up)
- **(A)dd** — add a new line
- **(R)emove** — remove line in area selected by mouse
- **(Q)uit & save** — quit and save annotations
- **(S)ave** — save the current frame and advance to next
- **(U)ndo** — undo last action

## Output Format

Annotations are stored in a `.lsd` file with this format:

```
frame:INT       <- frame number in the original video
lines:INT       <- number of lines in this frame
line1_X1,line1_Y1,line1_X2,line1_Y2
line2_X1,line2_Y1,line2_X2,line2_Y2
...
frame:INT
lines:INT
```

## Build

```bash
cmake .
killall -9 lsdvideo ; make ; ./lsdvideo bird.avi out.lsd
```

### Links

[VideoProcessing GitHub repository](https://github.com/ebadi/VideoProcessing)
