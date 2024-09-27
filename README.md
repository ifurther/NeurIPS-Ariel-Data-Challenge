# Ariel Data Challenge 2024: Exoplanet Spectrum Analysis

## Project Overview

This project is an attempt at the Ariel Data Challenge 2024, which focuses on extracting exoplanetary signals from simulated observations of the upcoming ESA Ariel Mission. The challenge involves processing complex astrophysical data to detect and characterize exoplanets.


Link to dataset: https://www.kaggle.com/competitions/ariel-data-challenge-2024


## Key Features

- Data loading and preprocessing for AIRS-CH0 and FGS1 signals
- Implementation of various calibration techniques:
  - Dark frame correction
  - Flat field correction
  - Dead/hot pixel correction
  - Linearity correction
  - Read noise correction
- Jitter correction using FGS1 data
- Transit model fitting
- Spectrum extraction and uncertainty estimation
- Machine learning model implementation (Linear Regression and Random Forest)

## Technologies Used

- Python 3.10
- Libraries: NumPy, Pandas, Matplotlib, SciPy, Scikit-learn

## Setup and Installation

1. Clone this repository
2. Install the required packages:
3. pip install numpy pandas matplotlib scipy scikit-learn tqdm

3. Download the Ariel Data Challenge dataset and place it in the appropriate directory

## Usage

Run the main script to process the data and generate a submission file:

## Project Structure

- `load_planet_data()`: Loads and applies initial corrections to the raw data
- `calibrate_data()`: Applies various calibration techniques
- `correct_jitter()`: Corrects for jitter using FGS1 data
- `fit_transit_model()`: Fits a transit model to the data
- `process_planet()`: Main function for processing individual planet data
- `process_all_planets()`: Processes all planets in the dataset
- `train_and_evaluate_models()`: Trains and evaluates machine learning models
- `prepare_submission()`: Prepares the final submission file

## Challenges and Learnings

This project presented significant challenges, particularly in understanding and correctly implementing the physics-based signal processing techniques required for accurate exoplanet detection. While the final model did not achieve a competitive score, the project provided invaluable learning experiences in:

- Astrophysical data processing
- Signal processing in the context of exoplanet detection
- The critical importance of domain knowledge in machine learning projects
- Handling and processing large, complex scientific datasets

## Future Improvements

- Implement more sophisticated jitter correction techniques
- Explore advanced machine learning models specifically designed for time-series spectral data
- Collaborate with domain experts to refine the signal processing approach
- Optimize code for faster processing of large datasets

## Acknowledgements

Special thanks to the organizers of the Ariel Data Challenge 2024 and to the Kaggle community for providing this learning opportunity.
