# kmeans-ishihara-extractor

A Python-based tool that applies K-Means clustering to segment and extract numbers from Ishihara color blindness test images. This is useful for analyzing how color vision deficiencies affect number visibility by isolating color regions.

---

## 🔍 Overview

This tool segments the colors of an Ishihara image using unsupervised K-means clustering. The user selects the cluster(s) that visually contain the number, and the tool creates a binary mask to isolate and extract those regions.

---

## 🧠 How It Works

1. Load the image using PIL.
2. Flatten the image into RGB pixel vectors.
3. Apply K-Means clustering to group similar colors.
4. Display each color cluster separately for inspection.
5. Ask the user to input which clusters contain the number.
6. Merge selected clusters into a binary mask and display the result.

---

## 🖼️ Example Results

Below are four example outputs showing the original Ishihara image and the extracted number:

| Example | Original Image | Extracted Number |
|--------:|----------------|------------------|
| 1 | ![Example 1 Original](examples/12.jpg) | ![Example 1 Result](examples/12_extracted.png) |
| 2 | ![Example 2 Original](examples/6jpg)   | ![Example 2 Result](examples/6_extracted.png)  |
| 3 | ![Example 3 Original](examples/42.jpg) | ![Example 3 Result](examples/42_extracted.png) |
| 4 | ![Example 4 Original](examples/74.jpg) | ![Example 4 Result](examples/74_extracted.png) |
