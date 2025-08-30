# Geometric-Transformations-in-Computer-Vision
Geometric-Transformations-in-Computer-Vision

This repository demonstrates **geometric transformations** in image processing using **Python** and **OpenCV**.  
Geometric transformations are fundamental operations that change the position, orientation, or perspective of an image without altering its pixel values.  
They are widely used in **computer vision, robotics, machine learning, AR/VR, and graphics**.  

---

## 📖 Overview
Geometric transformations allow us to manipulate images in space.  
This project explains and implements:
- **Basic transformations** → Translation, Rotation, Scaling, Flipping  
- **Advanced transformations** → Affine and Perspective  

Each transformation is explained in detail with mathematical background and real-world applications.

---

## 🔑 Types of Transformations in This Project

### 1️⃣ Translation
- **What it is**: Shifts an image from one place to another.  
- **How it works**: Each pixel `(x, y)` is moved to `(x + tx, y + ty)`.  
- **Key Points**:
  - Only position changes, shape and size remain the same.  
  - Can be horizontal, vertical, or both.  
- **Applications**:
  - Aligning multiple images.  
  - Moving objects within a frame.  
  - Image stitching in panorama creation.  

---

### 2️⃣ Rotation
- **What it is**: Turns the image around a fixed point (usually the center).  
- **How it works**: Uses a rotation matrix with angle θ.  
- **Key Points**:
  - Angle decides clockwise or counterclockwise rotation.  
  - Pivot point can be the center or any custom point.  
- **Applications**:
  - Correcting tilted images.  
  - Data augmentation in deep learning.  
  - Medical scan alignment.  

---

### 3️⃣ Scaling (Resizing)
- **What it is**: Enlarges or shrinks the size of an image.  
- **How it works**: Multiplies coordinates `(x, y)` by scaling factors `(sx, sy)`.  
- **Key Points**:
  - `sx, sy > 1` → enlargement.  
  - `0 < sx, sy < 1` → shrinking.  
  - Keep aspect ratio to avoid distortion.  
- **Applications**:
  - Compressing or enlarging images.  
  - Preparing fixed-size inputs for CNNs.  
  - Zooming in/out effects.  

---

### 4️⃣ Flipping (Reflection)
- **What it is**: Creates a mirror image of the original.  
- **Types**:
  - Horizontal flip (mirror across vertical axis).  
  - Vertical flip (mirror across horizontal axis).  
  - Both axes.  
- **Key Points**:
  - Orientation changes but size remains same.  
  - Common in dataset augmentation.  
- **Applications**:
  - Facial symmetry analysis.  
  - Data augmentation in deep learning.  
  - Graphics and photography effects.  

---

### 5️⃣ Affine Transformation
- **What it is**: A linear transformation that preserves points, straight lines, and parallelism.  
- **How it works**: Defined by a **2×3 matrix** and requires at least 3 points.  
- **Key Points**:
  - Can combine rotation, translation, scaling, and shearing.  
  - Parallel lines remain parallel, but angles may change.  
- **Applications**:
  - Correcting skewed documents.  
  - Shape analysis in computer vision.  
  - Map transformation in GIS.  

---

### 6️⃣ Perspective Transformation
- **What it is**: Warps an image as if viewed from a different angle.  
- **How it works**: Requires 4 corresponding points between source and destination.  
- **Key Points**:
  - Straight lines remain straight.  
  - Produces a “tilted” or 3D-like effect.  
- **Applications**:
  - Correcting perspective in photographs.  
  - Augmented reality overlays.  
  - 3D scene reconstruction.  

---

## 📊 Real-World Applications of Geometric Transformations
- 🔹 **Computer Vision** → Object detection, tracking, face recognition.  
- 🔹 **Medical Imaging** → Aligning CT/MRI scans.  
- 🔹 **Deep Learning** → Data augmentation for robust training.  
- 🔹 **Robotics** → Camera calibration and environment mapping.  
- 🔹 **AR/VR** → Overlaying digital objects on real scenes.  
- 🔹 **Graphics & Photography** → Special effects and perspective correction.  
