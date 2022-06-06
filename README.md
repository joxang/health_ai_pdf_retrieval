# health_ai_pdf_retrieval
Multiple methods for retrieving fulltxt of health AI publications.
Full text can be parsed and sections passed to NLP pipeline.

Includes:
000_doi_html_retrieval -> given doi and institutional access, parse html full text
001_elsevier_xml_retrieval -> uses science direct api to access xml full text
002_open_access_link_retrieval -> uses open access api to access links for pdfs
002b_open_access_pdf_scraper -> downloads pdfs using links