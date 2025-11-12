# 🟩 VibeCharts — Advanced JavaScript Charting Library

**VibeCharts** is a powerful, dependency-free JavaScript charting library designed for speed, simplicity, and beauty.  
It’s lightweight, fully responsive, and offers smooth animations — perfect for dashboards, analytics, and interactive data visualizations.

---

## ✨ Features

- ⚡ **Lightning Fast** — Built in pure JavaScript, no dependencies.  
- 🎨 **Customizable** — Complete control over colors, styles, and animations.  
- 📱 **Responsive** — Scales beautifully across all devices.  
- 🧩 **Modular Architecture** — Easy to extend and integrate.  
- 🕹️ **Animations** — Smooth transitions and loading placeholders.  
- 🌙 **Themes** — Includes Dark, Light, Gradient, and Glass themes.  
- 📊 **Chart Types** — Bar, Line, Pie, Donut, Area, Radar, Gauge, Waterfall, and more.

---

## 🚀 Getting Started

### 1. Include VibeCharts

Add the JS and CSS files to your project:
```html
<link rel="stylesheet" href="VibeCharts.css">
<script src="VibeCharts.js"></script>
```

### 2. Basic Usage
Create a container for your chart:

```
<div id="chart1" style="height: 300px;"></div>
```

#### Initialize a chart:

```
new VibeCharts('chart1', {
  type: 'bar',
  data: [
    { label: 'Jan', value: 45 },
    { label: 'Feb', value: 62 },
    { label: 'Mar', value: 58 },
    { label: 'Apr', value: 73 },
    { label: 'May', value: 89 }
  ],
  theme: 'dark',
  showLegend: true,
  legendPosition: 'bottom'
});
```

#### 🎨 Customization

Themes
```
theme: 'gradient',
style: 'rounded'
```

### Chart Types
Supported types include:

```
bar, line, pie, donut, area, radar, waterfall, gauge, heatmap, polar
```

Example:
```
new VibeCharts('chart2', { type: 'line', ... });
```

#### Responsive & Dynamic Updates
VibeCharts automatically resizes with the container.
You can also load or update data dynamically:
```
chart.loadData('/api/sales.json');
chart.updateOptions({ theme: 'dark', style: 'soft' });
```

### ⚙️ Configuration Options
Option	Type	Default	Description
```
type	string	'bar'	Chart type
data	array	[]	Array of { label, value } objects
theme	string	'dark'	Chart theme
style	string	'default'	Shape style (default, soft, rounded)
showLegend	bool	true	Show or hide legend
legendPosition	string	'bottom'	top / bottom / left / right
barColorMode	string	'series'	series / individual / shade
lineFill	bool	false	Fill area below line
animationDuration	int	800	Milliseconds for render animation
responsive	bool	true	Enable automatic resize
showPlaceholder	bool	true	Show shimmer loading placeholder
```

#### 🧠 Example: Donut Chart
```
new VibeCharts('chart4', {
  type: 'donut',
  data: [
    { label: 'Desktop', value: 45 },
    { label: 'Mobile', value: 35 },
    { label: 'Tablet', value: 20 }
  ],
  theme: 'dark',
  showLegend: true,
  legendPosition: 'bottom'
});
```

### 🧰 Developer Notes
Fully object-oriented class design (VibeCharts)
Uses HTML5 Canvas for rendering
Supports async data loading via loadData(url)
Compatible with all modern browsers
Zero external dependencies

### 🖤 License
MIT License
© 2025 VibeCharts

### 📫 Contact
Email: alteredindian@gmail.com
Website: https://alteredindian.in
GitHub: [https://github.com/alteredindian/VibeCharts](https://github.com/alteredindian/VibeCharts/)

### 🌟 Credits
Built with passion and precision for developers who love data.
Copy code

---
