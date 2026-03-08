# Spatial Image Filtering

Digital Image Processing project exploring spatial filtering techniques for image smoothing and noise reduction.

The project implements several spatial filters from scratch, including averaging, Gaussian, and median filters, as well as a user-defined filter. The effects of different filters and kernel sizes are evaluated on multiple images.

---

# Project Structure

```
spatial-image-filtering/
│
├── notebooks/
│   └── spatial_filtering.ipynb
│
├── data/
│   └── example images are placed here
│
└── README.md
```

---

# Project Overview

Spatial filtering is a fundamental technique in digital image processing used to modify images by applying operations to pixel neighbourhoods.

Filters can be used for:

- noise reduction
- image smoothing
- edge preservation
- image enhancement

This project implements several spatial filtering methods manually and evaluates their performance on different images.

---

# Implemented Filters

The following filters are implemented.

---

## 1. Averaging (Mean) Filter

The averaging filter replaces each pixel value with the average value of its neighbouring pixels.

The filter helps smooth the image by reducing local intensity variations.

Different filter sizes are tested to observe how the amount of smoothing changes.

---

## 2. Gaussian Filter

The Gaussian filter performs weighted smoothing using a Gaussian kernel.

Compared to a simple averaging filter, the Gaussian filter gives more importance to pixels closer to the centre of the neighbourhood.

This often results in smoother images while preserving important structures better than simple averaging.

---

## 3. Median Filter

The median filter replaces each pixel with the median value of its neighbourhood.

This filter is particularly effective for removing **salt-and-pepper noise** while preserving edges.

---

## 4. Custom Filter

The user can define a custom **3×3 filter kernel**.

This allows experimentation with different spatial filters and provides insight into how kernel values influence the output image.

---

# Edge Handling

When applying spatial filters near the image borders, neighbouring pixels may fall outside the image.

Different edge-handling strategies are implemented, including:

- zero padding
- other padding strategies

These methods determine how pixel values outside the image boundaries are treated.

---

# Results and Evaluation

The filters are tested on multiple images in order to evaluate their effectiveness.

Observations include:

- Averaging filters reduce noise but can blur important image details.
- Gaussian filters provide smoother results with better preservation of structures.
- Median filters are especially effective for removing impulse noise.
- Custom filters allow experimentation with different neighbourhood operations.

---

# Technologies Used

- Python
- NumPy
- OpenCV
- Matplotlib
- Jupyter Notebook

---

# Running the Project

Clone the repository:

```
git clone <repository-url>
```

Install dependencies:

```
pip install numpy opencv-python matplotlib
```

Launch Jupyter Notebook:

```
jupyter notebook
```

Open and run:

```
notebooks/spatial_filtering.ipynb
```

---

# Concepts Demonstrated

This project demonstrates several key image processing techniques:

- spatial filtering
- neighbourhood operations
- image smoothing
- noise reduction
- edge handling strategies
