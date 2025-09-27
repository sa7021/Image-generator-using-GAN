# 🎨 Raja Ravi Varma Image Generator

This project is an **AI-powered image generator/classifier** using **PyTorch** and a dataset of famous paintings by *Raja Ravi Varma*.  

---

## 📂 Project Structure

```
├── ART-IMAGE-GENERATOR-CORRECTED.ipynb   # Main Jupyter Notebook
├── raja_ravi_varma_dataset.csv           # Dataset (list of paintings with metadata & image URLs)
├── README.md                             # Documentation
```

---

## 🔧 Setup Instructions

### 1️⃣ Install Python & Jupyter
Make sure you have **Python 3.8+** installed.  
If you don’t have Jupyter:
```bash
pip install notebook
```

### 2️⃣ Install Required Libraries
Run this inside your Jupyter Notebook or terminal:

```bash
pip install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cpu
pip install matplotlib tqdm pandas
```

👉 If you have a **GPU with CUDA**, install PyTorch with GPU support:
```bash
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121
```

### 3️⃣ Clone or Download Project
Put both files in the same folder:
- `ART-IMAGE-GENERATOR-CORRECTED.ipynb`
- `raja_ravi_varma_dataset.csv`

---

## 📊 Dataset

We use a custom dataset:  
**`raja_ravi_varma_dataset.csv`**  

It contains:
- **id** → Painting ID  
- **title** → Name of the artwork  
- **year** → Year painted  
- **category** → e.g., Mythological, Portrait, Royal  
- **image_url** → Direct link to artwork  

Example:
```csv
id,title,year,category,image_url
1,Shakuntala,1870,Mythological,https://upload.wikimedia.org/wikipedia/commons/3/3a/Raja_Ravi_Varma_-_Shakuntala.jpg
2,Lady in Moonlight,1890,Portrait,https://upload.wikimedia.org/wikipedia/commons/5/5d/Lady_in_the_moonlight%2C_Raja_Ravi_Varma.jpg
```

Load dataset in your notebook:

```python
import pandas as pd
df = pd.read_csv("raja_ravi_varma_dataset.csv")
print(df.head())
```

---

## 🚀 Running the Notebook

1. Open Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
2. Open `ART-IMAGE-GENERATOR-CORRECTED.ipynb`
3. Run all cells step by step:
   - Setup (imports, device)
   - Load dataset
   - Training / Evaluation
   - Image Generation / Visualization

---

## 💡 Notes
- If `torch` is not found → run the install command above.  
- If using **Google Colab**, you don’t need local setup — just upload the notebook & dataset.  

---
