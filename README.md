# Phys-GS Lite: Material-Aware Dynamic Gaussian Splatting

**Tarun Gangadhar Vadaparthi**  
University at Buffalo, SUNY  

[📄 Project Report (PDF)](docs/PhysGSLite.pdf) 

Colab: 

[🌐 Project Website](https://<your-username>.github.io/phys-gs-lite/)  

---

## Abstract
Phys-GS Lite is a lightweight prototype that augments **3D Gaussian Splatting (3DGS)** with **semantic separation and physics-inspired dynamics**. Using simple geometry-driven heuristics, the method distinguishes between rigid and deformable regions (e.g., ship vs water). A sinusoidal wind field introduces wave-like deformation, while graph Laplacian smoothing ensures coherent motion.  

Unlike heavy neural pipelines, this approach is **lightweight, interpretable, and Colab-friendly**, showing that even simple physical cues can extend Gaussian Splatting towards dynamic, material-aware scenes.

---

## Method Overview
- **Semantic Labeling:** geometry heuristics (radial/z-thresholds + hull exclusion) to separate rigid vs deformable splats.  
- **Wind Deformation:** sinusoidal displacement modulated by vertical position.  
- **Laplacian Smoothing:** ensures spatially coherent wave-like motion.  
- **Visualization:** semantic view, close-up, orbit, and heatmap motion intensity.  

---

## Results
- Rigid structures (ship) remain static.  
- Water splats oscillate with realistic ripples.  
- Heatmaps show displacement intensity varies spatially.  
- Achieves visually convincing dynamics with **no fluid solver**.  

| Semantic View | Heatmap Motion |
|---------------|----------------|
| ![Semantic](docs/assets/semantic.png) | ![Heatmap](docs/assets/heatmap.png) |

---

## Demo
![Demo](docs/assets/demo.gif)

