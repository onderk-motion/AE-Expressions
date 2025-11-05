# After Effects Expressions Library

[![Buy Me A Coffee](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/onderk_motion)

A comprehensive collection of useful After Effects expressions for motion designers and animators. These expressions are production-ready and designed to speed up your workflow.

## 👋 About

Hi, I'm Onder - a Freelance Sr. Motion Designer and Content Creator. I've created these expressions through years of production work, and I'm sharing them with the community. Feel free to use and customize them for your projects!

---

## 📁 Repository Structure

The expressions are organized into categories for easy navigation:

```
AE-Expressions/
├── Animation/       # Motion, timing, and animation effects
├── Text/           # Text manipulation and formatting
├── Color/          # Color-related expressions
├── Shape/          # Shape layer operations
└── Utility/        # General-purpose utilities
```

---

## 🎬 Animation Expressions

### Bounce Effect
**File:** `Animation/Bounce Effect.expr`
**Apply to:** Position, Scale, Rotation, or any animated property

Adds a natural spring/bounce effect to your animations. Perfect for creating organic motion with controllable intensity and decay.

**Key Parameters:**
- `amp` - Bounce intensity (0.05 = subtle, 0.3 = strong)
- `freq` - Bounce speed (1 = slow, 4 = fast)
- `decay` - How quickly it settles (3 = slow, 8 = fast)

**Use Case:** Logo reveals, text animations, UI elements

---

### Smooth Inertia
**File:** `Animation/Smooth Inertia.expr`
**Apply to:** Any property

Creates smooth follow-through animation with lag/delay. Excellent for creating secondary motion or making one layer follow another with natural delay.

**Key Parameters:**
- `delay` - Response time (3 = quick, 10 = slow)
- `smoothness` - Transition smoothness (50 = loose, 95 = very smooth)

**Use Case:** Follow cameras, delayed animations, organic motion

---

### Wiggle with Limits
**File:** `Animation/Wiggle with Limits.expr`
**Apply to:** Position, Rotation, Scale, Opacity

Standard wiggle expression but constrained between minimum and maximum values. Prevents wiggle from going out of control.

**Key Parameters:**
- `freq` - Wiggle frequency (1 = slow, 5 = fast)
- `amp` - Wiggle intensity
- `minValue` & `maxValue` - Boundary limits

**Use Case:** Handheld camera shake, subtle movements, controlled randomness

---

### Loop Out with Offset
**File:** `Animation/Loop Out with Offset.expr`
**Apply to:** Position, Rotation, or any animated property with keyframes

Loops your animation but adds offset each cycle - perfect for walk cycles, rolling wheels, or any repeating motion that needs to progress.

**Key Parameters:**
- `offsetValue` - How much to progress per loop

**Use Case:** Walk cycles, rolling objects, repeating patterns with progression

---

### Rotation from Velocity
**File:** `Animation/Rotation from Velocity.expr`
**Apply to:** Rotation property

Automatically rotates layer based on its movement direction. The layer will always face the direction it's moving.

**Key Parameters:**
- `smoothness` - Rotation lag (0.05 = responsive, 0.2 = smooth)
- `offset` - Direction correction in degrees

**Use Case:** Flying objects, vehicles, directional arrows

---

### Keyframeless Animation
**File:** `Animation/Keyframeless Animation.expr`
**Apply to:** Any property

Creates continuous animation without keyframes using time-based functions.

**Use Case:** Continuous motion, procedural animations

---

### Multiple Position Follow by Markers
**File:** `Animation/Multiple Position Follow by Markers.expr`
**Apply to:** Position property

Animates position based on composition markers for precise timing control.

**Use Case:** Marker-driven animations, synchronized movements

---

### Time Remap to Comp Markers
**File:** `Animation/Time Remap to Comp Markers.expr`
**Apply to:** Time Remap property

Maps layer time to composition markers for advanced timing control.

**Use Case:** Frame-accurate timing, marker-based playback

---

## 📝 Text Expressions

### Text Counter
**File:** `Text/Text Counter.expr`
**Apply to:** Source Text property

Smoothly animates numbers counting from one value to another. Professional-looking counters with customizable formatting.

**Key Parameters:**
- `decimalPlaces` - Number formatting (0 = whole numbers)
- `prefix` & `suffix` - Add currency symbols, units, etc.
- `useCommas` - Thousand separators (1,000 vs 1000)

**Use Case:** Statistics, counters, animated numbers, data visualization

---

### Time to Frames
**File:** `Text/Time to Frames.expr`
**Apply to:** Source Text property

Displays current time as frame number or timecode. Perfect for creating custom timecode displays.

**Key Parameters:**
- `displayMode` - Choose "frames", "timecode", or "seconds"
- `startOffset` - Start counting from specific frame
- `useCompTime` - Use composition or layer time

**Use Case:** Timecode displays, frame counters, video editing tools

---

### Letter Index Number
**File:** `Text/Letter Index Number.expr`
**Apply to:** Source Text property

Manipulates text based on character index and position.

**Use Case:** Character-by-character animations, text effects

---

### Source Text (charAt())
**File:** `Text/Source Text (charAt()).expr`
**Apply to:** Source Text property

Advanced text character manipulation and extraction.

**Use Case:** Dynamic text effects, character-level control

---

## 🎨 Color Expressions

### Connect Color Hue to Another Property
**File:** `Color/Connect Color Hue to Another Property.expr`
**Apply to:** Color properties

Links color hue values to another layer's color property for synchronized color changes.

**Use Case:** Color coordination, synchronized palettes, dynamic color schemes

---

## 🔷 Shape Expressions

### Expand Linked Path Sizes
**File:** `Shape/Expand Linked Path Sizes.expr`
**Apply to:** Shape path properties

Dynamically expands or contracts shape paths while maintaining proportions and linked relationships.

**Use Case:** Responsive shapes, animated paths, scaling effects

---

## 🛠️ Utility Expressions

### Scale to Fit Comp
**File:** `Utility/Scale to Fit Comp.expr`
**Apply to:** Scale property

Automatically scales any layer to fit composition dimensions while maintaining aspect ratio. Works with any source dimension.

**Key Parameters:**
- `fitMode` - Choose "contain" (fit inside) or "cover" (fill completely)

**Use Case:** Responsive design, automatic scaling, multi-resolution workflows

---

### Distance Between Layers
**File:** `Utility/Distance Between Layers.expr`
**Apply to:** Opacity, Scale, or any numeric property

Calculates distance between two layers and maps it to property values. Create proximity-based effects.

**Key Parameters:**
- `targetLayerName` - Layer to measure distance to
- `minDist` & `maxDist` - Distance range in pixels
- `minValue` & `maxValue` - Output value range

**Use Case:** Proximity-based opacity, distance-driven animations, interactive effects

---

### Random Seed Based
**File:** `Utility/Random Seed Based.expr`
**Apply to:** Any property

Generates controllable random values using seed numbers. Same seed always produces same random values - perfect for consistent randomness across multiple layers.

**Key Parameters:**
- `seed` - Control randomness (same seed = same result)
- `minValue` & `maxValue` - Random value range

**Use Case:** Consistent randomness, duplicated layers with variation, controlled chaos

**Pro Tip:** Use `seed = index;` to give each layer unique but consistent random values.

---

### Count Layer with Name
**File:** `Utility/Count Layer with Name.expr`
**Apply to:** Any property

Counts layers with specific name patterns and uses the count to drive property values.

**Use Case:** Dynamic layer management, counting systems

---

### Pad Zero Function
**File:** `Utility/Pad Zero Function.expr`
**Apply to:** Text or numbering systems

Formats numbers with leading zeros (1 → 01, 2 → 02, etc.).

**Use Case:** Frame numbering, organized sequences, file naming

---

## 🚀 How to Use

1. **Browse** the category folders to find the expression you need
2. **Open** the `.expr` file in a text editor
3. **Copy** the expression code
4. **Paste** into your After Effects property
5. **Customize** the parameters at the top of each expression
6. **Read** the comments in each file for detailed usage instructions

## 📖 Tips

- All expressions include detailed comments and usage instructions
- Parameters are clearly marked at the top of each expression
- Most expressions work with both 2D and 3D layers
- Test with a single layer before applying to multiple layers
- Adjust parameters to match your specific needs

## 🤝 Contributing

Have a useful expression to share? Feel free to contribute! Please ensure:
- Code is well-commented
- Include usage instructions
- Follow the existing file structure
- Use descriptive file names

## 📄 License

These expressions are free to use in personal and commercial projects. Attribution is appreciated but not required.

## 💬 Support

If these expressions helped you, consider [buying me a coffee](https://www.buymeacoffee.com/onderk_motion)!

---

**Created by Onder** - Sr. Motion Designer & Content Creator
*Making motion design more efficient, one expression at a time.*
