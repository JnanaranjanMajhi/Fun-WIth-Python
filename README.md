# Fun-WIth-Python
## 🎨 Overview

Creates dynamic, animated visualizations by computing the positions of 10,000 points using sophisticated parametric equations involving trigonometric functions, square roots, and time-dependent variables. The result is a continuously morphing point cloud that creates beautiful, hypnotic patterns.

## ✨ Features

- **Real-time Animation**: Smooth 20 FPS animation with 100-frame cycles
- **Mathematical Beauty**: Complex parametric equations creating organic, flowing patterns
- **High Resolution**: 10,000 individual points for detailed visualizations
- **Customizable Output**: Option to save animations as GIF files
- **Optimized Performance**: Vectorized NumPy operations for efficient computation

## 🔧 Requirements

- Python 3.6 or higher
- NumPy
- Matplotlib

## 📦 Installation

1. Clone this repository:
```bash
git clone https://github.com/001shahab/kuzuri.git
cd kuzuri
```

2. Install the required dependencies:
```bash
pip install -r requirements.txt
```

## 🚀 Usage

### Basic Usage
Run the visualization directly:
```bash
python Animation.py
```

## 🧮 Mathematical Foundation

The visualization is based on parametric equations that transform each point through several mathematical operations:

1. **Base Coordinates**: Points are generated from indices 0 to 9999
2. **Trigonometric Transformations**: Multiple sine and cosine functions create wave-like patterns
3. **Time Dependency**: The parameter `t` evolves over time, creating smooth animations
4. **Spatial Mapping**: Final coordinates are mapped to screen space with appropriate scaling

Key equations include:
- `k = (4 + sin(x/11 + 8t)) * cos(x/14)`
- `d = sqrt(k² + e²) + sin(y/9 + 2t)`
- `q = 2*sin(2k) + sin(y/17) * k * (9 + 2*sin(y - 3d))`

## 🎛️ Customization

You can modify various parameters in `Animation.py`:

- **Point Count**: Change the range in `np.arange(9999, -1, -1)`
- **Animation Speed**: Adjust the `interval` parameter in `FuncAnimation`
- **Color Scheme**: Modify the `c` parameter in `ax.scatter()`
- **Mathematical Functions**: Experiment with the parametric equations
- **Window Size**: Adjust `figsize` parameter

## 🔬 Technical Details

- **Framework**: Built with NumPy and Matplotlib
- **Performance**: Utilizes vectorized operations for optimal speed
- **Memory Usage**: Efficiently handles 10,000 points in real-time
- **Animation**: Uses `FuncAnimation` with blitting for smooth rendering

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. Some ideas for contributions:

- Additional mathematical functions and patterns
- Interactive parameter controls
- 3D visualizations
- Performance optimizations
- New color schemes and visual effects

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Inspired by mathematical art and parametric equation visualizations
- Built with the powerful Python scientific computing ecosystem

## 📚 References

- [NumPy Documentation](https://numpy.org/doc/)
- [Matplotlib Animation Tutorial](https://matplotlib.org/stable/tutorials/advanced/blitting.html)
- [Parametric Equations in Computer Graphics](https://en.wikipedia.org/wiki/Parametric_equation)

---

*"Mathematics is the art of giving the same name to different things." - Henri Poincaré*
