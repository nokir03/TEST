```markdown
# Prerequisites

To run this code, you need Python installed on your computer. You can run the code using any Integrated Development Environment (IDE), such as VSCode, PyCharm, or others. The code can also be run from the terminal.

## Virtual Environment (optional)

A virtual environment (VENV) can be used when running the code. It is not mandatory. The following steps show how a VENV can be created. It is done by writing the presented lines in the terminal.

1. **Create the virtual environment:**

   ```
   python -m venv env
   ```

2. **Activate the virtual environment:**

   - Windows:
     ```
     .\env\Scripts\activate
     ```
   - Mac/Linux:
     ```
     source env/bin/activate
     ```

3. Next, install the required packages. After activating the virtual environment or even using one, install the necessary Python packages by running the following command:

   ```
   pip install numpy torch torchvision scikit-learn matplotlib seaborn tabulate
   ```

   If you are not using a virtual environment, ensure the packages are installed globally.

---

## Project Setup

1. Download the project from GitHub as a zip file and extract it. Once this is done, add the `src` and `datasets` folders to your work directory.

2. To test the code with full datasets, download the project datasets from the project guidelines PDF and add them to the `datasets` folder.

---

## Running the Code

1. Once the datasets are properly set up, you can run the code from the terminal. Navigate to the `data-exploration` directory by running:

   ```
   cd data-exploration
   ```

2. Run the following command:

   ```
   python DatasetsCleaning.py
   ```

   The code will generate a `processed` folder with all the processed images, as well as `.npz` files, which will be used for the rest of the code to speed up the process.

3. Once this is done, navigate to the `model-training` folder and run:

   ```
   python main.py
   ```

   This will train the model from scratch and add its `.pth` file to the `processed` folder.

4. To conduct tests, navigate to the folder containing the Python files needed to be run, and execute the following command in the terminal:

   ```
   python "name_of_python_file.py"
   ```
```
