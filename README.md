# ImageIO GIF Maker

A simple Python project for creating animated GIFs from a series of PNG images using the [imageio](https://imageio.readthedocs.io/) library.

## Features

- Combines multiple PNG images into a single GIF.
- Uses `imageio.v3` for reading and writing image files.
- Adjustable frame duration and looping options.

## Requirements

- Python 3.x
- [imageio](https://pypi.org/project/imageio/)
- [numpy](https://pypi.org/project/numpy/)
- [pillow](https://pypi.org/project/Pillow/)

Install dependencies:
```bash
pip install imageio numpy pillow
```

## Usage

1. Place your PNG images (e.g., `team-pic1.png`, `team-pic2.png`) in the project directory.
2. Run the script or notebook to generate an animated GIF (`team.gif`).

Example code:
```python
import imageio.v3 as iio

filenames = ['team-pic1.png', 'team-pic2.png']
images = [iio.imread(filename) for filename in filenames]

iio.imwrite('team.gif', images, duration=500, loop=0)
```

- `duration` sets the time (in milliseconds) each frame is shown.
- `loop=0` means the GIF will loop infinitely.

## Repository Setup Instructions

1. **Initialize Git**  
   ```bash
   git init
   ```
2. **Stage Files**  
   ```bash
   git add .
   ```
3. **Commit Changes**  
   ```bash
   git commit -m "Initial commit"
   ```
4. **Set Up Remote Repository**  
   ```bash
   git remote add origin <your-repo-url>
   ```
5. **Push to GitHub**  
   ```bash
   git push -u origin main
   ```

## Notes

- This project is designed for educational purposes and easy GIF creation.
- For more advanced GIF options, refer to the official [imageio documentation](https://imageio.readthedocs.io/).

## License

MIT License

---

**Author:** asha2409
