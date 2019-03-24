# RemoteDebugLauncher
VS Extension: Compile and invoke DebugAdapterHost.Launch 

1. Prepare your project for remote debugging according to:
https://github.com/Microsoft/MIEngine/wiki/Offroad-Debugging-of-.NET-Core-on-Linux---OSX-from-Visual-Studio

2. Set the output build path to a network share and configure `launch.json` accordingly.

3. Copy the `launch.json` created in steps 1 and 2 to your solution or project folder.

4. Install this extension.

Now you can press CTRL+ALT+SHIFT+F5. This will trigger a build (of the current project using the current configuration) and start remote debugging afterwards by invoking `DebugAdapterHost.Launch /LaunchJson:"<solution/project-directory>\launch.json" `
