# GVC-Project
# 3D Sorting Algorithm Visualization – README

## 📌 Objective
The objective of this project is to visually demonstrate how the **Bubble Sort** algorithm works using a **3D bar visualization**.  
Each element in the array is represented as a 3D bar whose **height corresponds to its value**.  
The program also illustrates core **computer graphics concepts** such as:
- Object modeling  
- Transformations  
- 3D viewing pipeline  
- Depth ordering (Z-buffer equivalent)  
- Frame buffer generation  
- Animation sequencing  

This project serves as both a sorting demonstration and a practical visual implementation of 3D graphics principles—without requiring Maya or Blender.

---

## 🛠 Toolchain Used
This project uses a fully Python-based workflow:

### **Programming Language**
- Python 3.x

### **Libraries**
- **Matplotlib (mplot3d)** – for 3D visualization  
- **NumPy** – generating and manipulating numerical data  
- **ReportLab** – for generating PDF posters  
- **Python-pptx** – for generating slide files  
- **PillowWriter** (via matplotlib) – creating GIF animations  

### **Optional Tools**
- **FFmpeg** – convert frames or GIF into MP4  
- **OBS Studio** – screen-record visualization window for MP4 output  

Everything runs locally and does **not** require any 3D modeling software.

---

## 📈 Methodology

### **1. Data Creation**
A random array of values is generated using NumPy.  
These values are used as heights for the 3D bars.

### **2. Bubble Sort Simulation**
As Bubble Sort runs:
- Every time two elements are swapped, a **snapshot** of the array is taken.
- These snapshots represent the steps of the algorithm.

### **3. 3D Modeling**
Each array element becomes one 3D bar defined by:
- X-position → index of element  
- Z-height → element value  
- Y-position → constant (aligned for simplicity)  
- Dimensions (dx, dy, dz) → bar width, depth, and height  

### **4. Transformations**
- **Translation**: bars are placed along the x-axis  
- **Scaling**: bar height scaled to represent value  
- **Camera Rotation**: slight azimuth rotation for 3D effect  

### **5. Rendering & Frame Buffer**
For each snapshot:
- A 3D bar plot is rendered  
- Frame is saved as a PNG → stored in `frames/`  
- These frames form the animation sequence  

### **6. Exporting Output**
Outputs include:
- A GIF animation of the sorting process  
- A PPT with key frames inserted  
- A PDF poster with multiple screenshots  
- A final ZIP submission folder  

---

## 🖼 Screenshots

Below are key example frames used in the project (6 samples shown in the PDF poster):

- `frames/frame_0000.png`
- `frames/frame_00XX.png` (mid-animation frames)
- `frames/frame_last.png`

These images represent different steps of the bubble sort process.

*(For the actual images, refer to the `/frames` folder included in your submission.)*

---

## 📦 File Structure

```
final_sorting_pack/
│
├── sorting_visualization.py        # Main Python script
├── sorting_visualization.gif       # Rendered animation
├── SortingVisualization.pptx       # Auto-generated PPT
├── Sorting_Visualization_Poster_Enhanced.pdf   # Final Poster
├── frames/                         # All generated frames
│   ├── frame_0000.png
│   ├── frame_0001.png
│   └── ...
└── README.md                       # This file
```

---

## 📚 References
- Matplotlib 3D documentation  
- NumPy official documentation  
- Standard Bubble Sort algorithm descriptions  
- FFmpeg and GIF animation resources  

---

## 📝 Author Notes
This project was built to be:
- Lightweight  
- Easy to understand  
- Fully Python-based  
- Compatible with assignment requirements that normally require Maya/3D software  

If you need improvements (coloring bars, comparing highlights, MP4 export, UI), they can be added easily.

---

## ✔ End of README
