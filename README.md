# Spark Assignment COVID-19 Analysis API

This project provides an API for analyzing COVID-19 data using Apache Spark and Python's `http.server` module. The API allows users to query various statistics related to COVID-19 cases and deaths across different countries.

## Prerequisites

- Python 3.x
- Apache Spark
- PySpark

## Installation

1. Clone this repositor:

```bash
git clone https://github.com/mohan-333/spark_assignment.git
```

2. Install the required dependencies:

```bash
pip install -r requirements.txt
```

## Project Structure

```css
spark-assignment/
├── src/
│   ├── main.py
│   ├── loader.py
│   └── proc.py
├── data/
│   ├── input/
│   └── output/
├── logs/
│   └── log.txt
├── README.md
└── requirements.txt
```

## Usage

1. Navigate to the project directory:

```bash
cd spark_assignment
```

2. Run the server

```bash
python3 src/main.py 2>&1 | tee logs/log.txt
```

3. Once the server is running, you can access the API endpoints through your web browser or by sending HTTP GET requests to `http://localhost:8000`.


## API Endpoints

The following endpoints are available:

- `/mostAffected`: Returns the country most affected by COVID-19 (total deaths / total cases).

- `/leastAffected`: Returns the country least affected by COVID-19 (total deaths / total cases).

- `/highestCases`: Returns the country with the highest number of COVID-19 cases.

- `/lowestCases`: Returns the country with the lowest number of COVID-19 cases.

- `/totalCases`: Returns the total number of COVID-19 cases worldwide.

- `/mostEfficient`: Returns the country that handled COVID-19 most efficiently (highest recovery rate per case).

- `/leastEfficient`: Returns the country that handled COVID-19 least efficiently (lowest recovery rate per case).

- `/highestCritical`: Returns the country with the highest number of critical COVID-19 cases.

- `/lowestCritical`: Returns the country with the lowest number of critical COVID-19 cases.


## Data Sources

The COVID-19 data used in this project is sourced from `https://disease.sh/v3/covid-19/countries`. The data is loaded and processed using Apache Spark.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## Author

#### MOHAN REDDY THOTA



