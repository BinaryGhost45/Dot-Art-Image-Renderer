# Dot Art Image Renderer

Turn any image into elegant **dot-style ASCII art** using Python.

This renderer uses the pixel brightness of an image to draw dots of varying sizes, creating a clean, minimalistic output saved as a `.jpg` file.

Perfect for artistic experimentation, retro visuals, and lightweight aesthetic renderings. Simply provide an image path, and the program handles the rest using only the `Pillow` library.

---

## Features

- Supports common image formats (JPG, PNG, BMP, etc.)
- Accepts the image path at runtime
- Grayscale-based dot sizing (darker pixels produce larger dots)
- Optimized for fast rendering
- Automatically saves the output as a `.jpg` in the same directory
- Written in pure Python with only one dependency (`Pillow`)
- Clean, modular code that is easy to modify and extend

---

## How It Works

### Process

1. **User Input**
   - Enter the full path to an image file.

2. **Image Preprocessing**
   - The image is resized to a fixed width (default: `100px`) while preserving its aspect ratio.
   - It is then converted to grayscale, where pixel values range from `0` (black) to `255` (white).

3. **Dot Rendering**
   - Each pixel's brightness determines the radius of a black dot drawn on a white canvas.
   - Darker pixels produce larger dots, while lighter pixels produce smaller dots or none at all.

4. **Output**
   - The generated image is saved as `dot_art_output.jpg` in the same directory as the input image.

---

## Getting Started

### Install Dependencies

```bash
pip install pillow
```

### Run the Program

```bash
python main.py
```

When prompted, enter the full path to your image file.

---

## Output

The rendered image is automatically saved as:

```
dot_art_output.jpg
```

in the same directory as the source image.

---

## Download

Download the latest Windows executable from the Releases page:

https://github.com/BinaryGhost45/-Dot-Art-Image-Renderer/releases/tag/v1.0.0

---

## Requirements

- Python 3.8 or later
- Pillow

---

## License

This project is open source. See the `LICENSE` file for details.
