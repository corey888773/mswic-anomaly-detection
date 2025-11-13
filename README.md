# mswic-anomaly-detection

Network Intrusion Detection using Machine Learning - DDoS Attack Detection

## Setup

### Virtual Environment

Create and activate virtual environment:

```bash
# Create virtual environment
python3 -m venv venv

# Activate virtual environment
# On macOS/Linux:
source venv/bin/activate

# On Windows:
venv\Scripts\activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Deactivate Virtual Environment

```bash
deactivate
```

## Project Structure

- `project.ipynb` - Main Jupyter notebook with data preprocessing pipeline
- `data.csv` - Network intrusion dataset (CICIDS2017)
- `requirements.txt` - Python dependencies
- `venv/` - Virtual environment (not tracked in git)

## Dataset

- **Source**: CICIDS2017 Network Intrusion Dataset
- **Records**: 225,745
- **Features**: 78 + 1 label
- **Classes**: DDoS, BENIGN
- **Task**: Binary classification for DDoS detection