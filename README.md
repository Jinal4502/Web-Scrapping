# Web-Scrapping

This repository contains a set of Jupyter Notebooks for scraping research article links (DOIs) from the ASU Library and extracting PDFs from various publishers. It is designed to automate the process of collecting and downloading PDFs for research purposes.

---

## 📂 Repository Contents

| File Name | Description |
|-----------|-------------|
| **asu_scrapper_doi (1).ipynb** | Scrapes article links/DOIs from the ASU Library. This notebook generates the URLs/links from which PDFs can later be downloaded. |
| **asu_pdf_extraction (2).ipynb** | Downloads PDFs for publishers where direct PDF download links are available. Handles straightforward cases where the PDF is directly accessible. |
| **failed_pdf_extractor.ipynb** | Handles failed cases from `asu_pdf_extraction`. Opens the article link in Safari and attempts to scrape the PDF when direct download fails. |
| **pdf_extraction_ieee_dash.ipynb** | Extracts PDFs from IEEE Xplore (and similar) links obtained via the ASU Library. |
| **pdf_extraction_onlinewiley.ipynb** | Extracts PDFs from OnlineWiley publisher links. |
| **sciencedirect_pdf_extraction (2).ipynb** | Extracts PDFs from ScienceDirect publisher links. |

---

## 📝 Workflow

1. **Scrape DOIs/Links**  
   Use `asu_scrapper_doi (1).ipynb` to scrape article links using DOIs from the ASU Library.

2. **Direct PDF Extraction**  
   Run `asu_pdf_extraction (2).ipynb` to download PDFs where direct download links exist.

3. **Handle Failed Downloads**  
   If some PDFs fail to download, for either of the publishers mentioned in `asu_pdf_extraction (2).ipynb`, run `failed_pdf_extractor.ipynb` to open the links in Safari and scrape PDFs manually.

4. **Publisher-Specific Extraction**  
   For publisher-specific links (IEEE, Wiley, ScienceDirect, etc.), run the respective notebooks:
   - `pdf_extraction_ieee_dash.ipynb`
   - `pdf_extraction_onlinewiley.ipynb`
   - `sciencedirect_pdf_extraction (2).ipynb`

---
