# Interactive Heatmap Data Visualization Exercise

This project demonstrates how to build an **interactive CT‑scan contour heatmap** using D3.js. Drawing inspiration from the eye‑tracking heatmap example, you’ll learn to:

- Load and parse flat CSV data of CT scan intensities  
- Generate contour levels with variable bin counts  
- Apply a real‑time slider filter to exclude low‑intensity regions  

## Features

1. **Dynamic Binning**  
   Adjust the number of contour levels on the fly to explore fine‑ and coarse‑grained structures.  
2. **Intensity Thresholding**  
   Use a slider to set a minimum intensity cutoff—automatically hides all contours below your threshold.  
3. **Diverging Color Scale**  
   Seamlessly transition from blue (low) → white (mid) → red (high) intensities via D3’s `interpolateRdBu`.  
4. **Offline‑Capable**  
   Runs entirely in the browser with a local copy of `d3.js`; no external dependencies.

## Getting Started

1. **Clone the repo**  
   ```bash
   git clone https://github.com/umassdgithub/Week-12-Contours.git
   cd Week-12-Contours/Major-Assignment-4

```
        const contours = d3.contours()
            .size([m, n])
                .thresholds(d3.range(min,max,bin_counts))
                (values_T);
```
5. Use colorScale based on the following code  (10 points)
```
THIS IS A SAMPLE:
        const colorScale = d3.scaleDiverging()
            .domain([min, mid, max])
            .interpolator(d3.interpolateRdBu);
```


<img src='./Screenshot 2025-04-21 at 13.54.29.png' width='400px' />
