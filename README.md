# RecordScreenRegionVideo

# The Idea
There's available a variety of applications for GNU/Linux distributions that are capable of screencasting/recording the screen video. Nevertheless, oftentimes they require many dependencies/flatpak runtimes, or design-wise are aimed at bigger desktop environments like KDE Plasma, GNOME.

The offerred solution is preferable for users with the following goals in mind:
1. Minimalism: few dependencies in form of [ffmpeg](https://ffmpeg.org/) and [slop](https://github.com/naelstrof/slop) available in distro repositories and a simple script.
2. One use-case: recording of the specified screen region.
3. No UI: starting and pausing the recording with one shortcut and mouse selection.
4. Works with X11 desktop environments, like Xfce, which haven't migrated to Wayland yet.
5. Adherence to UNIX-philosophy: do one thing and do it well.

# Usage
The recommended use for the script consists of the following steps:
1. Copy it to ~/.local/bin/.
2. Make it executable (`chmod +x record_screen_region_video`).
3. Create a shortcut for the script, like `Super + V`, to start and stop the recording:

![image](https://github.com/JayXT/RecordScreenRegionVideo/assets/8045344/0efb0df7-0e33-4ee4-9dea-821f13e6421a)

The video files are saved to ~/Downloads directory.

# Modifications

If need be, the ffmpeg command could be modified to also record audio, use different encoders, etc.


