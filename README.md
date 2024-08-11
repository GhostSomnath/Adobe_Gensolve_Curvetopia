# The Curve Enhancer Model

## Overview

The Curve Enhancer Model is the Adobe GenSolve project for our group, aimed at generating a model that can identify simple shape doodles. This project includes a well-structured setup process, ensuring ease of use and reproducibility. Users can clone the repository, set up a virtual environment, and manage datasets efficiently.

Key features of Curvetopia include:

- **Shape Identification:** Generate and train a model to identify and distinguish between simple shape doodles.
- **Data Management:** Easily manage and organize datasets using the designated `datasets` folder.
- **Virtual Environment:** Isolate project dependencies using a virtual environment.
- **Dependency Management:** Install necessary dependencies with a single command.
- **Cloud Integration:** Store and retrieve machine learning models using cloud storage solutions.

## Installation

Follow these steps to set up the project on your local machine.

### 1. Clone the Repository

then open the project folder


```bash
cd Adobe_Gensolve_Curvetopia

```

### 2. Create the 'datasets' Folder

Create a folder named **`datasets`** in the root directory of the project. This is where you will store the extracted ZIP files containing the datasets.

```bash
mkdir datasets
```

### 3. Create and Activate a Virtual Environment

Create a virtual environment to isolate the project's dependencies. Run the following command to create and activate the virtual environment:

For Windows:
```bash
python -m venv venv
venv\Scripts\activate
```

For Unix/macOS:
```bash
python3 -m venv venv
source venv/bin/activate
```

### 4. Extract the Datasets

Extract the dataset ZIP files into the **`datasets`** folder. Ensure that the structure is maintained as expected by the project.

```bash
unzip path/to/your_dataset.zip -d datasets/
```

### 5. Install Dependencies

Install the required dependencies for the project. This may involve using a package manager like **`pip`** for Python projects:

```bash
pip install -r requirements.txt
```

### To run this project, follow these steps:

1. **Set Up the Environment:**
    - Ensure you have Python installed. You can download it from [python.org](https://www.python.org/).
    - Install the required libraries. You can create a virtual environment and install the dependencies using `pip`.

    ```sh
    python -m venv venv
    venv\Scripts\activate  # On Windows
    pip install numpy opencv-python tensorflow scikit-learn
    ```

2. **Generate the Dataset:**
    - Run the [`generate_dataset.py`](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2FD%3A%2FSteeltroops%2FProgramming%2FCurvetopia%2Fsrc%2Fgenerate_dataset.py%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%5D "d:\Steeltroops\Programming\Curvetopia\src\generate_dataset.py") script to create the dataset of geometric shapes.

    ```sh
    python generate_dataset.py
    ```

3. **Train the Model:**
    - Run the [`model_creation_d.py`](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2FD%3A%2FSteeltroops%2FProgramming%2FCurvetopia%2Fsrc%2Fmodel_creation_d.py%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%5D "d:\Steeltroops\Programming\Curvetopia\src\model_creation_d.py") script to train the model on the generated dataset.

    ```sh
    python model_creation_d.py
    ```

4. **Test the Model:**
    - Run the [`test_model_d.py`](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2FD%3A%2FSteeltroops%2FProgramming%2FCurvetopia%2Fsrc%2Ftest_model_d.py%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%5D "d:\Steeltroops\Programming\Curvetopia\src\test_model_d.py") or [`test_model_dc.py`](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2FD%3A%2FSteeltroops%2FProgramming%2FCurvetopia%2Fsrc%2Ftest_model_dc.py%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%5D "d:\Steeltroops\Programming\Curvetopia\src\test_model_dc.py") script to test the model with a user-provided image.

    ```sh
    python test_model_d.py
    # or
    python test_model_dc.py
    ```

5. **View the Results:**
    - The script will display the image with the predicted class.

Make sure to replace the paths in the scripts with the correct paths to your dataset and model files if they differ.
