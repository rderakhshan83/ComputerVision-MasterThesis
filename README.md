# Master Thesis: Body Rumen Fill Scoring of Dairy Cows Using Digital Images

## Authors:
- Reza Derakhshan
- Soroush Yousefzadeh Boroujeni

## University:
Dalarna University, Borlänge

## Supervisor:
- Moudud Alam
- Co-supervisors: Niclas Högberg, Louise Winblad von Walter  
- Examiner: Mia Xiaoyun Zhao

## Abstract:
This thesis explores the automation of **rumen fill scoring** in dairy cows using **digital image processing** and **machine learning** techniques. The goal was to develop a system to automate the annotation and evaluation of rumen fill status based on images extracted from videos recorded on a Swedish dairy farm. By using **Logistic Regression**, **Support Vector Machines (SVM)**, and **Deep Neural Networks (VGG16)**, we aimed to replicate the manual rumen fill scoring traditionally performed by veterinarians. The study highlights the potential of automated scoring to improve farm efficiency, cow health monitoring, and sustainability in dairy production.

### Key Contributions:
- Developed and tested several machine learning models for image-based rumen fill scoring.
- Achieved moderate accuracy with the Logistic Regression model outperforming more complex models like VGG16.
- Identified limitations such as dataset imbalance and environmental factors affecting image quality, providing a roadmap for future improvements.

## Technologies:
- **Machine Learning**: Logistic Regression, SVM, and VGG16 Neural Network.
- **Data Processing**: Python, TensorFlow, Keras, and scikit-learn.
- **Image Processing**: Manual annotation and processing of 277 images.

## Results:
The study found that while machine learning models show promise, there is room for improvement in model accuracy, especially by expanding the dataset and using advanced feature engineering.

## Dataset:
The dataset used for this study is available in the repository under `DataSet.zip`. It contains the manually annotated images of dairy cows used for training and testing the machine learning models.

## Code:
The code for the thesis is provided in the `MasterThesis.ipynb` Jupyter Notebook. The notebook contains scripts for:
- **Preprocessing images**: cropping and resizing.
- **Training machine learning models**: Logistic Regression, SVM, and VGG16.
- **Evaluating model performance**: using metrics like accuracy, precision, recall, and F1-score.

## How to Use:
1. **Clone the repository**:
    ```bash
    git clone https://github.com/your-repository-url.git
    cd your-repository
    ```

2. **Unzip the dataset**:
    ```bash
    unzip DataSet.zip
    ```

3. **Install dependencies**:
    Ensure that you have Python installed and run the following command to install the necessary packages:
    ```bash
    pip install -r requirements.txt
    ```

4. **Run the Jupyter Notebook**:
    Open the `MasterThesis.ipynb` notebook using Jupyter and run the cells to preprocess the images, train the models, and evaluate the results.
    ```bash
    jupyter notebook MasterThesis.ipynb
    ```

5. **Dataset Overview**:
    The dataset includes:
    - **Training images**: Located in the `train/` directory.
    - **Testing images**: Located in the `test/` directory.
    - **Labels**: The labels are provided in `labels.csv`.

6. **Configuration**:
    - Hyperparameters for each model can be adjusted in the corresponding cells in the notebook.

## Results:
The notebook will output model performance metrics, including accuracy, precision, recall, and F1-score, for each of the models.

## Future Work:
Further research could explore improved image augmentation techniques, include more diverse datasets, and refine model architectures to achieve higher accuracy and better generalization.

## License:
This project is licensed under the MIT License.
