# Cast-Away
Repository for my talk at HOPE 2022, Cast Away, focusing on remote control and live video data exploration

[Video link to the presentation](https://www.youtube.com/watch?v=JKRFwzZPj20)
I should also try to do public speaking more often than once every 5+ years. I also doubt I am originating the field of technical narrative analysis but it is definitely a rich source of data.

As mentioned in the video, I didn't get to work on the project as much as I wanted when I was actually at HOPE because they decided to make the network more secure, which is great for everyone, unless you are trying to SSH to another host.

I'm mostly working on this offline and will push completed sections here when they are ready.


TODO / Next steps:
1. Background and justification
  * Humans like stories and don't like being bored
  * Narrative is important to how we understand the world and build our own identities
  * What if we can get the computer to watch TV for us?

2. Hardware
  * What is available now (SBC, DVR, case, heatsinks, fan, HDMI capture, etc)
  * Installation and setup

3. Some simple live video streaming examples

4. Getting the remote working
  * IR in modern Linux kernels
  * Hardware construction and setup
  * Capturing and sending IR codes
  * Setting up our web interface

5. More background information
  * [Article on movie barcodes](https://thefilmstage.com/movie-barcode-an-entire-feature-film-in-one-image/) - [Movie barcodes on Twitter](https://twitter.com/moviebarcodes)
  * Color grading

6. Introduction to image processing
  * Color histograms inspired by the movie barcodes
  * Feature / Commercial detection (Aside: using I-frames for already-encoded/compressed video)
  * Object detection with YOLOvN - because we are doomed to preserve fossilized pop culture artifacts in code

7. Lessons learned
  * Video processing will eat as much CPU as you give it
  * DVR won't tune analog signals, so automated VHS 2-pass caption recognition wouldn't be possible
  * DVR UI slows down if the unit is on for several days
