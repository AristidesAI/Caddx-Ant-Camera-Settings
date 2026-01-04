# Caddx FPV Ant Camera - Menu Settings & Configuration

Complete menu structure and recommended settings for the Caddx FPV Ant analog FPV camera. The goal of this post is to align the camera settings for the CADDX Ant Analog FPV micro camera, Suitable for tiny whoops and lightweight analog FPV builds. This camera comes with an OSD adjustment board that can be connected directly to the camera to enable this settings menu.

![Camera OSD Board](https://m.media-amazon.com/images/I/51GrZW6DVXL._AC_SL1500_.jpg)

## Main Menu

```
MAIN
├── AE
├── AWB
├── DAY/NIGHT
├── IMAGE ENHANCE
├── VIDEO SETTING
├── LANGUAGE
├── RESET
├── SAVE&EXIT
└── EXIT
```


## Exposure Settings

### Menu Path: `MAIN` → `AE`

| Setting | Default | Recommended | Description |
|---------|---------|-------------|-------------|
| **BRIGHTNESS** | `<14>` | `<15>` | Controls overall image brightness.  Increase for darker environments, decrease for brighter conditions. |
| **EXPOSURE MODE** | `<BLC>` | `<BLC>` | Back Light Compensation mode. Handles scenes with bright backlighting by brightening foreground subject. |
| **BLC** | `<4>` | `<6>` | Back Light Compensation intensity level (0-maximum compensation). Higher values provide stronger backlight correction. |

### Navigation
- From **MAIN** menu, select **AE**
- Adjust values as needed
- Select **RETURN** to go back to main menu


## Auto White Balance (AWB)

### Menu Path: `MAIN` → `AWB`

| Setting | Default | Recommended | Description |
|---------|---------|-------------|-------------|
| **MODE** | `<ATW>` | `<ATW>` | Auto Tracking White Balance.  Camera automatically adjusts color temperature to match lighting environment. ATW = intelligent auto mode. |

### Use Cases for AWB Mode
- **ATW (Auto Tracking)**: Best for mixed lighting, outdoor flying, or environments where lighting changes frequently
- Manual presets available for consistent indoor environments with stable lighting

### Navigation
- From **MAIN** menu, select **AWB**
- Confirm mode setting
- Select **RETURN** to go back to main menu


## Day/Night Mode

### Menu Path: `MAIN` → `DAY/NIGHT`

| Setting | Default | Recommended | Description |
|---------|---------|-------------|-------------|
| **MODE** | `<AUTO>` | `<AUTO>` | Automatically switches between color and black & white modes based on ambient light levels.  Enables ultra-low light scenarios.  |

### Mode Options & Behavior

| Mode | Behavior | Best For |
|------|----------|----------|
| **COLOR** | Fixed color mode | Daytime and bright environments only |
| **B&W** | Fixed black & white mode | Night flying and ultra-low light |
| **AUTO** | Intelligently switches between COLOR and B&W based on light intensity | Mixed environments, day-to-night transitions, all-around versatility |

### Important Notes
- **AUTO mode recommended** for maximum versatility and automatic adaptation
- AUTO mode will switch to black & white as light decreases, then back to color as light increases
- This setting enables ultra-low light performance when combined with proper exposure settings

### Navigation
- From **MAIN** menu, select **DAY/NIGHT**
- Select **MODE** to change setting
- Select **RETURN** to go back to main menu


## Image Enhancement Settings

### Menu Path: `MAIN` → `IMAGE ENHANCE`

| Setting | Default | Value | Recommended | Description |
|---------|---------|-------|-------------|-------------|
| **CONTRAST** | `<AUTO>` | — | `<AUTO>` | Automatic contrast adjustment. Enhances the difference between light and dark areas. |
| **SHARPNESS** | `<MANUAL>` | `<AUTO>` | `<MANUAL>` `<20>` | Edge definition and clarity.  MANUAL mode allows custom value adjustment. Higher values = sharper image but may introduce noise. |
| **SATURATE** | `<AUTO>` | — | `<AUTO>` | Automatic color saturation.  Adjusts color intensity to match scene conditions. |
| **3DNR** | `<AUTO>` | — | `<AUTO>` | 3D Digital Noise Reduction (temporal). AUTO mode adapts to light levels.  Reduces grain across multiple frames. |
| **2DNR** | `<MANUAL>` | `<AUTO>` | `<MANUAL>` `<5>` | 2D Digital Noise Reduction (spatial). MANUAL mode allows custom value.  Value `<5>` balances noise reduction with detail retention. |

### Sharpness Detailed Guide

**Setting**: `SHARPNESS <MANUAL> <20>`

| Value Range | Use Case | Lighting Condition |
|---|---|---|
| **0-5** | Soft, cinematic | Low light, night flying |
| **10-15** | Balanced | Mixed/indoor lighting |
| **18-25** | High definition | Bright outdoor, daytime racing |

- **Lower values**:  Reduces digital artifacts and sharpening noise, better for low-light
- **Higher values**: Improves detail clarity and edge definition, better for bright conditions

### 2DNR (2D Noise Reduction) Detailed Guide

**Setting**: `2DNR <MANUAL> <5>`

| Value | Intensity | Best For |
|---|---|---|
| **0-2** | Minimal | Bright daylight, detail preservation |
| **3-6** | Moderate (Recommended:  5) | General purpose, balanced |
| **7-10** | Aggressive | Night flying, low-light scenarios |

- **Lower values**: More detail, grainier in low light
- **Higher values**:  Smoother image, less detail, better in darkness

### Navigation
- From **MAIN** menu, select **IMAGE ENHANCE**
- Navigate through each setting with arrows
- To edit value:  select setting and adjust number
- Confirm changes
- Select **RETURN** to go back to main menu


## Video Settings

### Menu Path: `MAIN` → `VIDEO SETTING`

| Setting | Default | Recommended | Description |
|---------|---------|-------------|-------------|
| **HD** | `<CVBS>` | `<CVBS>` | Video output format. CVBS = Composite Video Baseband Signal (standard analog FPV video). |
| **STANDARD** | `<NTSC>` | `<PAL>` | Video standard format. PAL = 576 lines, larger pixel count for more detail.  NTSC = 480 lines.  Choose based on region and larger pixel count preference. |

### Video Standard Comparison

| Standard | Resolution | Refresh Rate | Region | Pixel Count |
|----------|-----------|--------------|--------|------------|
| **PAL** | 576 lines | 50Hz | Europe, Australia, most other regions | **Higher** (more detail) |
| **NTSC** | 480 lines | 60Hz | North America, Japan, some others | Lower |

### Recommendation
- **PAL** selected for larger pixel count and more detail in video feed
- Choose based on your geographic region and FPV transmitter compatibility
- Verify your VTx (video transmitter) supports your chosen standard

### Navigation
- From **MAIN** menu, select **VIDEO SETTING**
- Navigate to **STANDARD**
- Change to **PAL** for maximum pixel count and detail
- Select **RETURN** to go back to main menu


## Quick Reference:  Complete Settings Summary

### Current Recommended Configuration

```
EXPOSURE (AE)
├── BRIGHTNESS: 15 ✓
├── EXPOSURE MODE: BLC
└── BLC: 6 ✓

AUTO WHITE BALANCE (AWB)
└── MODE: ATW ✓

DAY/NIGHT
└── MODE: AUTO ✓

IMAGE ENHANCE
├── CONTRAST: AUTO ✓
├── SHARPNESS: MANUAL <20> ✓
├── SATURATE: AUTO ✓
├── 3DNR: AUTO ✓
└── 2DNR: MANUAL <5> ✓

VIDEO SETTINGS
├── HD: CVBS ✓
└── STANDARD: PAL ✓
```


## Saving Your Settings

### To Save Configuration: 

1. Navigate to **MAIN** menu
2. Select **SAVE&EXIT**
3. Settings are now permanently saved to camera memory
4. Camera will apply these settings on next power cycle

### To Exit Without Saving:

1. Navigate to **MAIN** menu
2. Select **EXIT** (without saving)
3. Changes will be lost


## Reset to Factory Defaults

### To Reset All Settings: 

1. Navigate to **MAIN** menu
2. Select **RESET**
3. Confirm reset (typically requires additional confirmation)
4. Camera will return to factory default settings
5. You will need to reconfigure all settings

> ⚠️ **WARNING**:  Resetting will erase all your custom configurations.  Only use if experiencing persistent issues.

---

## Troubleshooting

| Problem | Solution |
|---------|----------|
| Image too bright/washed out | Decrease BRIGHTNESS, or change BLC mode |
| Image too dark | Increase BRIGHTNESS, enable AUTO mode in DAY/NIGHT |
| Colors look wrong | Verify AWB MODE is set to ATW, allow 5-10 seconds for auto-adjustment |
| Image looks grainy | Increase 2DNR value (from 5 to 7-8), reduce SHARPNESS if in low light |
| Image looks blurry | Increase SHARPNESS value (from 20 to 22-25), reduce 2DNR if too much smoothing |
| No signal to VTx | Verify VIDEO STANDARD (PAL/NTSC) matches your transmitter and region |
| Poor night flying performance | Set DAY/NIGHT to AUTO, increase BRIGHTNESS, increase 2DNR to 8-10 |

---

## Best Practices

### ✅ Do's
- ✅ Save settings after each configuration session
- ✅ Test one setting change at a time
- ✅ Allow 10+ seconds for AUTO modes to adjust to new lighting
- ✅ Verify transmitter compatibility with your video STANDARD choice
- ✅ Document your optimal settings for different flying locations

### ❌ Don'ts
- ❌ Don't reset without saving your current configuration first
- ❌ Don't change multiple settings simultaneously (hard to identify which helped)
- ❌ Don't use mismatched video standards between camera and transmitter
- ❌ Don't forget to press SAVE&EXIT after making changes


## Recommended Profiles by Use Case

### 🏁 Outdoor Racing (Bright Daylight)
```
BRIGHTNESS: 14-15
BLC: 4-5
SHARPNESS: 22-25
2DNR: 2-3
STANDARD: PAL
DAY/NIGHT: AUTO
```

### 🎬 Freestyle (Mixed Lighting)
```
BRIGHTNESS: 15
BLC: 6
SHARPNESS: 20
2DNR: 5
STANDARD: PAL
DAY/NIGHT: AUTO
```

### 🌙 Night Flying (Low Light)
```
BRIGHTNESS: 16-17
BLC: 6
SHARPNESS: 15-18
2DNR: 8-10
STANDARD: PAL
DAY/NIGHT: AUTO
```

### 🏠 Indoor (Artificial Lighting)
```
BRIGHTNESS: 15
BLC: 4
SHARPNESS: 20-22
2DNR: 4-5
STANDARD: PAL
DAY/NIGHT:  AUTO
```



## Related Documentation

- [Camera Website](https://www.caddxfpv.com/products/caddx-ant-analog-camera)
- [Ant Tune from another guide](https://www.ericbrasseur.org/caddxfpv_ant_tuning.html?i=1)
- [Further Camera Guidance](https://oscarliang.com/fpv-camera-settings/)



**Last Updated**:  January 4, 2026  
**Camera Model**:  Caddx FPV Ant  
**Document Version**: 1.0



Thanks for reading! If you found this useful, Follow me on Instagram [@Aristides.FPV](https://www.instagram.com/aristides.fpv/)
