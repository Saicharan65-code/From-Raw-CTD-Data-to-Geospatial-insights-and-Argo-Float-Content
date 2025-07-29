SeaSnap
From Raw CTD Data to Geospatial Insights and Argo Float Context

SeaSnap is a comprehensive data pipeline and visualization platform for Conductivity, Temperature, and Depth (CTD) data. The project streamlines the transformation of raw CTD files into structured datasets, applies rigorous quality control, and presents interactive geospatial analytics via a web dashboard.

Features
Multi-format Data Ingestion
Supports parsing and extraction from various raw CTD file formats, including:

.cnv
.asci
.xls
.dat
Data Structuring
Converts extracted data into structured tables suitable for analysis and visualization.

Quality Control
Implements quality control mechanisms inspired by Argo float data standards.

Assigns QC flags to each parameter (e.g., temperature, salinity, conductivity).
Geospatial Visualization & Analytics

Interactive maps and plots to explore CTD data spatially and temporally.
Available plots include:
Depth vs Temperature
Depth vs Salinity
Depth vs Conductivity
Temperature-Salinity (TS) plots
Web Dashboard
A live web application (using a live server) presents all CTD data and analytics in an accessible dashboard format.

Getting Started
Prerequisites
Python 3.x
Required libraries (see requirements.txt)
(Optional) Node.js or another live-server tool for hosting the dashboard
Installation
Clone the repository

bash
git clone https://github.com/pajonnakuti/seasnap.git
cd seasnap
Install dependencies

bash
pip install -r requirements.txt
(Optional) Start the live server
For the dashboard:

bash
# Example using Python's http.server
python -m http.server 8000
Usage
Place your raw CTD files in the designated input directory.
Run the extraction and structuring scripts to process the data.
Access the dashboard via the live server to explore your data and analytics.
Project Structure
Code
seasnap/
│
├── data/                # Raw and processed CTD data
├── scripts/             # Extraction, QC, and processing scripts
├── dashboard/           # Web dashboard source code
├── requirements.txt     # Python dependencies
└── README.md
Quality Control
QC flags follow standard conventions similar to Argo float data.
Each parameter in the dataset (temperature, salinity, conductivity, etc.) receives a QC flag for transparency and reproducibility.
Visualization
Interactive geospatial visualizations for quick insights
Detailed parameter plots for scientific analysis
Contributing
Contributions are welcome! Please open issues and pull requests for suggestions, bugfixes, or new features.

License
MIT License
