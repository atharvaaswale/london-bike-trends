# London Bike Rides Analysis

![Bike Sharing](https://images.unsplash.com/photo-1551966775-a4ddc8df0528?ixlib=rb-4.0.3&auto=format&fit=crop&w=1350&q=80)

This project analyzes bike-sharing trends in London, examining the influence of weather, seasons, holidays, and weekends. It includes a Jupyter Notebook that preprocesses and cleans a bike rides dataset, producing a structured Excel file for further analysis.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset Description](#dataset-description)
- [Installation](#installation)
- [Usage](#usage)
- [File Structure](#file-structure)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Project Overview
This project explores bike-sharing patterns in London using hourly ride data. The Jupyter Notebook performs key preprocessing steps, including:
- Renaming columns for clarity
- Scaling humidity to a 0-1 range
- Mapping numerical codes to descriptive labels (e.g., "winter" for season, "Clear" for weather)
- Exporting the cleaned dataset as `london_bikes_final.xlsx`

The resulting dataset is ready for exploratory data analysis, visualizations, or predictive modeling.

## Dataset Description
The dataset (`london_merged.csv`) contains hourly bike ride counts in London with environmental and temporal features. Columns include:

- **time**: Timestamp of the record (hourly)
- **count**: Number of bike rides
- **temp_real_C**: Actual temperature in Celsius
- **temp_feels_like_C**: "Feels like" temperature in Celsius
- **humidity_percent**: Humidity as a percentage
- **wind_speed_kph**: Wind speed in kilometers per hour
- **weather**: Weather condition (e.g., Clear, Rain, Snowfall)
- **is_holiday**: Binary indicator for holidays (1 = holiday, 0 = non-holiday)
- **is_weekend**: Binary indicator for weekends (1 = weekend, 0 = weekday)
- **season**: Season of the year (spring, summer, autumn, winter)

The notebook transforms the data by standardizing formats and enhancing readability.

## Installation
To set up the project locally, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/LondonBikeRidesAnalysis.git
   cd LondonBikeRidesAnalysis
   ```

2. **Set up a Python environment**:
   Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**:
   Install required libraries from `requirements.txt`:
   ```bash
   pip install -r requirements.txt
   ```

4. **Install Jupyter Notebook** (if needed):
   ```bash
   pip install jupyter
   ```

## Usage
1. **Launch Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```
   Open `london_bike_rides.ipynb` in the Jupyter interface.

2. **Run the notebook**:
   - Ensure `london_merged.csv` is in the project directory or update the file path.
   - Execute cells sequentially to preprocess the data and generate `london_bikes_final.xlsx`.

3. **Explore the output**:
   The cleaned dataset, `london_bikes_final.xlsx`, is ready for further analysis or visualization.

## File Structure
```
LondonBikeRidesAnalysis/
├── london_bike_rides.ipynb    # Jupyter Notebook with preprocessing
├── london_bikes_final.xlsx    # Cleaned dataset output
├── requirements.txt           # Python dependencies
├── README.md                  # Project documentation
└── london_merged.csv          # Original dataset (add your own)
```

## Contributing
Contributions are welcome. To contribute:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Make changes and commit (`git commit -m "Add your feature"`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a Pull Request.

Please ensure code is documented and aligns with project standards.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements
- The dataset is sourced from public bike-sharing data for London.
- Thanks to the open-source community for tools like Pandas, NumPy, and Jupyter.
- Image credit: [Unsplash](https://unsplash.com).
