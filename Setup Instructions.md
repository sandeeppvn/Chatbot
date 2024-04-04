
# Workshop Setup Instructions

This README provides detailed instructions for setting up your environment for the workshop. Follow these steps carefully to ensure everything is correctly installed and configured.

## Step 0: Setup VSCode

1. **Create a new folder** - This will be your working directory.
2. **Open VSCode** - Launch Visual Studio Code.
3. **Open the Folder** - Go to `File > Open Folder` and select the newly created folder.

## Step 1: Setup GitHub

1. **Create requirements.txt** - Similarly, create a `requirements.txt` file and fill it with the following content:
    ```
    langchain
    python_dotenv
    cohere
    pypdf
    langchain-cohere
    faiss-cpu
    ```
3. **Publish to GitHub** - Use `Ctrl + Shift + P` > `Publish to GitHub`. Provide the repository name and ensure it is public.
4. **Configure Git** - Open the terminal in VSCode and run:
    ```
    git config --global user.email "you@example.com"
    git config --global user.name "Your Name"
    ```
5. **Link Repository** - Use `Ctrl + Shift + P` > `Git: Add Remote`, and link it to the same name as the folder.
6. **Initial Commit** - In VS Code, click on source control, provide the commit message as “Initial Commit” and click commit and push.

## Step 2: Create Python Virtual Environment

1. **Create Virtual Environment** - In the Terminal, run:
    ```
    python -m venv .venv
    ```
2. **Provide Permissions** (Windows) - Run:
    ```
    Set-ExecutionPolicy -ExecutionPolicy Unrestricted -Scope Process
    ```
3. **Activate the Environment** - Execute:
    ```
    .\.venv\Scriptsctivate
    ```
4. **Upgrade pip** - Run:
    ```
    python -m pip install --upgrade pip
    ```
5. **Install Requirements** - Install the required modules with:
    ```
    pip install -r ./requirements.txt
    ```
6. **Select Python Interpreter** - Use `Ctrl + Shift + P` > `Python: Select Interpreter`, and select `.venv`.

## Step 3: Setup Coherence API Key

1. **Create Account** - Go to [Cohere](https://cohere.ai/) and create an account.
2. **Get API Key** - Go to the dashboard and copy the API key.
3. **Create .env File** - Use `Ctrl + Shift + P` > `Create: New File` and name it `.env`.
2. **Add API Key** - In the `.env` file add:
    ```
    COHERE_API_KEY="<api_key>"
    ```

## Step 4: Load the PDFs

1. **Create Data Folder** - Create a new folder and name it `data`.
2. **Add PDFs** - Place one or more PDFs in the `data` folder.

## Step 5: Test Notebook

1. **Open Jupyter Notebook** - Open the jupyter notebook `assigment.ipynb`.


Follow these steps carefully to ensure your workshop environment is properly set up. Enjoy the workshop!
