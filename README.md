# RemoteDebugLauncher
VS Extension: Compile and invoke DebugAdapterHost.Launch 

First, prepare your project for remote debugging according to:
https://github.com/Microsoft/MIEngine/wiki/Offroad-Debugging-of-.NET-Core-on-Linux---OSX-from-Visual-Studio

Second, copy the `launch.json` created in first step to your solution or project folder.

Third, install this extension and press CTRL+ALT+SHIFT+F5.

This will trigger a build (of the current project using the current configuration) and start remote debugging afterwards by invoking `DebugAdapterHost.Launch /LaunchJson:"<solution/project-directory>\launch.json" `
