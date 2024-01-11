
<p align="center">
  <img src="/glass.png" alt="Glassmorphism">
</p>

# Tailwind Glassmorphism

[![npm](https://img.shields.io/npm/v/tailwind-glassmorphism)](https://www.npmjs.com/package/tailwind-glassmorphism)
[![GitHub license](https://github.com/AtharvaMistry/tailwind-classes)](https://github.com/AtharvaMistry/tailwind-classes)

A customizable Tailwind CSS utility for effortlessly adding Glassmorphism design effects to your web projects.

Glassmorphism is a modern design trend that brings a frosted glass-like appearance with a blurred background, providing a sleek and contemporary feel to your user interface.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Advanced Customization](#advanced-customization)
- [Examples](#examples)
- [Documentation](#documentation)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Features

- Easily create Glassmorphism effects in your Tailwind CSS project.
- Customizable transparency, shadows, and color schemes.
- Compatible with responsive and hover states.

## Installation

Install the package via npm:

```bash
npm install tailwind-glassmorphism
```

## Usage

1. **Include the Plugin in Tailwind Config:**

   Add the custom utility to your `tailwind.config.js` file:

   ```javascript
   // tailwind.config.js
   module.exports = {
     // ... other configurations
     plugins: [
       // ... other plugins
       require('tailwind-glassmorphism'),
     ],
   };
   ```

2. **Apply the Glassmorphism Class:**

   Use the `.glassmorph` class in your HTML or JSX to apply the Glassmorphism effect:

   ```html
   <div class="glassmorph">
     <!-- Your content goes here -->
   </div>
   ```

   Example in React JSX:

   ```jsx
   import React from 'react';

   const App = () => {
     return (
       <div className="glassmorph">
         {/* Your content goes here */}
       </div>
     );
   };

   export default App;
   ```

   Apply additional styles to customize the effect further:

   ```html
   <div class="glassmorph my-custom-styles">
     <!-- Your content goes here -->
   </div>
   ```

   ```jsx
   const App = () => {
     return (
       <div className="glassmorph my-custom-styles">
         {/* Your content goes here */}
       </div>
     );
   };
   ```

## Advanced Customization

For advanced customization, you can modify the `.glassmorph` class in your plugin file (`glassmorphism-plugin.js`). Adjust colors, shadows, and other properties to suit your design preferences:

```javascript
// glassmorphism-plugin.js
const plugin = ({ addUtilities }) => {
  const newUtilities = {
    '.glassmorph': {
      background: 'rgba(255, 255, 255, 0.1)', // Adjust the alpha channel for transparency
      // ... other styles
    },
  };
  addUtilities(newUtilities, ['responsive', 'hover']);
};

module.exports = plugin;
```

## Examples

Check the [`examples/`](examples/) directory for usage examples and demos.

## Documentation

For detailed documentation and advanced customization options, refer to the [official documentation](docs/README.md).

## Troubleshooting

If you encounter any issues, please check the [Troubleshooting Guide](docs/TROUBLESHOOTING.md) for common solutions.

## Contributing

We welcome contributions! Check out the [Contribution Guidelines](CONTRIBUTING.md) for details.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## Acknowledgments

- Inspired by the Glassmorphism design trend.
