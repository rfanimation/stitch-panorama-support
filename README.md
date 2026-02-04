# Stitch — AI-Powered Panoramas & Image Stacking

<p align="center">
  <img src="https://img.shields.io/badge/App_Store-Coming_Soon-blue.svg" alt="App Store">
  <img src="https://img.shields.io/badge/iOS-17.0+-000000.svg?logo=apple" alt="iOS 17+">
  <img src="https://img.shields.io/badge/Price-$4.99-green.svg" alt="Price">
</p>

<p align="center">
  <strong>Professional panorama stitching and image stacking for iPhone and iPad</strong>
</p>

---

## What is Stitch?

Stitch is a professional-grade photo processing app that combines traditional computer vision with cutting-edge AI to create stunning panoramas and stacked images. Whether you're a landscape photographer capturing sweeping vistas, an astrophotographer reducing noise in night shots, or a travel photographer removing crowds from your images, Stitch delivers results that rival desktop software.

**Try before you buy** — Sample images are included so you can test every feature before purchasing.

---

## Panorama Stitching

Transform overlapping photos into seamless panoramas using advanced computer vision and AI.

### Depth-Aware Stitching
Uses AI depth estimation to intelligently place seams in areas where they'll be least visible. The depth model analyzes each image to understand which objects are closer or farther away, then routes seams through background areas rather than cutting through foreground subjects.

**When to use:** Complex scenes with objects at varying distances, architectural shots, landscapes with foreground elements.

### 10 Projection Types
Different projections serve different purposes:

| Projection | Best For | Notes |
|------------|----------|-------|
| **Spherical** | Wide panoramas (>120°) | Default choice, handles most scenarios |
| **Cylindrical** | Horizontal panoramas | Keeps horizon flat, good for cityscapes |
| **Mercator** | Map-style output | Familiar look, vertical stretching at edges |
| **Panini** | Architecture | Keeps verticals straight, natural perspective |
| **Rectilinear** | Narrow panoramas (<90°) | Preserves straight lines, limited FOV |
| **Fisheye** | 360° panoramas | Requires full spherical coverage |
| **Stereographic** | 360° panoramas | Conformal (preserves angles) |
| **Transverse Mercator** | Vertical panoramas | Rotated Mercator projection |
| **Panini Portrait** | Vertical architecture | Panini optimized for portrait orientation |
| **Little Planet** | Creative effect | Creates "tiny planet" from 360° panoramas |

**When to use:** Tap "Projection" after stitching to experiment. The app automatically detects which projections are compatible with your panorama's field of view.

### Gigapixel Support
Automatically handles panoramas over 100 megapixels using a tiled processing approach that keeps memory usage manageable. Feature detection runs at reduced resolution, seam finding at even lower resolution, then final compositing happens tile-by-tile at full resolution.

**When to use:** Enabled automatically when the app detects your output would exceed memory limits. Works transparently in the background.

### Ghost Removal
Uses graph-cut seam finding to route stitching seams around moving objects and parallax artifacts. When objects appear in slightly different positions across overlapping images, this feature finds the optimal cutting path to avoid visible ghosting.

**When to use:** Any scene with movement (swaying trees, walking people in the distance, waves). Enabled by default.

---

## Image Stacking (Beta)

Stack multiple exposures to achieve effects impossible with a single shot.

> **Beta Notice:** Image stacking is a new feature that we are sharing. It has not yet been extensively tested and you may experience unexpected results or crashes, especially with large images or limited device memory.

### Noise Reduction
Combines multiple identical exposures to mathematically reduce random noise. Since noise is random but your subject is constant, averaging multiple frames cancels out the noise while preserving detail.

**When to use:** Low-light photography, astrophotography, any situation where you'd normally increase ISO. Take 5-10 identical shots and stack them for dramatically cleaner results than any single exposure.

**Minimum images:** 5+ recommended

### Crowd Removal
Uses median stacking to remove moving objects from your scene. Take several photos over 30-60 seconds, and anything that moves (people, cars, birds) will be removed, leaving only the static background.

**When to use:** Tourist landmarks, busy streets, any location where you want a "clean plate" without waiting for people to leave.

**Minimum images:** 3+ (more is better)

### Light Trails
Combines exposures using maximum blending to accumulate light trails from moving sources. Each frame's brightest pixels are kept, building up trails from car headlights, stars, or other light sources.

**When to use:** Traffic light trails, star trails, any creative long-exposure effect where you want to accumulate light over time.

**Minimum images:** 10+ recommended

### Long Exposure Simulation
Averages multiple short exposures to simulate a long exposure. Creates silky water effects, motion blur in clouds, and smooth movement without needing an ND filter.

**When to use:** Waterfalls, ocean waves, clouds, any moving element you want to blur. Equivalent to using an ND filter but with more control.

**Minimum images:** 10+ recommended

---

## HDR Processing (Beta)

Merge bracketed exposures into high dynamic range images.

> **Beta Notice:** HDR processing has not yet been extensively tested with all camera types and exposure brackets.

### Merge Methods

**Mertens Fusion** — Exposure fusion that doesn't require exposure time metadata. Works with any bracketed set by analyzing local contrast and saturation. Best for most users.

**Debevec HDR** — True radiometric HDR that reconstructs the actual light values in the scene. Requires accurate EXIF exposure data. Produces a 32-bit floating-point image that can be tone-mapped.

### Tone Mapping

After creating an HDR image, tone mapping compresses the dynamic range for display:

- **Reinhard** — Natural-looking results, good all-around choice
- **Drago** — Logarithmic compression, preserves detail in both highlights and shadows
- **Mantiuk** — Contrast-based, punchy results with strong local contrast

---

## Additional Features

### Horizon Leveling
Automatically detects and corrects tilted horizons in your final panorama. Uses edge detection to find the dominant horizontal line and rotates to level.

**When to use:** Handheld shots where you didn't have a tripod or level.

### Moving Object Removal (Beta)
Automatically detects and removes people, cars, and other moving objects during panorama stitching using temporal analysis of overlapping regions.

> **Beta Notice:** This feature works best with significant overlap between images and consistent movement patterns.

### Professional Export
- **JPEG** — Universal compatibility, adjustable quality
- **PNG** — Lossless compression, transparency support
- **HEIF** — Modern format, excellent compression, wide gamut
- **TIFF 16-bit** — Professional workflows, maximum quality
- **TIFF 32-bit** — HDR workflows, floating-point precision

---

## Tips for Best Results

### Panorama Shooting
1. **Overlap 30-50%** between adjacent images
2. **Keep the camera level** — use the grid overlay if available
3. **Lock exposure** — tap and hold to lock AE/AF before shooting
4. **Rotate around the lens** — not your body, to minimize parallax
5. **Shoot quickly** — minimize changes in lighting and moving objects

### Image Stacking
1. **Use a tripod** if possible (though handheld works for crowd removal)
2. **Same settings** — keep ISO, aperture, and shutter speed constant for noise reduction
3. **Bracket exposures** — vary only shutter speed for HDR
4. **More is better** — 10+ frames gives noticeably better results than 3-5

---

## Device Requirements

- **iPhone 12 Pro or later** / **iPad Pro with M1 or later**
- **iOS 17.0+**
- **500MB+ free storage**
- More RAM = larger panoramas possible

---

## Pricing

**$4.99** — One-time purchase, no subscription

Includes all features and all future updates. Try with included sample images before purchasing.

---

## Support

Having issues? We're here to help.

- **[Report a Bug](https://github.com/rfanimation/stitch-panorama-support/issues/new?template=bug_report.md)**
- **[Request a Feature](https://github.com/rfanimation/stitch-panorama-support/issues/new?template=feature_request.md)**
- **[Ask a Question](https://github.com/rfanimation/stitch-panorama-support/issues/new?template=question.md)**

---

## Privacy

Stitch processes all images **locally on your device**. We do not collect, store, or transmit your photos or any personal data. No account required, no analytics, no tracking.

[Read our full Privacy Policy](PRIVACY.md)

---

## Credits & Attribution

Stitch is built with these open-source technologies:

### OpenCV
**License:** Apache 2.0
**Website:** [opencv.org](https://opencv.org)

The Open Source Computer Vision Library provides the core stitching algorithms, including feature detection (ORB), homography estimation, bundle adjustment, seam finding, and multi-band blending.

### Depth Anything V2
**License:** Apache 2.0
**Paper:** [Depth Anything V2](https://arxiv.org/abs/2406.09414)
**Authors:** Lihe Yang, Bingyi Kang, Zilong Huang, et al.

State-of-the-art monocular depth estimation model used for depth-aware seam placement. Runs entirely on-device using Apple's Core ML framework.

---

## Beta Features

The following features are marked as Beta. They are functional but have not been extensively tested across all devices and image types:

| Feature | Status | Notes |
|---------|--------|-------|
| **Image Stacking** | Beta | All stacking modes (noise reduction, crowd removal, light trails, long exposure) |
| **HDR Processing** | Beta | Mertens and Debevec merge, all tone mapping operators |
| **Moving Object Removal** | Beta | Automatic removal during panorama stitching |

Beta features may experience:
- Unexpected results with certain image types
- Higher memory usage
- Longer processing times
- Occasional crashes on memory-constrained devices

We appreciate your patience as we continue to refine these features. Please [report any issues](https://github.com/rfanimation/stitch-panorama-support/issues/new?template=bug_report.md) you encounter.

---

## Version History

### 1.0 (Initial Release)
- Panorama stitching with 10 projection types
- Depth-aware seam placement
- Gigapixel support (100MP+)
- Ghost removal
- Image stacking (Beta): Noise reduction, crowd removal, light trails, long exposure
- HDR merge and tone mapping (Beta)
- Horizon leveling
- Professional export formats (JPEG, PNG, HEIF, TIFF)
- Sample images included for testing

---

<p align="center">
  <strong>Made for photographers who demand more</strong>
</p>
