#  Vehicle Edge Detection using Sobel & Canny Filters

This project applies Sobel and Canny edge detection techniques to vehicle images to enhance features such as license plate contours. The implementation is inspired by the scientific research paper titled:

 **"Automatic Number Plate Recognition of Saudi License Car Plates" (ETASR, Vol. 12, No. 2, 2022)**  
 [Paper Included](./Automatic_Number_Plate_Recognition_of_Saudi_License_Car_Plates.pdf)




---

##  Techniques Used

- **Sobel Edge Detection**: For gradient-based edge enhancement
- **Canny Edge Detection**: For precise contour detection using automatic thresholding
- **Gaussian Blur**: To reduce noise before applying edge detection
- **OpenCV**: For image processing and operations
- **Jupyter Notebook**: To visualize and document results interactively

---

##  Dataset Privacy

The dataset contains sensitive vehicle images that are not included in this repository.  
The `results/` directory contains **50 sample images of Saudi vehicle license plates**, demonstrating edge detection results using both Sobel and Canny methods.

---

##  How to Run

```bash
pip install -r requirements.txt
jupyter notebook notebooks/edge_detection.ipynb
```

---

##  Research Background: Use of Sobel & Canny

This project is directly inspired by the research titled:

**"Automatic Number Plate Recognition of Saudi License Car Plates"**  
 Published in: *Engineering, Technology & Applied Science Research (ETASR)*, Vol. 12, No. 2, 2022  


###  Sobel & Canny in the Study

The study uses classical edge detection methods to identify and isolate license plates:

- **Canny Edge Detection** was used to **locate the license plate region** using Otsu’s thresholding to dynamically define sensitivity.
- **Sobel Edge Detection** was used for **highlighting gradient-based structures** inside the plate such as the borders and text, playing a key role in character segmentation.

These methods were validated and shown to be effective for structured license plate formats in Saudi Arabia.

###  Code Reference

```python
from src.sobel_filter import sobel, canny

sobel_edges = sobel(img, L2gradient=True)
canny_edges = canny(img, L2gradient=True)
```

The results are shown visually in the notebook using side-by-side comparisons.

---

##  Requirements

All libraries can be installed via:

```bash
pip install -r requirements.txt
```

Libraries:
- opencv-python
- numpy
- pillow
- jupyter
- matplotlib

---

 [Download Full Paper (PDF)](./Automatic_Number_Plate_Recognition_of_Saudi_License_Car_Plates.pdf)
