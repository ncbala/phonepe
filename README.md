Overview:
This project contains the code and scripts that are required to collect phonepe data from a GitHub clone and store them in mysql db for further analysis.  The project contains the following modules:
1) GitHub Data Loader: This module contains the Python code to traverse all the GitHub data files (json) into dataframes.  Once the content is loaded into dataframes further analysis is done to clean up the data.
2) CSV Writer: Post clean-up, the data collected in the dataframes are further processed and stored in CSV files. This would save time and eliminate performing Step 1 multiple times.
3) DB Writer: This Python module reads the data from the above mentioned CSV files and stores them into mysql db using appropriate sql commands.
4) Geo Indexer: This module is responsible for scanning the data folder and extract the geo information (Country, State, District & Pincodes)
5) Streamlit WebApp: A webapp based on streamlit framework is used to present various insights derived from the phonepe data.

Deliverables:
1) pp_dbdef_nocred.ipynb: Contains Python code to create the db and tables.
2) pp_backend_nocred.ipynb: Contains Python code for GitHub Data Loader, CSV Writer, DB Writer and Geo Indexer.
3) pp_app_nocred.ipynb: Contains Python code for the webapp for presenting various dashboards.
4) csv files: These files contain the transaction, insurance and user records.  Additionally geo records for state, districts and pincodes are also present.

DB Schema: 
1) Transaction tables: transaction_agg, transaction_top, transaction_hover
2) Insurance tables: insurance_agg, insurance_top, insurance_hover
3) User and Device tables: user_agg, user_top, user_hover and device_agg
4) Geo-info tables: Geo (used for storing information about geo locations referenced in the phonepe data)

