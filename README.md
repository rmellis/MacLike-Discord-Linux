# MacLike Discord Theme

![Version](https://img.shields.io/badge/version-1.1.2-blue)   ![Discord_Client](https://img.shields.io/badge/Supports-BetterDiscord%20|%20Vencord-7289DA)   [![Discord](https://img.shields.io/badge/Discord-WAM_Project-5865F2?style=flat&logo=discord&logoColor=white)](https://discord.gg/MyxaEQxjFT)

A clean, minimalist Discord theme aiming to create a more native, macOS-like experience across multiple operating systems.

---

## Preview
![MacLike Theme Preview](https://github.com/user-attachments/assets/1c59aaa7-9922-4dbe-af33-4c5e3134dde2)

## Features

* **Native Window Controls**: macOS-style "traffic light" window controls (close, minimize, maximize) custom-built to override native OS window borders.
* **Translucency**: Incorporates a subtle background blur (mica/acrylic effect) on various UI elements for depth.
* **Mac-style Sidebar**: Replicates a native macOS app look.
* **Rounded Corners**: Consistent use of corner radii across the UI, overriding sharp default backgrounds.
* **Cross-Platform**: Tailored CSS and layout adjustments for Windows, macOS, and Linux to ensure consistent rendering of UI elements like history arrows and window controls.
* **Theme Support**: Support for native Discord color themes (Appearance settings). Full restart required when applying a new theme. I cannot fix this; it is an issue on Discord's end.

---

## Installation

A Discord client mod is required. BetterDiscord or Vencord is recommended.

### BetterDiscord
1.  Download the `MacLike.theme.css` file from the [latest release](https://github.com/syryz/MacLike-Discord/releases/latest).
2.  Open Discord settings.
3.  Navigate to the `Themes` tab in the BetterDiscord section.
4.  Click the `Open Themes Folder` button.
5.  Move the downloaded `MacLike.theme.css` file into the opened folder.
6.  Return to Discord and enable `MacLike` from the theme list.

### Vencord
1.  Download the `MacLike.theme.css` file from the [latest release](https://github.com/syryz/MacLike-Discord/releases/latest)
2.  Open Discord settings.
3.  Navigate to the `Vencord` tab and select the `Themes` sub-tab.
4.  If using QuickCSS, copy and paste the contents of `MacLike.theme.css` to the editor.
5.  Alternatively, follow steps 4-6 above (same as BetterDiscord).

## Customization
- Open the CSS file through QuickCSS or navigating to the themes folder and opening the `MacLike.theme.css` file with a text editor.
- Edit the sidebar background and blur to your liking!
- Turn off the window border if unwanted.

### Enable Translucency/Fix Rounded Corners

**Windows**
1. Install [MicaForEveryone](https://github.com/MicaForEveryone/MicaForEveryone).
2. Add new rule > Add process rule.
3. Enter `Discord`.
4. Set Backdrop Type to `Acrylic` and switch on `Extend frame into client area` and `Enable blur behind`.
5. Set Corner Preference to `Rounded`
6. Go to Discord settings.
7. In the BetterDiscord or Vencord settings page, check `Enable window transparency.`
8. Fully restart Discord.

**macOS**
1. Go to Discord settings > BetterDiscord/Vencord Settings.
2. Make sure `Enable window transparency` is unchecked (off).
3. Under `Window vibrancy style`, select `HUD (Most transparent)`
4. Fully restart Discord.

**Linux**
1. Ensure your desktop environment is running an **X11** session. (Electron natively struggles to render custom window transparency under modern Wayland compositors without complex flags).
2. Go to Discord settings.
3. In the BetterDiscord or Vencord settings page, check `Enable window transparency`.
4. Fully restart Discord.

### Auto-Apply Theme (After Discord Updates)
- Install [BetterVencordPatch](https://github.com/AaronWijesinghe/BetterVencordPatch)

---

## Planned Features
- [ ] **Font Integration**: Replacing the default font with SF Fonts
- [ ] **Animations**: Replicate macOS-style UI animations and transitions (context menu)
- [ ] **Theme Settings Plugin**: Streamline customization options

### Known Issues
- Switching between light and dark themes removes transparency. This is an issue with Discord/Vencord's implementation, so it cannot be fixed on my end.

### Credits
- Huge thanks to [hxntxihero](https://github.com/hxntxihero) for Windows compatibility.
- Linux layout and X11 rendering adjustments contributed by rmellis.
- Part of the WAM project

Created by *syrys*
