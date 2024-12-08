# How to Run the Code

## Prerequisites

To run this code, you need Python installed on your computer. You can execute the code using any Integrated Development Environment (IDE), such as **VSCode**, **PyCharm**, or others. The code can also be run directly from the terminal.


## Virtual Environment (Optional)

A virtual environment (VENV) can be used when running the code. While it is not mandatory, it is recommended for managing dependencies. Follow these steps to create a virtual environment:

### Step 1: Create the Virtual Environment

```bash
python -m venv env
```


### Step 2: Activate the Virtual Environment

#### Windows:

```bash
.\env\Scripts\activate
```

#### Mac/Linux:

```bash
source env/bin/activate
```


## Installing Required Packages

After activating the virtual environment (or if you’re not using one), install the necessary Python packages by running the following command:

```bash
pip install numpy torch torchvision scikit-learn matplotlib seaborn tabulate
```

If you are not using a virtual environment, ensure the packages are installed globally.

---

## Setting Up the Project

1. **Download the Project**: Download the project from GitHub as a ZIP file and extract it.
2. **Add Required Folders**: Place the **`src`** and **`datasets`** folders in your working directory.
3. **Set Up Datasets**: To test the code with full datasets, download the datasets from the **project guidelines PDF** and add them to the **`datasets`** folder.

---

## Running the Code

### Step 1: Data Cleaning

Navigate to the `data-exploration` directory and run the following command in your terminal:

```bash
cd data-exploration
python DatasetsCleaning.py
```

This will generate a `processed` folder containing all the processed images and `.npz` files. These files will be used in subsequent steps to speed up processing.

### Step 2: Model Training

Once the data is processed, navigate to the `model-training` folder and run the following command:

```bash
cd ../model-training
python main.py
```

This command will train the model from scratch and generate a `.pth` file in the `processed` folder.

### Step 3: Conducting Tests

After training the model, navigate to the folder containing the required Python scripts for testing. Run the desired script using the following command:

```bash
python "name_of_python_file.py"
```

Replace **`name_of_python_file.py`** with the actual file name you wish to execute.
