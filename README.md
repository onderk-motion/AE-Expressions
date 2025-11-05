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

### Easy Ease (Custom)
**File:** `Animation/Easy Ease Custom.expr`
**Apply to:** Any property

Manual ease in/out control without keyframes. Create smooth animations with customizable easing curves.

**Key Parameters:**
- `easeIn` - Ease in amount (0 = linear, 100 = maximum)
- `easeOut` - Ease out amount (0 = linear, 100 = maximum)
- `duration` - Animation duration
- `startValue` & `endValue` - Value range

**Use Case:** Smooth transitions, custom timing curves, keyframe-free animation

---

### Overshoot
**File:** `Animation/Overshoot.expr`
**Apply to:** Position, Scale, Rotation, or any animated property

Overshoots the target value and bounces back for an elastic, springy feel.

**Key Parameters:**
- `overshootAmount` - How much to overshoot (1.1 = 10% over)
- `bounceSpeed` - Bounce frequency (1 = slow, 5 = fast)
- `smoothness` - Bounce smoothness (0.5 = bouncy, 0.9 = smooth)

**Use Case:** UI elements, elastic animations, organic motion

---

### Camera Shake
**File:** `Animation/Camera Shake.expr`
**Apply to:** Camera Position or Rotation (or any layer)

Realistic camera shake for impact, earthquake, or explosion effects with natural decay.

**Key Parameters:**
- `intensity` - Shake strength (10 = subtle, 100 = extreme)
- `frequency` - Shake speed (10 = slow, 30 = fast)
- `decay` - Fade speed (1 = slow, 5 = quick)
- `startTime` & `duration` - When and how long

**Use Case:** Impact effects, explosions, earthquakes, action scenes

---

### Look At Camera
**File:** `Animation/Look At Camera.expr`
**Apply to:** Orientation property of 3D layer

Automatically orients 3D layer to face camera or another layer - perfect for billboard effects.

**Key Parameters:**
- `mode` - Choose "camera" or "layer"
- `targetLayerName` - Layer to look at (if mode is "layer")
- `offsetX/Y/Z` - Rotation offsets

**Use Case:** Billboard effect, characters looking at camera, directional elements

---

### Oscillate
**File:** `Animation/Oscillate.expr`
**Apply to:** Position, Rotation, Scale, or any numeric property

Creates continuous back-and-forth motion like a pendulum with various wave types.

**Key Parameters:**
- `amplitude` - Range of motion
- `frequency` - Speed of oscillation (1 = slow, 3 = fast)
- `waveType` - Choose "sine", "triangle", "square", or "sawtooth"

**Use Case:** Pendulums, floating objects, breathing effects, alarm lights

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

### Typewriter Effect
**File:** `Text/Typewriter Effect.expr`
**Apply to:** Source Text property

Types out text character by character like a typewriter with optional blinking cursor.

**Key Parameters:**
- `charsPerSecond` - Typing speed (5 = slow, 20 = fast)
- `showCursor` - Display blinking cursor
- `cursorChar` - Cursor character (default: "|")

**Use Case:** Computer screens, subtitle effects, revealing text, retro effects

---

### Text Box Fitter
**File:** `Text/Text Box Fitter.expr`
**Apply to:** Scale or Size of shape layer behind text

Automatically adjusts background box/shape size based on text length with smooth animation.

**Key Parameters:**
- `textLayerName` - Name of text layer to track
- `padding` - Space around text (in pixels)
- `animationSpeed` - How fast box adjusts (1 = slow, 10 = instant)

**Use Case:** Dynamic buttons, animated labels, subtitle backgrounds, lower thirds

---

### Random Text Generator
**File:** `Text/Random Text Generator.expr`
**Apply to:** Source Text property

Generates random characters for Matrix, hacking, glitch, or data visualization effects.

**Key Parameters:**
- `textLength` - Number of characters
- `changeSpeed` - Character changes per second
- `characterSet` - Characters to use (binary, hex, letters, symbols, etc.)
- `groupSize` - Characters per group (0 = no grouping)

**Use Case:** Matrix effect, hacking scenes, glitch text, data streams, security codes

---

## 🎨 Color Expressions

### Connect Color Hue to Another Property
**File:** `Color/Connect Color Hue to Another Property.expr`
**Apply to:** Color properties

Links color hue values to another layer's color property for synchronized color changes.

**Use Case:** Color coordination, synchronized palettes, dynamic color schemes

---

### RGB Separation
**File:** `Color/RGB Separation.expr`
**Apply to:** Position of duplicated layers

Creates chromatic aberration/VHS glitch effect by separating RGB channels.

**Key Parameters:**
- `channel` - Set 0 (Red), 1 (Green), or 2 (Blue) for each layer
- `separationAmount` - Pixel offset (3 = subtle, 15 = extreme)
- `angle` - Separation direction (in degrees)

**Use Case:** VHS effects, glitch art, chromatic aberration, retro looks

**Setup:** Duplicate layer 3 times, apply expression with different channel values, use blend modes

---

### Color Cycle (Rainbow)
**File:** `Color/Color Cycle Rainbow.expr`
**Apply to:** Fill Color, Stroke Color, or any color property

Smoothly cycles through rainbow colors or custom color palettes over time.

**Key Parameters:**
- `cycleMode` - Choose "rainbow" or "custom"
- `cycleSpeed` - Cycles per second (0.5 = slow, 2 = fast)
- `customColors` - Define custom color palette (for custom mode)

**Use Case:** Neon signs, loading indicators, music visualizers, RGB lighting effects

---

### Brightness Based on Position
**File:** `Color/Brightness Based on Position.expr`
**Apply to:** Fill Color, Effect Color, or Opacity

Changes brightness/opacity based on distance from a light source position.

**Key Parameters:**
- `lightPosition` - Light source position [X, Y]
- `maxDistance` - Distance at which brightness reaches minimum
- `falloffType` - Choose "linear", "quadratic", or "smooth"

**Use Case:** Proximity lighting, spotlight effects, interactive lighting, depth effects

---

## 🔷 Shape Expressions

### Expand Linked Path Sizes
**File:** `Shape/Expand Linked Path Sizes.expr`
**Apply to:** Shape path properties

Dynamically expands or contracts shape paths while maintaining proportions and linked relationships.

**Use Case:** Responsive shapes, animated paths, scaling effects

---

### Auto Stroke Width
**File:** `Shape/Auto Stroke Width.expr`
**Apply to:** Stroke Width property

Maintains consistent stroke width regardless of layer scale - perfect for responsive designs.

**Key Parameters:**
- `baseStrokeWidth` - Desired width in pixels (at 100% scale)
- `scaleCompensation` - Enable/disable compensation
- `inheritParentScale` - Account for parent layer scale

**Use Case:** Logos with consistent line weight, icons, UI elements, technical drawings

---

### Path Trim Animator
**File:** `Shape/Path Trim Animator.expr`
**Apply to:** Trim Paths Start or End property

Smoothly animates path trimming for line drawing and reveal effects with various easing options.

**Key Parameters:**
- `applyTo` - Choose "start" or "end"
- `duration` - Animation duration
- `direction` - Choose "forward" or "reverse"
- `easeType` - Choose "linear", "smooth", or "bounce"

**Use Case:** Line reveals, drawing animations, write-on effects, path animations

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

### Snap to Grid
**File:** `Utility/Snap to Grid.expr`
**Apply to:** Position property

Snaps layer position to a grid system for pixel-perfect alignment and organized layouts.

**Key Parameters:**
- `gridSize` - Grid cell size in pixels (5, 10, 20, 50, etc.)
- `snapX/Y/Z` - Enable/disable snapping per axis
- `offset` - Grid origin offset

**Use Case:** Pixel art, UI alignment, organized layouts, isometric grids

---

### Layer Sequencer
**File:** `Utility/Layer Sequencer.expr`
**Apply to:** Opacity, Position, Scale, or any property

Automatically sequences animation across multiple layers based on index - perfect for cascading effects.

**Key Parameters:**
- `delayPerLayer` - Delay between each layer (in seconds)
- `animationDuration` - How long each animation takes
- `startValue` & `endValue` - Animation range
- `reverseOrder` - Reverse sequence direction

**Use Case:** Sequential reveals, cascading effects, stagger animations, menu animations

---

### Value Remap/Range
**File:** `Utility/Value Remap Range.expr`
**Apply to:** Any property

Remaps values from one range to another (like Arduino's map function) - extremely versatile utility.

**Key Parameters:**
- `inputMin` & `inputMax` - Source value range
- `outputMin` & `outputMax` - Target value range
- `sourceValue` - Value to remap (can link to other properties)

**Use Case:** Mapping sliders to properties, converting ranges, linking different property types

---

### Exponential Growth/Decay
**File:** `Utility/Exponential Growth Decay.expr`
**Apply to:** Any numeric property

Creates exponential growth (viral spread) or decay (fade out) curves for dramatic effects.

**Key Parameters:**
- `mode` - Choose "growth" or "decay"
- `rate` - Speed of change (1 = slow, 5 = fast)
- `startValue` & `endValue` - Value range

**Use Case:** Viral growth, social media counters, explosions, deceleration, signal loss

---

### Blink/Flicker
**File:** `Utility/Blink Flicker.expr`
**Apply to:** Opacity property

Creates blinking or flickering effects with various patterns including morse code.

**Key Parameters:**
- `pattern` - Choose "blink", "flicker", "random", or "morse"
- `frequency` - Blinks per second
- `onOpacity` & `offOpacity` - On/off values
- `dutyCycle` - ON duration ratio

**Use Case:** Warning lights, broken screens, cursor blinks, morse signals, faulty electronics

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

Have a useful expression to share? Contributions are welcome!

**Guidelines:**
- Code must be well-commented with clear explanations
- Include usage instructions and parameter descriptions
- Follow the existing file structure and naming conventions
- Use descriptive file names with `.expr` extension
- Test your expressions before submitting

Open an issue or pull request to contribute your expressions!

## 📄 License

These expressions are free to use in personal and commercial projects. Attribution is appreciated but not required.

## 💬 Support

If these expressions helped you, consider [buying me a coffee](https://www.buymeacoffee.com/onderk_motion)!

---

**Created by Onder** - Sr. Motion Designer & Content Creator
*Making motion design more efficient, one expression at a time.*
