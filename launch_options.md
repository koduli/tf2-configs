## TF2 Launch Options Cheat Sheet

### 🎥 Video / Rendering

- **-novid** - Skips the Valve intro video (faster startup).
- **-fullscreen** - Forces fullscreen mode.
- **-windowed** or **-sw** - Forces windowed mode.
- **-noborder** - Removes window borders (good for borderless windowed fullscreen).
- **-w <width> / -h <height>** - Sets resolution width/height manually (e.g. -w 1920 -h 1080).
- **-refresh <hz>** - Forces monitor refresh rate (useful if TF2 picks the wrong one).
- **-dxlevel <version>** - Forces DirectX level (81, 90, 95, 98).
  - ⚠️ Only use once — remove after the first launch or it resets your settings each time.
- **-softparticlesdefaultoff** - Disables soft particles by default (saves GPU).

### ⌨️ Input / Controller

- **-nojoy** - Disables joystick support (slightly faster load).
- **-nosteamcontroller** - Disables Steam Input controller system.
- **-useforcedmparms -noforcemaccel -noforcemspd** - Forces Windows mouse acceleration settings off. (Only matters if you haven't already set raw input with m_rawinput 1.)

### 📦 Performance / Memory

- **-reuse** - Reuses render context between map loads (can shorten load times).
- **-high** - Forces TF2 to run in high CPU priority. ⚠️ Can cause instability if your PC is multitasking.
- **-threads <num>** - Forces number of processor threads. ⚠️ Generally not recommended — let Source handle it.
- **-nocrashdialog** - Suppresses Windows error popups (closes TF2 directly on crash).
- **-noasync** - Disables async sound loading (can reduce stutter at cost of longer load times).
- **-limitvsconst** - Forces a limited number of vertex shader constants (old GPUs only).
- **-particles <num>** - Controls particle detail (1 = lowest).

### 🌐 Network

- **-tcp** - Forces Steam to use TCP instead of UDP. ⚠️ Usually slower, only for troubleshooting connection issues.

### 🧪 Debug / Misc

- **-console** - Opens developer console on startup.
- **-autoconfig** - Resets video/audio settings to default based on hardware (one-time use).
- **-safe** - Starts TF2 in safe mode with minimal video settings.
- **-nobreakpad** - Disables Valve's crash reporting tool.
- **-nocrashdialog** - Suppresses Windows crash dialogs.
- **-condebug** - Writes console output to console.log in your TF2 folder. Useful for debugging configs.

### 💡 Recommended “Max FPS” Set

For competitive / maximum performance TF2:

```
-fullscreen -high -novid -nojoy -nosteamcontroller -reuse -softparticlesdefaultoff -particles 1 -console
```

This setup:

- Forces exclusive fullscreen
- Gives TF2 highest CPU priority
- Strips unnecessary subsystems
- Reduces particle load
- Starts with console open
