# Location Mention Recognition (LMR) for Disaster Response

## Table of Contents
- [Project Overview](#project-overview)
- [Project Objectives](#project-objectives)
- [Accessing Data](#accessing-data)
- [Solution Approach](#solution-approach)
- [Project Results](#project-results)
- [Usage](#usage)
- [Resources](#resources)
- [Acknowledgments](#acknowledgments)
- [License](#license)

## Project Overview

This project is part of a competition focused on building an automated system for Location Mention Recognition (LMR) in microblogging posts (e.g., tweets) during emergencies. The aim is to recognize location mentions and support response authorities by providing geolocation data for critical information, such as the need for medical assistance, food, shelter, and infrastructure reports.

## Project Objective

The goal of the LMR system is to extract toponyms (e.g., place, area, street names) from unstructured microblogging posts. Due to the high volume of posts, this system automates location extraction, enabling authorities to efficiently gather location data critical for disaster response.

## Accessing Data

The data used in this project is sourced from microblogging posts provided in CSV format. The dataset is split as follows:
- ```Train_1.csv```: Contains training data with labeled location mentions.
- ```Test.csv```: Contains test data for model inference without target-related columns.

Each row in the data represents a single post, with location mentions annotated for training purposes. Data files are structured as follows:
- ```ID```: Unique identifier for each post.
- ```Text```: Content of the post.
- ```Location Mentions```: Target labels indicating location mentions in the text (for Train_1.csv only).

Sample data and the submission format are available for reference. Find in [/Data](./Data/)

## Solution Approach

This project leverages state-of-the-art Natural Language Processing (NLP) techniques for the LMR task, focusing on:
1. **Tokenization**: Breaking down text into tokens to identify location mentions accurately.
2. **Named Entity Recognition (NER)**: Using a pre-trained language model fine-tuned to identify location entities in text.
3. **Location Mention Recognition**: Recognizing and tagging location mentions in the text, including city, area, and street names.

Key steps in the process:
- **Data Preprocessing**: Clean and preprocess text data to optimize model performance.
- **Model Training**: A custom NER model is trained to detect location mentions from text. Model training adheres to competition restrictions of an 8-hour maximum runtime.
- **Inference**: The trained model is applied to the test data to generate predictions within the specified time limits.

## Project Results

Model performance is evaluated based on the accuracy of location mentions extracted in terms of both precision and recall. Metrics and sample predictions are included in the notebook.

## Usage

To run this project:
1. **Install Required Libraries:** Use the `requirements.txt` file to install the necessary libraries.
2. **Open the Notebook:** Open the Google Colab notebook to run the model and generate predictions.
3. **Run the Notebook:** Execute the cells in the notebook to reproduce the analysis and predictions.

### Submission Format
Ensure that the submission file matches the format in `SampleSubmission.csv`, maintaining correct row order and ID names.


## Resources

This project was completed with support from:
- [Microsoft Learn modules](https://learn.microsoft.com/) on NLP, LLMs, and Azure Machine Learning.
- Dataset and detailed guidelines are available on the [IDRISI GitHub repository](https://github.com/rsuwaileh/IDRISI/tree/main/LMR).

## Acknowledgments

Special thanks to [Microsoft](https://www.microsoft.com), [Hamad Bin Khalifa University (HBKU)](https://www.hbku.edu.qa) and [Zindi](https://zindi.africa) for hosting this competition.


## License

[![CC BY-SA 4.0][cc-by-sa-shield]][cc-by-sa]

This work is licensed under a
[Creative Commons Attribution-ShareAlike 4.0 International License][cc-by-sa].

[![CC BY-SA 4.0][cc-by-sa-image]][cc-by-sa]

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/
[cc-by-sa-image]: https://licensebuttons.net/l/by-sa/4.0/88x31.png
[cc-by-sa-shield]: https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg


