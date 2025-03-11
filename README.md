# 🚀 CounterUp.js

**Advanced Vanilla JavaScript Counter Animation**  
_Inspired by jquery.counterUp.js—dependency-free and ready for production!_

---

## 🔥 Key Features

- **Zero Dependencies**: Lightweight and efficient—no external libraries required.
- **Intersection Observer Integration**: Animations trigger intelligently as counters scroll into view.
- **Smooth Animations**: Utilizes `requestAnimationFrame` for optimal performance and smooth effects.
- **Flexible Number Formatting**: Supports decimals, separators, prefixes (e.g., `$`), and suffixes (e.g., `%`).
- **Multiple Easing Options**: Built-in easing functions (`easeOutExpo`, `easeInCubic`, etc.) for dynamic animation effects.
- **Highly Customizable**: Easy to adjust duration, offset, formatting, and more.

---

## 💡 Usage

### Quick Start

```javascript
import CounterUp from './CounterUp.js';

// Initialize CounterUp
const counter = new CounterUp('.counter', {
  duration: 1200,
  easing: 'easeOutExpo',
  once: true,
  separator: ',',
  prefix: '$',
  suffix: '+'
});
```

### HTML Example
```html
<div class="counter">1,500</div>
<div class="counter">2500.50</div>
<div class="counter">$5,000+</div>
```

### ⚙️ Configuration Options
| Option    | Type    | Default       | Description                                 |
|-----------|---------|---------------|---------------------------------------------|
| duration  | number  | `800`         | Total animation duration in milliseconds.   |
| easing    | string  | `easeOutExpo` | Easing function used for the animation.     |
| offset    | string  | `0%`          | Offset value for IntersectionObserver.      |
| once      | boolean | `false`       | If true, animation triggers only once.      |
| decimals  | number  | `null`        | Number of decimals (null auto-detects).     |
| separator | string  | `,`           | Thousands separator character.              |
| prefix    | string  | `''`          | Prefix added before number (e.g., `$`).     |
| suffix    | string  | `''`          | Suffix added after number (e.g., `%`).      |


### 🎯 Public Methods
- `updateOptions(options)`: Dynamically update configuration.
- `restart()`: Restart animations and observers completely.
- `replay()`: Replay animations without resetting observers.
- `destroy()`: Clean up observers and animations to free resources.

### 📦 Installation
Clone or download the repository:
```bash
git clone <your-repo-url>
```

Or include directly into your HTML:
```html
<script type="module" src="/path/to/CounterUp.js"></script>
```
### 📈 Browser Support
Fully compatible with modern browsers supporting:

- Intersection Observer API
- requestAnimationFrame

_(Consider polyfills for legacy browser support.)_

## 📝 License
MIT License
