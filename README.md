# health_ai_pdf_retrieval
Sequential methods for retrieving fulltext of health AI publications.
Full text can be parsed and sections passed to NLP pipeline.
Data not uploaded due to filesize, but methods generalisable.


Includes:

Inputs = list of PMIDs/DOIs

01_elsevier_xml_retrieval -> uses science direct api to access xml full text (best quality - methods are properly structured) 

==============

02_open_access_url_retrieval -> for remaining papers, use open access api to access direct links for pdfs

02b_open_access_url_pdf_scraper -> for successfully obtained open access links, perform direct pdf download using links

02c_remaining_url_retrieval_pdf_scraper -> for remaining papers (no open access links), try to generate pdf links using host, and download using chrome engine

==============

03a_pdf_to_cermine_xml -> using cermine java app to convert all pdfs to XML format

03b_cermxml_to_methods -> parse xml files to extract methods section

==============

04_remaining_html_scrape_to_methods -> for remaining papers with no pdfs, create online full text access links, scrape and parse html for methods section

==============

05_join_and_clean_methods -> join all successfully extracted methods, and clean text for NLP


#####################################

z_doi_html_retrieval -> deprecated
