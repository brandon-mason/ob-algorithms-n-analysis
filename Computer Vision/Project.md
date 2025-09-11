*HSV(Hue, Saturation, Value)*
*Kernel:* 
*Erosion:* Whatever overlaps with the kernel is kept.
*Dialation:*
### detect_line_staff
**cv2.cvtColor(src, code[, dst[, dstCn]])**
*Parameters:*
- **`src`**: input image whose color space is to be changed.
- **`code`**: color space conversion code (e.g., cv2.COLOR_BGR2GRAY).
- **`dst(Optional)`**: Output image of the same size and depth as src.
- **`dstCn(Optional)`**: Number of channels in destination image. If *0*, it’s derived automatically.

**cv2.inRange(src, lowerb, upperb)**
Used for color detection. Checks every pixel in src to see if it falls in the HSV range
*Parameters:*
- **`src`**: The input image in HSV color space.
- **`lowerb`**: The lower boundary of the color you want to detect (as a tuple of HSV values).
- **`upperb`**: The upper boundary of the color.
*Returns:*
A binary mask, where pixels inside the specified range are white (255), and pixels outside the range are black (0).