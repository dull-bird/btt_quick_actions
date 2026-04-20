# BetterTouchTool QuickActions Preset Guide

*[中文版本](README_CN.md)*

This document introduces the shortcut gestures and keyboard shortcut logic included in the current [BetterTouchTool (BTT)](https://folivora.ai/) preset. You can quickly get started by following these gesture instructions, or share it with others as a user reference.

## 🚀 Quick Start

1. Download the `QuickActions.bttpreset` file.
2. Open **BetterTouchTool**.
3. Go to **Manage Presets** (top right corner).
4. Click **Import** and select the downloaded file.
5. Make sure the preset is enabled and "Global" is selected.

---

## 🌐 Global Gestures

Global gestures are applicable to almost all daily applications and usage scenarios. For memory and feedback convenience, some gestures will display an exclusive Emoji Head-Up Display (HUD) on the screen when triggered.

### 🤟 3-Finger Gestures
Mainly used for **window management** and **tab switching**.

| Action | Execution (Shortcut) | HUD |
| :--- | :--- | :--- |
| **Swipe Down** | `Command + W` (Close current window/tab) | None |
| **Swipe Up** | `Command + Tab` (Switch applications) | None |
| **Swipe Left** | `Ctrl + Tab` (Next tab) | None |
| **Swipe Right** | `Ctrl + Shift + Tab` (Previous tab) | None |
| **Click** | Maximize window to **Next Display** | ✈️ |
| **Double Tap** | `Ctrl + Cmd + D` (Look up dictionary at cursor) | None |

**Advanced 3-Finger Gestures with Modifiers**:
> [!TIP]
> **Design Logic**: The modifier keys are intuitively mapped to the macOS window control buttons:
> - `Fn` ⟷ 🔴 (Close)
> - `Control (⌃)` ⟷ 🟡 (Minimize)
> - `Option (⌥)` ⟷ 🟢 (Fullscreen)

* 🔴 Hold `Fn` + **Swipe Down**: Close the window hovered under cursor
* 🟡 Hold `Control (⌃)` + **Swipe Up**: Open Mission Control
* 🟡 Hold `Control (⌃)` + **Swipe Down**: Minimize the window hovered under cursor
* 🟢 Hold `Option (⌥)` + **Swipe Up**: Enter app fullscreen mode (if supported)

### 🖖 4-Finger Gestures
Mainly used for **app-level control** and **system tools**.

> [!CAUTION]
> **Safety Warning**: 4-finger **Swipe Down** is mapped to `Command + Q` (Quit Application). Use it with caution as it can be easily triggered by accident. You can manually disable this gesture in BTT if you find it too risky.

| Action | Execution (Shortcut) | HUD |
| :--- | :--- | :--- |
| **Swipe Down** | `Command + Q` (Quit current application) | 🥥 |
| **Double Tap** | Open macOS native screenshot/recording tool (Mojave+)| None |


### 👆 1-Finger Gestures
* Hold `Option (⌥)` + **Tap bottom center**: Trigger `Command + M` (Minimize current window)

---

## ⌨️ Global Shortcuts

The preset integrates some in-depth keyboard shortcut configurations (using specific modifier key combinations). Since keyboard configurations can be complex, here is the **core capability panel** they provide:

* **📏 Window Splitting & Positioning**: Includes "Maximize window left/right" to quickly split workspaces.
* **↔️ Cross-Display**: Use shortcuts to instantly "Maximize to Next Display".
* **🎯 Elastic Window Resizing**: Custom resize actions that **automatically center** the window afterwards.
* **✖️ Efficient Closing**: Directly "Close window under cursor" (works even in Mission Control).
* **💡 Screen Control**: Shortcuts for Brightness Up and Down.

---

## 🖱️ Mouse Support

Some configurations cater to users with external regular mice:
* **Side Button (Button 4)**: Directly **Maximize** the current window.
* **Middle Button (Button 3)**: Directly **Minimize** the hovered window under cursor.

---

## 📦 App-Specific Settings

The preset provides dedicated adaptations for specific applications:

### 1. Safari Browser
* Bound **horizontal scrolling** to simulate `Ctrl + Tab` and `Ctrl + Shift + Tab` for quick tab switching.
* *(Note: This feature is temporarily set to "Disabled" in the current preset; you can manually un-disable it in BTT if needed.)*

### 2. PDF Expert (PDF Reader)
* Enhanced backward/forward navigation logic:
  * Pressing `[` triggers `Command + [`
  * Pressing `]` triggers `Command + ]`
  * Benefit: Simplifies shortcuts so you only need to press bracket keys for back/forward navigation.

---

## 🛠️ Recommended System Settings

To ensure the best experience and avoid conflicts with macOS native gestures, we recommend following these settings in **System Settings > Trackpad** (as shown in the screenshots below):

![Settings Part 1](assets/mac_trackpad_settings_1.png)
![Settings Part 2](assets/mac_trackpad_settings_2.png)
![Settings Part 3](assets/mac_trackpad_settings_3.png)

---

## ⚙️ General Settings & Tuning

The preset includes in-depth system-level tuning (BTTGeneralSettings), which not only improves gesture trigger success rates but also optimizes the native macOS experience:

* **🧲 Advanced Window Snapping**:
  * **Omni-directional Snapping**: Enabled quick snapping/expansion for top, bottom, and four corners of the screen.
  * **Visuals & Experience**: Smooth preview animations, custom highlight colors, rounded borders, and enhanced drag sensitivity.
  * **Memory Optimization**: Enabled Memory Saver for snap areas and edge gap adjustments for Stage Manager.

* **🖐️ Trackpad & Force Touch Tuning**:
  * **Pressure Control**: Precise force thresholds distinguishing "Normal Click" and "Force Click" (higher force required to prevent accidental triggers), paired with detailed Haptic feedback.
  * **Palm Rejection**: Enabled Palm Recognition and allowed thumbs resting on edges to avoid finger conflicts in complex gestures.
  * **Sensitivity Tweaks**: Custom swipe sensitivities for 3 & 4 fingers, and precise tweaks for double-tap delays.

* **💻 Notch & Touch Bar Adaptations**:
  * Configured status bar icon hiding/showing logic for Macs with Notch or Touch Bar.
  * Supports filtering Magic Mouse edge accidental touches for heavy mouse users.
