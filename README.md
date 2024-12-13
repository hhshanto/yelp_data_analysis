# Yelp Data Analysis Project

## Overview
This project analyzes the Yelp dataset using Azure Databricks and Delta Lake. It implements a complete ETL pipeline for processing and analyzing Yelp's business, review, and user data to derive meaningful insights.

## Project Structure
```
yelp_data_analysis/
├── config/              # Configuration files
│   └── config.py       # Project configuration settings
├── data/               # Data directory
│   ├── raw/            # Raw Yelp dataset files
│   └── processed/      # Processed data files
├── docs/               # Documentation files
│   ├── data_dictionary.md
│   ├── setup_guide.md
│   └── analysis_guide.md
├── logs/               # Log files
├── notebooks/          # Jupyter notebooks for analysis
│   ├── 01_data_ingestion.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_data_transformation.ipynb
│   ├── 04_business_analysis.ipynb
│   └── 05_user_analysis.ipynb
├── src/                # Source code
│   ├── ingestion/      # Data ingestion modules
│   ├── transformation/ # Data transformation modules
│   ├── analysis/       # Analysis modules
│   └── utils/          # Utility functions
├── tests/              # Unit tests
├── venv/               # Virtual environment
├── .gitignore
├── requirements.txt    # Project dependencies
└── README.md
```

## Prerequisites
- Python 3.8+
- Azure Databricks account
- Azure Storage account
- Yelp dataset

## Setup
1. Clone the repository:
```bash
git clone https://github.com/yourusername/yelp_data_analysis.git
cd yelp_data_analysis
```

2. Create and activate virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Configure Azure credentials in `config/config.py`

5. Download and extract Yelp dataset to `data/raw/`

## Data Pipeline
1. **Data Ingestion**
   - Load raw JSON files
   - Validate data structure
   - Perform initial quality checks

2. **Data Transformation**
   - Clean and standardize data
   - Handle missing values
   - Create derived features

3. **Data Analysis**
   - Business metrics analysis
   - Review sentiment analysis
   - User behavior analysis
   - Geographic analysis

## Usage
Follow the notebooks in numerical order:
1. `01_data_ingestion.ipynb`: Initial data loading and validation
2. `02_data_cleaning.ipynb`: Data cleaning and preprocessing
3. `03_data_transformation.ipynb`: Feature engineering and transformations
4. `04_business_analysis.ipynb`: Business-focused analysis
5. `05_user_analysis.ipynb`: User behavior analysis

## Testing
Run tests using pytest:
```bash
pytest tests/
```

## Documentation
- `docs/data_dictionary.md`: Detailed description of all data fields
- `docs/setup_guide.md`: Detailed setup instructions
- `docs/analysis_guide.md`: Analysis methodology and guidelines

## Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments
- Yelp for providing the dataset
- Azure Databricks for the processing platform