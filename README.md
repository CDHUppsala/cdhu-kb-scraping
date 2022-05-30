# cdhu-kb-scraping
Extract datasets from The National Library of Sweden

### generate_from_csv.ipynb 

This notebook parses a previously created csv data-file (sou_data.csv) to generate a bash-script that will download SOU dataset from https://sou.kb.se. 

The bash script uses wget to download while also giving the pdf-files sanitized names based on titles in the csv-file. The generated script also sorts them into a folder structure organized by year. A pre-generated example script can be found in the subfolder run-csv/. You can either edit/execute the script directly or run this notebook to customize the download-script to your liking. 


```python
CDHU="""\
 ____ ____ ____ ____ ________ 
||C |||D |||H |||U |||       
||__|||__|||__|||__|||_______
|/__\|/__\|/__\|/__\|/_______

 EXTRACT SOU / BEAUTIFUL SOUP
"""
```

### scrape_sou_links.ipynb

Update: This script is not needed anymore! Instead use generate_from_csv.ipynb to parse sou_data.csv.

This notebook extracts all pdf-links from https://sou.kb.se. The links are written to "sou_pdf_links.txt" and to "wget_all.sh", as a batch of wget commands with proper output names (filesystem sane). Edit wget_all.sh to limit downloads to a smaller range of years if needed – the dataset is relatively huge (hundreds of gigabytes). Use chmod +x and then execute in a Linux/Unix environment.

Already prepared outputfiles can also be found in [run/](https://github.com/CDHUppsala/cdhu-kb-scraping/tree/main/run).

```python
CDHU="""\
 ____ ____ ____ ____ ________ 
||C |||D |||H |||U |||       
||__|||__|||__|||__|||_______
|/__\|/__\|/__\|/__\|/_______

 EXTRACT SOU / BEAUTIFUL SOUP
"""
```
