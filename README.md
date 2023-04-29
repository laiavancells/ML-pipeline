# Pre-Processing and Machine Learning Pipeline for Instrumented Insole GRFs

## Description

The purpose of this code is to import, clean, normalize and manipulate Ground Reaction Force (GRF) data from instrumented insoles in pandas DataFrame format

## Getting Started

### Dependencies

Python 3

Pandas

Matplotlib

Spicy

### Installing

To run this code, you must have Python installed. You can install the necessary libraries using pip:
- import pandas as pd
- import numpy as np
- import matplotlib.pyplot as plt
- from scipy.signal import find_peaks

Additionally, this code requires the following files to be present in the working directory:

- The raw GRF files (in this case: tred02.txt)
- An excel file with the labels (in this case: labels tredmill.xlsx)

### Instructions

To run the code, execute each cell in the order presented. The resulting DataFrame will be printed after each cell.

The tred02.txt (or an equivalnent file) must be in the correct format, as follows:

- The first row contains strings describing the contents of each column.
- The second row contains units for each column.
- The third row contains empty cells.
- The fourth row contains the data, with the first column containing time in seconds.


The labels tredmill.xlsx (or an equivalent file)  must have the following format:

- The first row contains column headers.
- The first column contains comments describing each row.
- The second column contains the body weight of each subject, in kg.

The resulting DataFrame (output) will contain the following columns:
- Time: The time in seconds.
- Forefoot: The GRF measured by the forefoot sensor.
- Midfoot: The GRF measured by the midfoot sensor.
- Heel: The GRF measured by the heel sensor.
- Total: The total GRF measured by all sensors.
- NormForefoot: The normalized GRF measured by the forefoot sensor.
- NormMidfoot: The normalized GRF measured by the midfoot sensor.
- NormHeel: The normalized GRF measured by the heel sensor.
- NormTotal: The normalized total GRF.
- AT_loading: The calculated Achilles tendon loading.

## Help

If you encounter any issues while using this project, try the following:

- Check that all dependencies are installed correctly
- Make sure that you are using the correct command to run the project

## Authors

Laia Vancells Lopez 

laia.vancellslopez@student.fairfield.edu

## Version History
* 0.1
    * Initial Release

## License

This project is licensed under the laiavancells License - see the LICENSE.md file for details

## Acknowledgments

I would like to thank Dr. Drazan and Dr. Bandara for their valuable feedback and contributions to this project. Their insights and expertise were instrumental in improving the quality of our work.
