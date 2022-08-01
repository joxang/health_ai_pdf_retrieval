# health_ai_pdf_retrieval
Multiple methods for retrieving fulltxt of health AI publications.
Full text can be parsed and sections passed to NLP pipeline.

Includes:

Inputs = list of PMIDs/DOIs

01_elsevier_xml_retrieval -> uses science direct api to access xml full text

02_open_access_url_retrieval -> from remaining files, use open access api to access direct links for pdfs
02b_open_access_url_pdf_scraper -> direct pdf download using links
02c_closed_access_yrl_retrieval_pdf_scraper -> generate pdf links for remaining files, and download using chrome engine

03
002b_open_access_pdf_scraper -> downloads pdfs using links


000_doi_html_retrieval -> given doi and institutional access, parse html full text
