# Textmining Trykkefrihedens Skrifter - Python Jupyter Notebook Version

This project provides Jupyter Notebooks for text mining analysis of "Trykkefrihedens Skrifter" (Freedom of the Press Writings), replicating the original R workflow in Python. The notebooks guide you through data loading, tokenization, stopword removal, word frequency analysis, filtered analysis, keyword-in-context (KWIC) analysis, and bigram analysis.

## Features

- **Interactive Jupyter Notebooks**: All steps are divided into clear code and markdown cells with explanations
- **Data Loading**: Reads structured CSV data from Trykkefrihedens Skrifter
- **Regex Tokenization**: Splits text into words using a regex pattern
- **Stopword Removal**: Handles Danish, German, and project-specific stopwords
- **Word Frequency Analysis**: Counts and ranks word frequencies
- **Filtered Analysis**: Focuses on Række 1, Bind 5+6 (Landøkonomi)
- **Keyword-in-Context (KWIC)**: Finds and displays context for keywords (e.g., 'jord')
- **Bigram Analysis**: Analyzes word pairs and their frequencies
- **Network Visualization**: Creates network graphs of frequent bigrams
- **Results Export**: Saves results to CSV files for further analysis

## Notebooks

### 1. TextMining_Trykkefrihedens_Skrifter.ipynb
Main text mining workflow including:
- Word frequency analysis
- Stopword removal
- Keyword-in-context analysis
- Filtered analysis (Række 1, Bind 5+6)

### 2. Bigrams_Trykkefrihedens_Skrifter.ipynb
Bigram (word pair) analysis including:
- Bigram formation and counting
- Stopword filtering for bigrams
- Regex pattern matching
- Network graph visualization
- Bigram frequency analysis

## Installation

1. **Install Python dependencies:**
   ```bash
   pip install pandas numpy nltk matplotlib seaborn networkx
   ```
2. **Download NLTK data:**
   The notebooks will attempt to download required NLTK data (stopwords, punkt) automatically. If you encounter issues, run these in a Python shell:
   ```python
   import nltk
   nltk.download('punkt')
   nltk.download('stopwords')
   ```

## Usage

1. **Open the notebooks:**
   - Launch Jupyter Notebook or JupyterLab in your project directory.
   - Open either `TextMining_Trykkefrihedens_Skrifter.ipynb` or `Bigrams_Trykkefrihedens_Skrifter.ipynb`.

2. **Check your data files:**
   - `tfs_data/tfs_structured.csv` — Main text data
   - `tfs_data/tfs_stopord.csv` — Project-specific stopwords

3. **Run the notebooks:**
   - Execute each cell in order. Read the markdown explanations for guidance.
   - The notebooks will display word frequencies, bigram analysis, and visualizations.

4. **View and use results:**
   - Output CSV files will be saved in your project directory:
     - `results_word_frequencies_all.csv`
     - `results_word_frequencies_filtered.csv`
     - `results_kwic_jord.csv`
     - `results_bigrams_filtered.csv`
     - `results_bigrams_match.csv`
   - Network graphs will be saved as PNG files in the `graphics/` folder.

## Notebook Structure

### Text Mining Notebook:
1. **Title & Introduction** — Overview of the workflow
2. **Install and Import Dependencies** — Required packages and setup
3. **Load Data** — Read main data and stopwords
4. **Tokenization with Regex** — Split text into words
5. **Stopword Handling** — Remove Danish, German, and project-specific stopwords
6. **Word Frequency Analysis** — Count and display word frequencies
7. **Filtered Analysis** — Focus on Række 1, Bind 5+6
8. **Keyword-in-Context (KWIC) Analysis** — Find context for keywords
9. **Save Results** — Export results to CSV
10. **Conclusion** — Summary and next steps

### Bigram Analysis Notebook:
1. **Title & Introduction** — Overview of bigram analysis
2. **Install and Import Dependencies** — Required packages and setup
3. **Load Data** — Read main data and stopwords
4. **Formation of Bigrams** — Create word pairs from text
5. **Count Bigrams** — Count bigram frequencies
6. **Remove Bigrams with Stopwords** — Filter out stopwords from bigrams
7. **Count Filtered Bigrams** — Count frequencies after filtering
8. **Search for Specific Bigrams** — Regex pattern matching
9. **Visualization as Network Graph** — Create network visualizations
10. **Save Graph and Results** — Export results and visualizations

## Data Structure

The notebooks expect the following columns in `tfs_structured.csv`:
- `refnr`: Reference number
- `række`: Series number
- `bind`: Volume number
- `side`: Page number
- `content`: Text content

## Notes

- The workflow is now fully interactive and notebook-based.
- You can further explore, visualize, or adapt the analysis as needed.
- If you need to add new analyses or visualizations, simply add new cells to the notebooks.
- The bigram analysis provides insights into word co-occurrence patterns.

---