# Cultural Heritage Data Guides - Python

Welcome to these guides for working with the Royal Danish Library's digital cultural heritage.

This site contains guides in the form of Python scripts that you can use to programmatically explore datasets that are made from the Royal Danish Library's digital collections. [If you are more familiar with R you can find R scripts on another page.](https://github.com/kb-dk/cultural-heritage-data-guides-R)

[Read more about the Royal Danish Library's digital cultural heritage materials and open datasets](https://www.kb.dk/services/kulturarv-til-forskning-og-studier/kulturarv-som-data-og-datasaet).
 
## Guides

### Archive for Danish Literature (ADL)
**Explore the ADL dataset** - Learn how to parse XML files from the Archive for Danish Literature, clean text data, remove stopwords, and perform collocation analysis to discover word associations in Danish literary texts.

### Flora Danica
**Clean the Flora Danica dataset** - Transform messy metadata into a tidy format by renaming columns, extracting Latin names, parsing taxonomic information, and creating a clean dataset ready for analysis.

**Visualise the Flora Danicas metadata** - Create visualizations to explore the collection, the authors, the taxonomic groups, and the publication patterns.

**Change size on tiff files of Flora Danica** - Resize large TIFF image files while preserving aspect ratios, and display images in Jupyter notebooks using PIL and Matplotlib.

### Copenhagen Diplomatarium (Københavns Diplomatarium)
**Explore the kd dataset** - Analyze medieval, renaissance, and early modern Danish documents from Copenhagen using text mining techniques, including frequency distributions, n-grams, and collocation analysis with NLTK.

### Freedom of the Press Writings (Trykkefrihedens Skrifter)
**Text Mining Freedom of the Press Writings** - Comprehensive text mining workflow including tokenization with regex, removal of Danish and German stopwords, word frequency analysis, filtered analysis by series and volume, and keyword-in-context (KWIC) analysis.

**Bigram Analysis of Freedom of the Press Writings** - Explore word associations and patterns in the Freedom of the Press texts by analyzing bigrams (word pairs), creating network visualizations, and discovering frequently co-occurring terms.

### Denmarks Letters (Danmarks Breve)
**Explore Denmarks Letters** - Explore a dataset constructed from the XML sources behind the Royal Danish Library’s digital collection, `Danmarks Breve`, which holds 13,000+ printed letters and metadata.

## Table of Contents
```{tableofcontents}
```

---

## AI Disclosure

This page has been created with the assistance of the artificial intelligence tools Cursor, a code editor built for scripting and programming. Cursor has been used to co-write scripts, to draft translation from Danish to English, and to organise the content of the notebooks in a similar structure: for example in writing the “Script Summary” sections that is found in the begining of each notebooks. The use of Cursor has served as an opportunity to dive into how to use an AI tool as a “scripting companion”. All AI-created content has been reviewed and critically assessed.