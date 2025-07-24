# cytokinesis-feature-analysis

CellProfiler-based feature extraction and interactive PCA/LDA software for analyzing cytokinesis stages from multichannel fluorescence microscopy. Developed by Amin Zehtabian at the Ewers Lab, Freie Universität Berlin.

## Features

- CellProfiler pipeline for segmenting bridge-like midbody structures
- Feature extraction from multichannel fluorescence images
- Visualize pairwise feature relationships
- Interactive Jupyter Notebook for PCA/LDA-based phase visualization
- Interactive GUI for selecting features, components, and plot types
- Optional polynomial fit overlay on PCA/LDA projections

## File Structure

- `PCA_Software_v3.ipynb` – Jupyter notebook for PCA and feature analysis
- `CP_featureExtraction.cppipe` – CellProfiler pipeline for feature extraction
- `Feature_Excel_File.xlsx` – Sample input feature table
- `requirements.txt` – Python dependencies
- `README.md` – This file

## Installation

Create a new Python environment and install dependencies:

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```

Or install manually in a Colab notebook using:

```python
!pip install pandas numpy matplotlib seaborn scikit-learn ipywidgets openpyxl
```

## Usage

1. Place `Feature_Excel_File.xlsx` in the same directory as the notebook (or update the path in code).
2. Run `PCA_Software_v3.ipynb` in Jupyter or Colab.
3. Use the GUI to:
   - Select features
   - Visualize PCA/LDA projections
   - Optionally apply polynomial fitting
4. Use the CellProfiler pipeline separately to extract features from image data.

## Author

Developed by **Amin Zehtabian, PhD**  
Ewers Lab, Freie Universität Berlin  
GitHub: [@zehtabian](https://github.com/zehtabian)  
Contact: amin.zehtabian@fu-berlin.de

## License

MIT License

## Related Repositories

Part of the broader analysis effort alongside Zack Marin's  
[expansion-analysis](https://github.com/zacsimile/expansion-analysis) repository.
