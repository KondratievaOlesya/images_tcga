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
