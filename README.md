**Start with Windows**  
Allows starting RivaTuner Statistics Server with Windows. Enable this option only when using RivaTuner Statistics Server as a standalone framerate monitoring solution. If you are using this application in conjunction with clients such as RivaTuner, HIS iTurbo, EVGA Precision, or MSI Afterburner, the clients will load the server when necessary.  
*Hints:*  
- You may disable user interface tooltips via the *User Interface* tab in advanced properties.

---

**Show On-Screen Display**  
Globally controls On-Screen Display visibility. Use this option to hide the On-Screen Display without changing the profiles. Client applications can also remotely control this option via hotkeys.  
*Hints:*  
- You may disable user interface tooltips via the *User Interface* tab in advanced properties.

---

**Application Detection Level: None**  
Disables detection for the application associated with the current profile. In this mode, RivaTuner Statistics Server does not collect runtime statistics, such as framerate, and does not provide additional services, such as On-Screen Display, to the associated application.  
*Hints:*  
- Some protected applications may treat executable code hooking, required for proper application detection, statistics collection, and On-Screen Display rendering, as a possible threat and refuse to run. To troubleshoot such issues, try adding a profile for such an application and decrease the application detection level.  
- You may disable user interface tooltips via the *User Interface* tab in advanced properties.

---

**Application Detection Level: Low**  
Selects a low detection level for the application associated with the current profile. In this mode, RivaTuner Statistics Server intercepts the application's calls to Direct3D and OpenGL runtime libraries. This mode is recommended for collecting runtime statistics, such as framerate, and enabling additional services, such as On-Screen Display, in the majority of modern 3D applications.  
*Hints:*  
- Some protected applications may treat executable code hooking, required for proper application detection, statistics collection, and On-Screen Display rendering, as a possible threat and refuse to run. To troubleshoot such issues, try adding a profile for such an application and decrease the application detection level.  
- You may disable user interface tooltips via the *User Interface* tab in advanced properties.

---

**Application Detection Level: Medium**  
Selects a medium detection level for the application associated with the current profile. In this mode, RivaTuner Statistics Server intercepts the application's calls to DirectDraw, Direct3D, and OpenGL runtime libraries. This mode is recommended for collecting runtime statistics, such as framerate, and enabling additional services, such as On-Screen Display, in the majority of modern 3D applications as well as in applications using outdated 2D/3D hardware acceleration interfaces like DirectDraw and Direct3D7.  
*Hints:*  
- Some protected applications may treat executable code hooking, required for proper application detection, statistics collection, and On-Screen Display rendering, as a possible threat and refuse to run. To troubleshoot such issues, try adding a profile for such an application and decrease the application detection level.  
- You may disable user interface tooltips via the *User Interface* tab in advanced properties.

---

**Application Detection Level: High**  
Selects a high detection level for the application associated with the current profile. In this mode, RivaTuner Statistics Server intercepts the application's calls to DirectDraw, Direct3D, and OpenGL runtime libraries and intercepts the application's attempts to load new libraries. This mode is recommended for collecting runtime statistics, such as framerate, and enabling additional services, such as On-Screen Display, in applications that load DirectDraw, Direct3D, and OpenGL runtime libraries dynamically.  
*Hints:*  
- Some protected applications may treat executable code hooking, required for proper application detection, statistics collection, and On-Screen Display rendering, as a possible threat and refuse to run. To troubleshoot such issues, try adding a profile for such an application and decrease the application detection level.  
- You may disable user interface tooltips via the *User Interface* tab in advanced properties.

---

**Stealth Mode**  
Anti-cheat systems of some games may treat game code hooking, required for application detection and On-Screen Display rendering, as a possible cheat and block connection to multiplayer servers. Enabling stealth mode may help resolve such issues. When this mode is enabled, RivaTuner Statistics Server uses sophisticated code hooking techniques, making it harder for third-party applications to detect the hook.  
*Hints:*  
- You may disable user interface tooltips via the *User Interface* tab in advanced properties.

---

**Custom Direct3D Support: Enable Compatibility with Modified Direct3D Runtime Libraries**  
By default, RivaTuner Statistics Server supports Direct3D applications using native Microsoft Direct3D runtime libraries only. You may enable this option to make it compatible with Direct3D applications using custom modified runtime Direct3D proxy libraries (e.g., InjectFXAA-enabled Direct3D applications). This option is profile-specific, so you can configure it independently for different applications. It is not recommended to enable it globally, as the compatibility mode can prevent some Direct3D applications from starting.  
*Hints:*  
- You may disable user interface tooltips via the *User Interface* tab in advanced properties.

---

**Framerate Limit**  
Allows switching between framerate and frametime limit modes. In frametime mode, the limit is specified as the target frametime with 1-microsecond precision.  
*Hints:*  
- You may disable user interface tooltips via the *User Interface* tab in advanced properties.

---

**Scanline Sync Mode**  
Allows switching between single, double, and half scanline synchronization modes. In single scanline synchronization mode, the framerate is synchronized to the rasterizer position per each display refresh period. In other words, you're limiting the framerate to the refresh rate and achieving a VSync ON effect with a tearline located in a fixed position. The tearline can be moved down and hidden in the vertical blanking interval. In double scanline synchronization mode, the framerate is synchronized to the rasterizer position twice per display refresh period. In other words, you're limiting the framerate to double the refresh rate and achieving a VSync ON effect with two tearlines located in fixed positions. Both tearlines can be moved down, and one of them can be hidden in the vertical blanking interval. In half scanline synchronization mode, the framerate is synchronized to the rasterizer position once per two display refresh periods. In other words, you're limiting the framerate to half the refresh rate and achieving a VSync ON effect with a tearline located in a fixed position. In this case, the tearline can be moved down and hidden in the vertical blanking interval.  
*Hints:*  
- It is necessary to disable VSync for proper scanline synchronization functionality.  
- You may enable scanline sync in conjunction with front/back edge sync framerate limiting modes to activate hybrid scanline sync modes. In this case, the actual target scanline synchronization is performed just once on framerate limiting start, and then you can steer the tearline positioning with the system clock.  
- You may use the FCAT overlay in moving bar mode as a visual tearline position indicator.  
- You may specify a negative scanline index to set the offset from the total number of scanlines.  
- You may disable user interface tooltips via the *User Interface* tab in advanced properties.

---

**Enable On-Screen Display Support**  
Enables On-Screen Display support for the application associated with the current profile.  
*Hints:*  
- Anti-cheat systems of some games may treat game code hooking, required for application detection and On-Screen Display rendering, as a possible cheat and block connection to multiplayer servers. To troubleshoot such issues, try adding a profile for such a game and disable On-Screen Display support, or if that doesn't help, try decreasing the application detection level.  
- You may disable user interface tooltips via the *User Interface* tab in advanced properties.

---

**On-Screen Display: Vector 2D Rendering Mode**  
On-Screen Display can be rendered using either vector or raster fonts via hardware-accelerated 2D or hardware-accelerated 3D DirectX/OpenGL functions. The 2D acceleration-based implementation provides maximum compatibility with most existing game 3D engines; however, it is not supported in DirectX 10 and newer games when multisampled antialiasing is enabled. 2D acceleration can also be poorly optimized in some display drivers, so the 3D acceleration-based implementation can be much more effective in terms of performance on such systems. However, the 3D implementation has a higher chance of being incompatible with some game 3D engines. Try disabling 3D mode if you notice any rendering anomalies in a game while running it with OSD enabled.  
*Hints:*  
- Anti-cheat systems of some games may treat game code hooking, required for application detection and On-Screen Display rendering, as a possible cheat and block connection to multiplayer servers. To troubleshoot such issues, try adding a profile for such a game and disable On-Screen Display support, or if that doesn't help, try decreasing the application detection level.  
- You may disable user interface tooltips via the *User Interface* tab in advanced properties.

---

**On-Screen Display: Vector 3D Rendering Mode**  
On-Screen Display can be rendered using either vector or raster fonts via hardware-accelerated 2D or hardware-accelerated 3D DirectX/OpenGL functions. The 2D acceleration-based implementation provides maximum compatibility with most existing game 3D engines; however, it is not supported in DirectX 10 and newer games when multisampled antialiasing is enabled. 2D acceleration can also be poorly optimized in some display drivers, so the 3D acceleration-based implementation can be much more effective in terms of performance on such systems. However, the 3D implementation has a higher chance of being incompatible with some game 3D engines. Try disabling 3D mode if you notice any rendering anomalies in a game while running it with OSD enabled.  
*Hints:*  
- Anti-cheat systems of some games may treat game code hooking, required for application detection and On-Screen Display rendering, as a possible cheat and block connection to multiplayer servers. To troubleshoot such issues, try adding a profile for such a game and disable On-Screen Display support, or if that doesn't help, try decreasing the application detection level.  
- You may disable user interface tooltips via the *User Interface* tab in advanced properties.

---

**On-Screen Display: Raster 3D Rendering Mode**  
On-Screen Display can be rendered using either vector or raster fonts via hardware-accelerated 2D or hardware-accelerated 3D DirectX/OpenGL functions. The 2D acceleration-based implementation provides maximum compatibility with most existing game 3D engines; however, it is not supported in DirectX 10 and newer games when multisampled antialiasing is enabled. 2D acceleration can also be poorly optimized in some display drivers, so the 3D acceleration-based implementation can be much more effective in terms of performance on such systems. However, the 3D implementation has a higher chance of being incompatible with some game 3D engines. Try disabling 3D mode if you notice any rendering anomalies in a game while running it with OSD enabled. You may click the selected raster 3D rendering mode button again to change the font type and style, or hold *Ctrl* and click it again to load a pre-rendered raster font from a bitmap file.  
*Hints:*  
- Anti-cheat systems of some games may treat game code hooking, required for application detection and On-Screen Display rendering, as a possible cheat and block connection to multiplayer servers. To troubleshoot such issues, try adding a profile for such a game and disable On-Screen Display support, or if that doesn't help, try decreasing the application detection level.  
- You may disable user interface tooltips via the *User Interface* tab in advanced properties.

---

**On-Screen Display Coordinate Space: Viewport**  
By default, On-Screen Display coordinate space matches the coordinate space of the rendering viewport, i.e., the last rectangular area the application was rendering to. However, certain applications (e.g., StarCraft II: Wings of Liberty) can use multiple viewports during frame rendering (e.g., different viewports for the 3D world and HUD). In this case, the On-Screen Display origin follows one of the corners of the last viewport defined during frame rendering, which may be located in an undesired position. On-Screen Display coordinate space override-related options can be used to restore the expected origin position in such applications. This button selects the rendering viewport as the coordinate space for On-Screen Display.  
*Hints:*  
- Anti-cheat systems of some games may treat game code hooking, required for application detection and On-Screen Display rendering, as a possible cheat and block connection to multiplayer servers. To troubleshoot such issues, try adding a profile for such a game and disable On-Screen Display support, or if that doesn't help, try decreasing the application detection level.  
- You may disable user interface tooltips via the *User Interface* tab in advanced properties.

---

**On-Screen Display Coordinate Space: Framebuffer**  
By default, On-Screen Display coordinate space matches the coordinate space of the rendering viewport, i.e., the last rectangular area the application was rendering to. However, certain applications (e.g., StarCraft II: Wings of Liberty) can use multiple viewports during frame rendering (e.g., different viewports for the 3D world and HUD). In this case, the On-Screen Display origin follows one of the corners of the last viewport defined during frame rendering, which may be located in an undesired position. On-Screen Display coordinate space override-related options can be used to restore the expected origin position in such applications. This button selects the entire framebuffer as the coordinate space for On-Screen Display.  
*Hints:*  
- Anti-cheat systems of some games may treat game code hooking, required for application detection and On-Screen Display rendering, as a possible cheat and block connection to multiplayer servers. To troubleshoot such issues, try adding a profile for such a game and disable On-Screen Display support, or if that doesn't help, try decreasing the application detection level.  
- You may disable user interface tooltips via the *User Interface* tab in advanced properties.

---

**Enable On-Screen Display Shadow**  
Enables On-Screen Display shadow rendering. Shadow rendering can improve On-Screen Display readability in some applications by preventing the text from merging with solid screen colors. Please note that shadow rendering increases the performance hit caused by On-Screen Display rendering in vector modes, so enable it only when necessary.  
*Hints:*  
- Anti-cheat systems of some games may treat game code hooking, required for application detection and On-Screen Display rendering, as a possible cheat and block connection to multiplayer servers. To troubleshoot such issues, try adding a profile for such a game and disable On-Screen Display support, or if that doesn't help, try decreasing the application detection level.  
- You may disable user interface tooltips via the *User Interface* tab in advanced properties.

---

**Enable On-Screen Display Fill**  
Enables filling the underlying On-Screen Display area with a solid or transparent color. Fill color and transparency level can be adjusted in the On-Screen Display palette. Filling the underlying area can improve On-Screen Display readability in some applications by preventing the text from merging with solid screen colors.  
*Hints:*  
- Anti-cheat systems of some games may treat game code hooking, required for application detection and On-Screen Display rendering, as a possible cheat and block connection to multiplayer servers. To troubleshoot such issues, try adding a profile for such a game and disable On-Screen Display support, or if that doesn't help, try decreasing the application detection level.  
- You may disable user interface tooltips via the *User Interface* tab in advanced properties.

---

**On-Screen Display Palette: Base Color**  
Displays the base color for On-Screen Display and allows you to redefine it. You can also adjust the base color transparency level for vector 3D and raster 3D On-Screen Display rendering modes.  
*Hints:*  
- Anti-cheat systems of some games may treat game code hooking, required for application detection and On-Screen Display rendering, as a possible cheat and block connection to multiplayer servers. To troubleshoot such issues, try adding a profile for such a game and disable On-Screen Display support, or if that doesn't help, try decreasing the application detection level.  
- You may disable user interface tooltips via the *User Interface* tab in advanced properties.

---

**On-Screen Display Palette: Shadow Color**  
Displays the shadow color for On-Screen Display and allows you to redefine it for vector On-Screen Display rendering modes. You can also adjust the shadow color transparency level for vector 3D On-Screen Display rendering mode. Please note that shadow rendering increases the performance hit caused by On-Screen Display rendering in vector modes, so enable it only when necessary.  
*Hints:*  
- Anti-cheat systems of some games may treat game code hooking, required for application detection and On-Screen Display rendering, as a possible cheat and block connection to multiplayer servers. To troubleshoot such issues, try adding a profile for such a game and disable On-Screen Display support, or if that doesn't help, try decreasing the application detection level.  
- You may disable user interface tooltips via the *User Interface* tab in advanced properties.

---

**On-Screen Display Palette: Fill Color**  
Displays the fill color for On-Screen Display and allows you to redefine it. You can also adjust the fill color transparency level for vector 3D and raster 3D On-Screen Display rendering modes.  
*Hints:*  
- Anti-cheat systems of some games may treat game code hooking, required for application detection and On-Screen Display rendering, as a possible cheat and block connection to multiplayer servers. To troubleshoot such issues, try adding a profile for such a game and disable On-Screen Display support, or if that doesn't help, try decreasing the application detection level.  
- You may disable user interface tooltips via the *User Interface* tab in advanced properties.

---

**On-Screen Display Zoom**  
Adjusts the On-Screen Display zoom ratio. Use the On-Screen Display preview window for visual control of On-Screen Display appearance when zooming.  
*Hints:*  
- Anti-cheat systems of some games may treat game code hooking, required for application detection and On-Screen Display rendering, as a possible cheat and block connection to multiplayer servers. To troubleshoot such issues, try adding a profile for such a game and disable On-Screen Display support, or if that doesn't help, try decreasing the application detection level.  
- You may disable user interface tooltips via the *User Interface* tab in advanced properties.

---

**Show Own Statistics**  
The primary purpose of RivaTuner Statistics Server is to collect framerate statistics for all 3D applications running in the system and provide this data to client applications, such as RivaTuner, HIS iTurbo, EVGA Precision, or MSI Afterburner. It also provides additional services, such as On-Screen Display, screen capture support, or 3D detection, to the clients. However, you can also use RivaTuner Statistics Server as a standalone framerate monitoring solution. Enable this option to allow RivaTuner Statistics Server to show its own framerate statistics in the On-Screen Display without running any additional client applications. When client applications are using RivaTuner Statistics Server's video capture engine, this option also controls the display of additional video capture-related statistics. Enable it to display video file time, size, per-frame compression ratio, and compression time statistics next to the video capture indicator.  
*Hints:*  
- Anti-cheat systems of some games may treat game code hooking, required for application detection and On-Screen Display rendering, as a possible cheat and block connection to multiplayer servers. To troubleshoot such issues, try adding a profile for such a game and disable On-Screen Display support, or if that doesn't help, try decreasing the application detection level.  
- You may disable user interface tooltips via the *User Interface* tab in advanced properties.

---

**On-Screen Display Preview**  
Displays the On-Screen Display preview. Please note that the preview size and position are accurate only for display modes matching your current display mode and are relative to the origin corner.  
*Hints:*  
- You may detach and set a custom position and size for the preview window by double-clicking the preview window area. This may simplify the process of visually adjusting the On-Screen Display position.  
- You may right-click this window and select the *Capture Screenshot* command from the context menu to capture a screenshot from the currently running 3D application and use it as the background image for this window. This may simplify the process of visually adjusting the On-Screen Display position. The default background can be selected with the *Clear* command from the context menu.  
- Anti-cheat systems of some games may treat game code hooking, required for application detection and On-Screen Display rendering, as a possible cheat and block connection to multiplayer servers. To troubleshoot such issues, try adding a profile for such a game and disable On-Screen Display support, or if that doesn't help, try decreasing the application detection level.  
- You may disable user interface tooltips via the *User Interface* tab in advanced properties.
