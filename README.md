# Agentic AI Projects Repository

This repository contains all the code and projects related to my journey in learning and implementing Agentic AI. It serves as a centralized location for personal projects, notes, and experimental setups.

---

## Project Structure

The repository is organized as follows:

- **Main Folder:** Contains common files shared across all projects:
  - `.env`: Stores environment variables like API keys.
  - `requirements.txt`: Lists all Python dependencies for the projects.
- **Project Folders:** Each project has its own folder with a similar structure:
  - Code files specific to the project.
  - Subdirectories for modules, scripts, or additional data as needed.

---

## GenAI Project Setup

### 1. Installing Anaconda and Setting Up the Environment

To set up the Python environment:

```bash
conda create -p venv python==3.12
```

- **Note**: `-p` creates the environment in the same folder.

Activate the environment using one of the following methods:

```bash
conda activate venv/
```

or

```bash
conda activate /path/to/your/venv
```

---

### 2. Create `requirements.txt` and `.env` File

Install dependencies from the `requirements.txt` file:

```bash
pip install -r requirements.txt
```

#### Add API Keys into `.env`

Define the following API keys in your `.env` file:

- `GROQ_API_KEY` : Obtain it from the GROQ website.
- `PHI_API_KEY` : Obtain it from the PHI Data website.
- `OPENAI_API_KEY` : Your OpenAI API key.

#### For Temporary Keys in the Session (Mac):

```bash
export GROQ_API_KEY="your_groq_api_key"
export PHI_API_KEY="your_phi_api_key"
export OPENAI_API_KEY="your_openai_api_key"
```

#### For Temporary Keys in the Session (Windows):

```bash
setx GROQ_API_KEY "your_groq_api_key"
setx PHI_API_KEY "your_phi_api_key"
setx OPENAI_API_KEY "your_openai_api_key"
```

#### To Persist API Keys in the Conda Environment:

```bash
conda env config vars set MY_API_KEY="your_api_key_here"
conda env config vars list
```

---

### 3. Running a Project

To run a specific project, navigate to its folder and execute the relevant script. For example:

```bash
cd project-folder
python playground.py
```

---

### 4. Using the PHI Data Playground

The PHI Data Playground is an interactive UI where you can test and visualize your agent applications. After running the project script (e.g., `playground.py`), note the port number displayed in the terminal (e.g., `LOCALHOST:7777`). Use this port number in the PHI Data Playground section to connect and interact with your application.

---

### Notes

- The `.env` file and `requirements.txt` are shared across all projects and are located in the main folder.
- Feel free to modify and extend the setup as needed for individual projects.

Happy experimenting with Agentic AI!

