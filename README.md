**Feature extraction from tumor slides in cancer**


### **Introduction**
Certain genetic mutations and features in tumor cells can help predict how well a patient might respond to therapies like immunotherapy. Two areas of focus in this research are tumor mutational burden (TMB) and POLE mutation.

**Tumor mutational burden** refers to the total number of mutations found in a tumor. Tumors with a high TMB often create more neoantigens. **Neoantigens** are new proteins produced by mutated cells, and they can trigger the immune system to attack the tumor. 

POLE mutations are changes in a gene that helps repair DNA in cells. Tumors with POLE mutations usually have many mutations across their DNA and may produce more neoantigens. These features make them good candidates for immunotherapy. 

Histopathology images are digital scans of tissue samples taken from tumors. These images contain a lot of information about the structure, color, and shape of cells in the tissue. It is possible to analyze features like texture (the way cells are organized), color (variations in staining), and morphology (the shapes of cells and structures) to understand how tumors behave. For example, specific patterns in these features may be linked to POLE mutations or neoantigen production. 

This project focuses on extracting and analyzing features from histopathology images to connect these visual patterns with genetic and immunological markers. By studying these features, we aim to better understand how visual information from tissue slides can help predict important tumor characteristics like neoantigen count and POLE mutations.

### **Objective**

The objective of this project is to extract features from histopathology slides of tumor and explore their potential to predict:  

1. Neoantigen counts
2. POLE mutations
3. Tumor mutational burden


### **Steps**

1. **Literature Review**  
   - Review existing research on visual features (texture, color, morphology) commonly analyzed in tissue slides.  
   - Explore machine learning models used for feature extraction from tissue slides.  
   - Investigate the role of these features in cancers with MSI classification.  

2. **Data Preparation**  
   - Download and preprocess histopathology images from TCGA.  

3. **Feature Extraction**  
   - Implement algorithms to extract features, such as texture, color distributions, and morphological descriptors.  

4. **Feature Analysis**  
   - Test for significant visual patterns linked to POLE mutations.  
   - Explore correlations between extracted features and neoantigen counts.
# TCGA-COAD slides
The diagnostic slide images from TCGA are quite large and stored in **SVS format**, which contains high-resolution pathology images. 

To analyse locally, I created a **subset of tumor slides**, converted them to PNG format, and uploaded them to Google Drive for easier access. You can download the subset from the following link:

[Download PNG subset](https://drive.google.com/file/d/1ZP-sRfEzg9YKTQu-9H6PNP3HyNNF2Bdk/view?usp=sharing)

## Downloading Diagnostic Slide Images from TCGA

### Step 1: Create a Cohort
1. Go to the [GDC Data Portal](https://portal.gdc.cancer.gov/).
2. Select **"Colorectal"** as the cancer type. This will create a new cohort.

![Creating a Cohort](img/screen1.png)

3. Save your cohort by clicking the save button as shown in the screenshots.

![Saving a Cohort](img/screen2.png)

### Step 2: Select Diagnostic Slide Images
1. Navigate to the [Repository](https://portal.gdc.cancer.gov/analysis_page?app=Downloads) page.
2. Ensure that you are working with the **Colorectal cohort**.
3. In the **Filters** section, locate the "Experimental Strategy" panel.
4. Select **"Diagnostic Slide"**.

![Saving a Cohort](img/screen3.png)

### Step 3: Add Files to Cart
1. Click **"Add All Files to Cart"** to add the selected images.
2. Navigate to your cart by clicking on the cart icon in the top-right corner.

### Step 4: Downloading Large Data
1. Since the dataset is large, it is recommended to use the **GDC Data Transfer Tool**.
2. Download the tool from [GDC Data Transfer Tool](https://gdc.cancer.gov/access-data/gdc-data-transfer-tool).
3. Follow the instructions provided by GDC to download your selected images efficiently.



