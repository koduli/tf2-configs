## TF2 Launch Options

### Video / Rendering

**-novid** - Skips the Valve intro video (faster startup).<br>
**-fullscreen** - Forces fullscreen mode.<br>
**-windowed** or **-sw** - Forces windowed mode.<br>
**-noborder** - Removes window borders (good for borderless windowed fullscreen).<br>
**-w <width> / -h <height>** - Sets resolution width/height manually (e.g. -w 1920 -h 1080).<br>
**-refresh <hz>** - Forces monitor refresh rate (useful if TF2 picks the wrong one).<br>
**-dxlevel <version>** - Forces DirectX level (81, 90, 95, 98). Only use once — remove after the first launch or it resets your settings each time.<br>
**-softparticlesdefaultoff** - Disables soft particles by default (saves GPU).

### Input / Controller

**-nojoy** - Disables joystick support (slightly faster load).<br>
**-nosteamcontroller** - Disables Steam Input controller system.<br>
**-useforcedmparms -noforcemaccel -noforcemspd** - Forces Windows mouse acceleration settings off. (Only matters if you haven't already set raw input with m_rawinput 1.)

### Performance / Memory

**-reuse** - Reuses render context between map loads (can shorten load times).<br>
**-high** - Forces TF2 to run in high CPU priority. Can cause instability if your PC is multitasking.<br>
**-threads <num>** - Forces number of processor threads. Generally not recommended — let Source handle it.<br>
**-nocrashdialog** - Suppresses Windows error popups (closes TF2 directly on crash).<br>
**-noasync** - Disables async sound loading (can reduce stutter at cost of longer load times).<br>
**-limitvsconst** - Forces a limited number of vertex shader constants (old GPUs only).<br>
**-particles <num>** - Controls particle detail (1 = lowest).

### Network

**-tcp** - Forces Steam to use TCP instead of UDP. Usually slower, only for troubleshooting connection issues.

### Debug / Misc

**-console** - Opens developer console on startup.<br>
**-autoconfig** - Resets video/audio settings to default based on hardware (one-time use).<br>
**-safe** - Starts TF2 in safe mode with minimal video settings.<br>
**-nobreakpad** - Disables Valve's crash reporting tool.<br>
**-nocrashdialog** - Suppresses Windows crash dialogs.<br>
**-condebug** - Writes console output to console.log in your TF2 folder. Useful for debugging configs.
