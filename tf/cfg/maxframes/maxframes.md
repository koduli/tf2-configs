## About this config

This config is already max-FPS optimized. If you want to use this config but adjust it for your preferences, here are the main settings you can tweak:

```
fps_max
```

300 (current setting) = good balance<br>
0 = uncapped (can be unstable, but gives max raw FPS)<br>
If you notice stutters, try capping to something your PC can hold (144 / 240).<br>

```
mat_queue_mode
```

2 (current setting) = multithreaded, best for modern CPUs<br>
If you ever crash or see glitches, try -1 (auto-detect).<br>

```
mat_picmip
```

2 (current setting) = ugliest but fastest<br>
If you want slightly nicer textures with only a tiny performance cost, try 1.<br>

## Recommended launch options with this config

```
-fullscreen -high -novid -nojoy -nosteamcontroller -reuse -softparticlesdefaultoff -particles 1 -console
```

- Forces exclusive fullscreen
- Gives TF2 highest CPU priority
- Strips unnecessary subsystems
- Reduces particle load
- Starts with console open
