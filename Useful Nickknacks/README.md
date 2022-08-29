- Connecting to other computer on the same network using ssh
  ssh://user_name@ip_address
- VLC player
  - Open VLC player
  - Use CTRL+N
  - In NETWORK rtsp://admin:aitoe2016@192.168.0.202. Replace  192.168.0.202 with your camera IP.
  - Go to VLC icon on the top right corner and press record and quit (I guess press it again) it will show up on your videos folder in HOME.

- FFMPEG useful commands
  Command to convert .dav to mp4
  `ffmpeg -y -i input-file.dav -vcodec libx264 -crf 24 -filter:v "setpts=1*PTS" output-file.mp4`

  Convert images to video
  `ffmpeg -r 5 -i %d.jpg -c:v libx264 -vf fps=25 -pix_fmt yuv420p test.mp4`

  Convert video to images
  `ffmpeg -i input.mp4 -vf fps=1 out%d.png`

  Extract time from video
  `ffmpeg -i officeBaggageDetection.mp4 -ss 00:00:05 -to 00:00:20 -c copy -async 1 officeBaggageDetectionCut.mp4`

  Crop video based on time → tested
  `ffmpeg -i Atm15.mp4 -ss 00:05:15 -to 00:08:50 -async 1 TestCases/Atm5.mp4`

  Compress the videos 
  `ffmpeg -i input.mp4 -vcodec libx264 -crf 20 output.mp4`

- Accessing GPU remotely
  `ssh name@xxx.xxx.x.xx` 
  `screen -ls`
  - To make your own screen or instance on GPU
    - `screen -S Name`
    - `screen -ls`
  - To run a particular screen
    `screen -r screen_name`
  - To detach and close a screen
    **CTRL+A+D** 
  - To kill 
    **CTRL+D**
  - Log out from the screen
    `exit`


