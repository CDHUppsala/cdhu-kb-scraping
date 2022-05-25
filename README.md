# cdhu-kb-scraping
Extract datasets from The National Library of Sweden

### scrape_sou_links.ipynb

This notebook extracts all pdf-links from https://sou.kb.se. The links are written to "sou_pdf_links.txt" and, as a batch of wget commands with proper output names (filesystem sane), to "wget_all.sh". Edit wget_all.sh to limit downloads to a smaller range of years if needed – the dataset is relatively huge (hundreds of gigabytes). Use chmod +x and then execute in a Linux/Unix environment.

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
