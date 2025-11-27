# mswic-anomaly-detection

Network Intrusion Detection using Machine Learning - DDoS Attack Detection

## Prerequisites

### Git LFS

This project uses Git LFS for large files (dataset). Install Git LFS before cloning:

```bash
# macOS
brew install git-lfs

# Ubuntu/Debian
sudo apt-get install git-lfs

# Windows
# Download from https://git-lfs.github.com/
```

After installation, initialize Git LFS:

```bash
git lfs install
```

### Clone Repository

```bash
git clone <repository-url>
cd mswic-anomaly-detection

# Pull LFS files
git lfs pull
```

## Setup

### Option 1: Virtual Environment (venv)

Create and activate virtual environment:

```bash
# Create virtual environment
python3 -m venv venv

# Activate virtual environment
# On macOS/Linux:
source venv/bin/activate

# On Windows:
venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

### Option 2: Conda

```bash
# Create conda environment
conda create -n mswic python=3.12

# Activate environment
conda activate mswic

# Install dependencies
pip install -r requirements.txt
```

### Deactivate Environment

```bash
# For venv:
deactivate

# For conda:
conda deactivate
```

## Project Structure

- `project.ipynb` - Main Jupyter notebook with complete ML pipeline
- `data.csv` - Network intrusion dataset (CICIDS2017) - **stored in Git LFS**
- `requirements.txt` - Python dependencies
- `venv/` - Virtual environment (not tracked in git)

## Dataset

- **Source**: CICIDS2017 Network Intrusion Dataset
- **Records**: 225,745
- **Features**: 78 + 1 label
- **Classes**: DDoS, BENIGN
- **Task**: Binary classification for DDoS detection
- **Size**: ~74 MB (stored in Git LFS)

## Running the Project

1. Make sure you have activated your environment (venv or conda)
2. Open Jupyter Notebook:
   ```bash
   jupyter notebook project.ipynb
   ```
3. Run all cells to:
   - Load and preprocess data
   - Train models (Random Forest, Logistic Regression)
   - Evaluate and compare results