# Chest X-Ray Image Analysis

## Overview

This Streamlit app analyzes chest X-ray images to detect potential abnormalities using a pre-trained DenseNet121 model. It provides a user-friendly interface for uploading and processing images, and it visualizes predictions with Grad-CAM.

Check out the live Streamlit App [here](https://chestxrayanalysis.streamlit.app).

Image from the web:

<img src="https://lh3.googleusercontent.com/pw/AP1GczMnFxVlt5xk6Y6TZDPwgmu6u3iHnCo4idmkvsfUC2KZ9qFt7ezq-8GvalO7esUBbmNShqQwIygRHDmA5BfZiZQnxMVvCX8XdIR_XgjCk_CloWPsIygo=w2400" alt="alt text" width="400" />
<img src="https://lh3.googleusercontent.com/pw/AP1GczMV9bbE7wXN5UKj2Ve_NhVG_LrcApL8e9JuX5tznZgtVOFubmUP1vcZqhr2xrQO3iguagnPZ7WHTiuzgkVqBABekPqRPxBKC5PHUkSNl0Mso_94ywE4=w2400" alt="alt text" width="400" />

## Features

- **Image Upload**: Accepts chest X-ray images in JPG, JPEG, or PNG format.
- **Abnormality Detection**: Uses a machine learning model to predict the probability of 14 different conditions.
- **Grad-CAM Visualization**: Highlights areas of the image most relevant to the model's predictions.
- **Interactive Interface**: Built with Streamlit for easy and intuitive use.

## Important Notes

- This tool is for educational purposes only.
- It is not a substitute for professional medical advice or diagnosis.
- Ensure you upload only chest X-ray images for accurate results.

## Instructions

1. **Upload a Chest X-Ray Image**: Click on the "Upload a chest X-ray image" button and select an image file.
2. **View the Results**: The app will display the uploaded image, prediction results, and Grad-CAM visualizations.
3. **Explore Further**: Visit the portfolio and source code repository for more projects and insights.

## How to Run Locally

1. Clone this repository:

    ```bash
    git clone https://github.com/kimnguyen2002/Chest-X-Ray-Image-Analysis.git
    ```

2. Navigate to the project directory:

    ```bash
    cd Chest-X-Ray-Image-Analysis
    ```

3. Install the required packages:

    ```bash
    pip install -r requirements.txt
    ```

4. Run the Streamlit app:

    ```bash
    streamlit run app.py
    ```

## Datasets
The dataset includes approximately 1,000 chest X-ray images. This project is based on the [ChestX-ray8 datasets](https://arxiv.org/abs/1705.02315), which contains 108,948 frontal-view
X-ray images of 32,717 unique patients, you could download the entire dataset [here](https://nihcc.app.box.com/v/ChestXray-NIHCC). These images are accompanied by a CSV file containing the corresponding labels for each X-ray. To facilitate use, a processed subset of the data and labels has been provided, organized into three separate files:

- `/train-small.csv`: Contains 875 images intended for training.
- `/valid-small.csv`: Contains 109 images intended for validation.
- `/test.csv`: Contains 420 images intended for testing.

This subset has been annotated through consensus among four radiologists for five of the 14 possible pathologies:

- Consolidation

- Edema

- Effusion

- Cardiomegaly

- Atelectasis

The folder path for accessing the images is stored in the `IMAGE_DIR` variable. This structure ensures ease of use when loading and processing the dataset.

## Model Details

The model is based on DenseNet121 and is trained to identify 14 conditions:

- Cardiomegaly
- Emphysema
- Effusion
- Hernia
- Infiltration
- Mass
- Nodule
- Atelectasis
- Pneumothorax
- Pleural Thickening
- Pneumonia
- Fibrosis
- Edema
- Consolidation

## Acknowledgments
This project was made possible thanks to the **AI for Medical Diagnosis** course by Andrew Ng on Coursera. The course provided the foundation for understanding key concepts and introduced the pre-trained model used in this project. While the pre-trained DenseNet121 model and dataset processing stem from the course materials, the focus of this project is on building an interactive web application to make these insights more accessible and intuitive for users.

## Disclaimer
This project is intended solely for **educational and research purposes**. It is **NOT a substitute for professional medical advice, diagnosis, or treatment**. Results produced by the model should not be used for clinical decision-making or as a definitive diagnostic tool. Always consult a qualified healthcare professional for medical concerns.

## License

This project is licensed under the MIT License.

Feel free to adjust the structure to fit your actual project layout!
