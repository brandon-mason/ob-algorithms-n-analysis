## Homography
Homography is a concept that describes the relationship between two different views of the **same planar surface** (like a piece of paper or a wall) taken from different angles or positions. It helps us answer: "If I know where a point is in one image, where does it end up in a second image, after a viewpoint change?"

Describes the relationship between one point on two on different images.

Represented by a 3x3 matrix:
![[Pasted image 20251006222526.png]]
where ***H*** is the homography matrix, and (x1, y1) and (x2, y2) are matching points on two images.
### What the Matrix Does
- The matrix maps points from the coordinate system of one image (the source plane) to the coordinate system of the other (the destination plane).[](https://www.productteacher.com/quick-product-tips/homography-for-computer-vision-product-managers)
- It captures all planar transformations: rotations, translations, scaling, and perspective effects between the two views.[](https://www.geeksforgeeks.org/computer-vision/what-is-homography-how-to-estimate-homography-between-two-images/)
- Applying the matrix (with `cv2.warpPerspective` in OpenCV) effectively re-aligns and transforms an entire image based on this mapping.