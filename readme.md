# ffmpeg-cheatsheet
A list of useful commands for ffmpeg 🎞

## Resize
`ffmpeg -i input.avi -vf scale=320:240 output.avi`

To keep aspect ratio (some codes require height divisible by 2) :
`ffmpeg -i input.avi -vf scale=320:-2 output.avi`

## Reduce file size
`ffmpeg -i input.mp4 -vcodec libx265 -crf 20 output.mp4`

## WebM
`ffmpeg -i input.mp4 -c:v libvpx-vp9 -b:v 2M output.webm`
