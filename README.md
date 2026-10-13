# Disaster Tweets Classification 🌍🌀

![GitHub release](https://img.shields.io/badge/Latest_Release-v1.0.0-brightgreen)  
[![GitHub Releases](https://img.shields.io/badge/Check_Releases-blue)](https://github.com/kade-one/disaster-tweets-classification/releases)

## Table of Contents
1. [Project Overview](#project-overview)
2. [Technologies Used](#technologies-used)
3. [Getting Started](#getting-started)
   - [Prerequisites](#prerequisites)
   - [Installation](#installation)
4. [Data Sources](#data-sources)
5. [Project Structure](#project-structure)
6. [Analysis and Modeling](#analysis-and-modeling)
   - [ETL Process](#etl-process)
   - [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
   - [Deep Learning Models](#deep-learning-models)
7. [Visualization](#visualization)
8. [Usage](#usage)
9. [Contributing](#contributing)
10. [License](#license)
11. [Contact](#contact)

## Project Overview

The **Disaster Tweets Classification** project aims to classify tweets that are related to disasters. This project leverages data from AWS RDS, utilizing CSV files for data storage. The process includes an ETL (Extract, Transform, Load) pipeline, exploratory data analysis (EDA), and the implementation of deep learning models in Jupyter Notebooks. Visualizations and dashboards are created using Tableau to present the findings effectively.

For the latest updates, please check our [Releases](https://github.com/kade-one/disaster-tweets-classification/releases).

## Technologies Used

- **AWS RDS**: For relational database storage.
- **AWS S3**: For storing CSV files.
- **Python**: Primary programming language for data analysis and modeling.
- **Jupyter Notebook**: For interactive coding and data exploration.
- **Deep Learning**: Utilizing neural networks for classification tasks.
- **Tableau**: For creating visualizations and dashboards.
- **Transformers**: For advanced NLP tasks.

## Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:

- Python 3.6 or higher
- Jupyter Notebook
- AWS CLI configured with access to RDS and S3
- Tableau Desktop or Tableau Prep Builder

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/kade-one/disaster-tweets-classification/releases
   cd disaster-tweets-classification
   ```

2. Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Download the necessary data files from the [Releases](https://github.com/kade-one/disaster-tweets-classification/releases) section and place them in the appropriate directories.

## Data Sources

The project uses CSV files stored in AWS RDS. These files contain tweets and their respective classifications. The data is sourced from Kaggle competitions, ensuring a rich dataset for analysis.

## Project Structure

The repository is organized as follows:

```
disaster-tweets-classification/
│
├── data/
│   ├── raw/                 # Raw data files
│   ├── processed/           # Processed data files
│
├── notebooks/               # Jupyter notebooks for analysis
│   ├── etl_notebook.ipynb
│   ├── eda_notebook.ipynb
│   ├── model_notebook.ipynb
│
├── src/                    # Source code
│   ├── etl.py              # ETL pipeline
│   ├── eda.py              # EDA functions
│   ├── model.py            # Deep learning models
│
├── visualizations/         # Tableau files
│   ├── dashboard.twbx
│   ├── prep_flow.tfl
│
├── requirements.txt        # Python dependencies
└── README.md               # Project overview
```

## Analysis and Modeling

### ETL Process

The ETL process involves extracting data from the RDS database, transforming it into a suitable format, and loading it into a new dataset for analysis. The `etl.py` script handles this process, ensuring that the data is clean and structured.

### Exploratory Data Analysis (EDA)

EDA is performed in `eda_notebook.ipynb`. This notebook contains visualizations and statistical summaries that help in understanding the data. Key insights include:

- Distribution of tweet categories.
- Frequency of words in disaster-related tweets.
- Correlation between tweet length and classification.

### Deep Learning Models

The modeling process is carried out in `model_notebook.ipynb`. Here, we implement various deep learning architectures, including:

- **Convolutional Neural Networks (CNN)**: Effective for text classification.
- **Recurrent Neural Networks (RNN)**: Useful for sequential data.
- **Transformers**: State-of-the-art models for NLP tasks.

The models are evaluated based on accuracy, precision, and recall metrics.

## Visualization

Visualizations are created using Tableau, providing a clear and interactive dashboard for users. The `visualizations` folder contains Tableau files that can be opened in Tableau Desktop or Tableau Prep Builder. Key visualizations include:

- Tweet distribution by category.
- Word clouds for different disaster types.
- Trends over time for tweet activity.

## Usage

To run the analysis, open the Jupyter notebooks in the `notebooks` directory. Execute each cell step-by-step to perform the ETL process, EDA, and modeling. For visualizations, open the Tableau files in Tableau Desktop.

## Contributing

We welcome contributions to improve the project. If you would like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For questions or suggestions, feel free to reach out to the project maintainers. You can find their contact information in the repository.

For more updates and to download the latest files, please visit our [Releases](https://github.com/kade-one/disaster-tweets-classification/releases).