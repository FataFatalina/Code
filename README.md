# <span style="color: #007bff;">Data Science Classification Engine - Project Overview</span>

## <span style="color: #28a745;">Project Description:</span>
- **Objective**: Feasibility study for a classification engine using both text and image data.
- **Dataset**: A dataset with 1,050 rows and 3 columns (descriptions, product categories, image names).
- **Target Categories**: 
  - Home furnishing
  - Baby care
  - Watches
  - Home decor & festive needs
  - Kitchen & dining
  - Beauty and personal care
  - Computers

## <span style="color: #28a745;">Data Preprocessing:</span>
### <span style="color: #17a2b8;">Text Preprocessing:</span>
- Removal of **special characters**, **numbers**, and **stopwords**.
- **Lemmatization**: Converted words to their canonical form.

### <span style="color: #17a2b8;">Image Preprocessing:</span>
- **Feature Extraction** from images using **ORB**.
- **Histogram computation** and dimensionality reduction with **PCA**.

## <span style="color: #28a745;">Feature Extraction & Clustering:</span>
### <span style="color: #17a2b8;">Text Data:</span>
- **Feature extraction**: Text data processed and prepared for analysis.
- **Dimensionality Reduction**: Applied techniques like PCA for feature space reduction.
- **Clustering**: **KMeans** used for clustering product categories.

### <span style="color: #17a2b8;">Image Data:</span>
- **ORB Feature Extraction**: Extracted features from images for clustering.
- **ResNet50 CNN Model**: Used to extract image features with a pre-trained CNN model.
- **Dimensionality Reduction**: Applied **PCA** and **Isomap** for feature reduction.
- **KMeans Clustering**: Categorized images based on extracted features.
- **Similarity Calculation**: Used **Adjusted Rand Index (ARI)** to calculate the similarity between predicted clusters and original categories.

## <span style="color: #28a745;">Model Evaluation:</span>
- Calculated the **Adjusted Rand Index (ARI)** to measure the similarity between actual product categories and those assigned by the clustering model.

## <span style="color: #28a745;">Conclusion:</span>
- **Feasibility**: The project demonstrated the feasibility of creating a classification engine using both text and image data.
- **Results**: Preliminary clustering results show potential for classification with further refinement.

## <span style="color: #28a745;">Libraries & Tools Used:</span>
- **Python**, **pandas**, **scikit-learn**, **KMeans**, **ResNet50**, **ORB**, **PCA**, **Isomap**, **Matplotlib**, **Seaborn**.
