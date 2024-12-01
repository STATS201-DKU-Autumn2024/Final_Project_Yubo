# Data Folder

## Data Source Description

The datasets used in this project focus on detecting AI-generated fake restaurant reviews. The primary goal of these datasets is to provide a benchmark for distinguishing between authentic and machine-generated restaurant reviews, using both textual and visual data. The data consists of text-based reviews paired with corresponding images of restaurant dishes. These datasets serve as the foundation for training and evaluating machine learning models for fake review detection.

The datasets were sourced from the [AiGen-FoodReview dataset](https://github.com/iamalegambetti/aigen-foodreview), a publicly available multimodal dataset. The dataset consists of 20,144 review-image pairs, with labels indicating whether a review is authentic (0) or machine-generated (1). This dataset is hosted on GitHub and is available for use in research on fake review detection.

For the images, you can download them from the following link:  
[Download Images](https://drive.google.com/drive/folders/1z-lXVUVl5EdNPnAXMq2KPWfA4_BmZCp3?usp=sharing)

## Data Dictionary

Below is the structured data dictionary for the datasets used in this project:

| Variable        | Type           | Description                                                                 |
|-----------------|----------------|-----------------------------------------------------------------------------|
| **ID**          | Integer        | Unique identifier for each review-image pair.                               |
| **text**        | String         | The text content of the restaurant review.                                   |
| **label**       | Integer (0/1)   | Label indicating whether the review is authentic (0) or machine-generated (1). |
| **image**       | File (.jpg)     | Image file corresponding to the review, depicting the restaurant dish.       |

### Notes:
- The **ID** is a unique identifier used to link the review text and the corresponding image.
- **text** contains the full review text for each restaurant entry.
- The **label** column helps differentiate between authentic and machine-generated reviews (0 for authentic, 1 for machine-generated).
- The **image** column refers to the image file associated with the review text, and the images are stored in the `images/` folder.

This dataset will be used to train and evaluate models for fake review detection across different modalities (text and image).
