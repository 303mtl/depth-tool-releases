# 303 Depth Tool

Downloads and automatic updates for the 303 Depth Tool on macOS and Windows. Only the finished app lives here. The source code stays private.

## What it does

Drop in any video and it turns into a live, audio reactive depth visual. An AI model estimates depth right on your computer, so a flat clip becomes a 3D point cloud, a LiDAR scan or a thermal look. No Kinect and no sensor, just the video.

You get ten looks to start from, like KINECT RED, LIDAR WHITE, THERMAL SCAN and RGB POINT CLOUD. Save any look to a scene and recall it with one click while you play. Feed it a live audio input and the visuals move with the music.

When it is time to go on screen, the output goes straight into Resolume, OBS or TouchDesigner. Syphon (Mac) or Spout (Windows) handles it locally on the same machine, and NDI sends it over the network, even between a Mac and a PC. When you want a file instead, it exports in H.264, H.265 or ProRes 4444 with alpha.

## Download

**Mac:** [Get the latest version](https://github.com/303mtl/depth-tool-releases/releases/latest) and download the `.dmg`.

**Windows:** [Download the installer](https://github.com/303mtl/depth-tool-releases/releases/download/win-v1.0.3/KinectDepthStudio-Setup.exe) (about 650 MB).

## Installing on a Mac

Open the dmg and drag the app onto your Applications folder. The first time you open it, macOS will block it, because the app is not notarised by Apple. Go to System Settings, then Privacy and Security, scroll to the bottom and click Open Anyway, then confirm.

If macOS says the app is damaged instead, open Terminal once and run this line:

```
xattr -dr com.apple.quarantine "/Applications/Kinect Depth Studio.app"
```

After that first launch you never have to do it again. When a new version comes out, the app tells you on startup and updates itself with one click.

You need an Apple Silicon Mac (M1 or newer) on macOS 14 Sonoma or later. NDI output needs the free NDI Tools runtime installed.

## Installing on Windows

Run `KinectDepthStudio-Setup.exe`. Windows will warn you with "Windows protected your PC", because the app is not signed. Click More info, then Run anyway. The installer needs no admin rights and puts the app in your own user folder, with a Start menu entry.

Like on the Mac, the app checks for new versions on startup and updates itself with one click.

You need 64 bit Windows 10 or 11. Depth analysis runs on the processor, so the first analysis of a clip takes longer than on a Mac. Every clip is analysed only once and then cached. Exports use your graphics card's encoder (NVIDIA, Intel or AMD) when it has one. For Spout output in Resolume, pick it under Sources, then Spout. NDI output needs the free NDI Tools runtime.

## Thanks

Big thanks to Giannis Veronis ([@giannisveronis](https://github.com/giannisveronis)) for the Scenes idea and the NDI output.
