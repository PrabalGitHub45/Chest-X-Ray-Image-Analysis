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
