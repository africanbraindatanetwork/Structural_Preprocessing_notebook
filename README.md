# Structural Preprocessing Notebooks

## Overview

This repository contains a comprehensive set of Jupyter notebooks for preprocessing structural MRI (Magnetic Resonance Imaging) data. The notebooks are designed to guide users through the entire preprocessing pipeline, from raw MRI data to analysis-ready structural images.

## Description

Structural MRI preprocessing is a critical step in neuroimaging research that prepares raw brain imaging data for subsequent analysis. This collection of notebooks provides a step-by-step workflow that covers:

- **Data preparation and organization**: Setting up your neuroimaging data in standardized formats
- **Quality control**: Assessing image quality and identifying potential artifacts
- **Preprocessing pipeline**: Implementing standard preprocessing steps including:
  - Skull stripping and brain extraction
  - Bias field correction
  - Image registration and normalization
  - Tissue segmentation (gray matter, white matter, CSF)
  - Spatial normalization to standard templates

## Notebooks

The preprocessing workflow is divided into three parts:

1. **mri_preprocessing_colab_part1.ipynb**: Initial setup, data loading, and quality assessment
2. **mri_preprocessing_colab_part2.ipynb**: Core preprocessing steps and transformations
3. **mri_preprocessing_colab_part3.ipynb**: Advanced processing, segmentation, and final output generation

## Prerequisites

Before you begin, you'll need to install the following software on your computer:

### 1. Python Installation

Download and install Python 3.7 or higher:
- **Windows/macOS/Linux**: Visit [python.org](https://www.python.org/downloads/) and download the latest Python installer
- During installation, make sure to check "Add Python to PATH"
- Verify installation by opening a terminal/command prompt and typing:
  ```bash
  python --version
  ```

### 2. Visual Studio Code (Recommended)

VS Code provides an excellent environment for working with Jupyter notebooks:
- Download from [code.visualstudio.com](https://code.visualstudio.com/)
- Install the following VS Code extensions:
  - **Python** (by Microsoft)
  - **Jupyter** (by Microsoft)
  - **Pylance** (by Microsoft)

To install extensions:
1. Open VS Code
2. Click the Extensions icon in the sidebar (or press `Cmd+Shift+X` on macOS / `Ctrl+Shift+X` on Windows)
3. Search for each extension and click "Install"

### 3. Git (for cloning the repository)

- **macOS**: Git is pre-installed. Verify by typing `git --version` in Terminal
- **Windows**: Download from [git-scm.com](https://git-scm.com/downloads)
- **Linux**: Install via package manager (e.g., `sudo apt-get install git`)

### Alternative: Google Colab (No Installation Required)

If you prefer not to install software locally, you can run these notebooks directly in [Google Colab](https://colab.research.google.com/):
- Requires only a Google account
- Provides free access to computational resources
- Simply upload the notebooks to Google Drive and open with Colab

## Requirements

- Python 3.7+
- Jupyter Notebook or Google Colab
- Neuroimaging libraries (specific dependencies listed in each notebook)

## Getting Started

### Option 1: Local Setup (VS Code)

1. Clone this repository:
   ```bash
   git clone <repository-url>
   cd structuralpreprocessingnotebooks
   ```

2. Open the folder in VS Code:
   ```bash
   code .
   ```
   Or open VS Code and use `File > Open Folder` to select the `structuralpreprocessingnotebooks` directory

3. Set up a virtual environment (recommended):
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On macOS/Linux
   # On Windows: .venv\Scripts\activate
   ```

4. Install required dependencies (see individual notebooks for specific requirements)

5. Open the notebooks in VS Code:
   - Click on any `.ipynb` file in the Explorer sidebar
   - VS Code will prompt you to select a Python kernel
   - Choose the Python interpreter from your `.venv` virtual environment

6. Run the notebooks in order, starting with Part 1

### Option 2: Google Colab Setup

1. Upload the notebook files to your Google Drive
2. Right-click on a notebook file and select `Open with > Google Colaboratory`
3. Follow the instructions in each notebook to install dependencies
4. Run cells sequentially

## Usage

Each notebook contains:
- Detailed explanations of preprocessing concepts
- Code cells with preprocessing implementations
- Visualization of results at each step
- Quality control checkpoints

Follow the notebooks sequentially for the complete preprocessing pipeline, or use individual sections as needed for specific preprocessing tasks.

## Notes

- These notebooks are designed to work in Google Colab for easy access to computational resources
- Sample data requirements and formats are specified in Part 1
- Processing time will vary depending on data size and computational resources

