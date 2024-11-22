# Barbell Exercise Tracker

## Overview
This project focuses on developing a barbell exercise tracking system to classify exercises, count repetitions, and detect improper form using accelerometer and gyroscope data from wearables. The system was built with the aim of providing real-time insights for strength training, similar to a digital personal trainer, leveraging machine learning for accurate tracking and feedback.

## Features
- **Exercise Classification**: Classifies various barbell exercises using sensor data.
- **Repetition Counting**: Counts repetitions accurately during gym workouts.
- **Form Detection**: Detects improper exercise form to help users prevent injuries.

## Tools and Technologies
- **Programming Languages**: Python
- **Data Collection**: Accelerometer and Gyroscope data from **Empatica Embrace Plus** wristband sensors.
- **Libraries**: 
  - **NumPy, Pandas**: For data manipulation and preprocessing.
  - **scikit-learn**: For training and evaluation of machine learning models.
- **Data Analysis Techniques**:
  - **Supervised Learning**: Used for classifying exercises and detecting improper form.
  - **Clustering (K-Means)**: To identify patterns in exercise data.
  - **Feature Engineering**: PCA, Low-pass Filtering, and Fourier Transformation for data preprocessing.
- **Deployment Tools**:
  - **Anaconda**: Used to create and manage the project environment.
  - **Docker**: For containerizing the application and ensuring consistency across environments.

## How It Works
1. **Data Collection**: Data is collected from wristband sensors during different barbell exercises such as squats, deadlifts, and presses.
2. **Data Preprocessing**: The raw sensor data is cleaned, aggregated, and transformed using techniques like **low-pass filtering** and **PCA**.
3. **Model Training**: A variety of machine learning models, including **Random Forests**, were trained and evaluated to classify exercises and detect improper form.
4. **Repetition Counting**: Peak counting algorithms were applied to count the number of repetitions during each exercise.
5. **Form Analysis**: Models were trained to detect improper exercise form using collected data, providing corrective feedback.

## Setup and Installation
1. **Clone the Repository**:
   ```sh
   git clone <repository-url>
   cd barbell-exercise-tracker
   ```
2. **Set Up Environment**:
   - Create and activate an Anaconda environment:
     ```sh
     conda create --name exercise_tracker_env --file conda_requirements.txt
     conda activate exercise_tracker_env
     ```
   - Install additional Python packages:
     ```sh
     pip install -r pip_requirements.txt
     ```
3. **Run the Application**:
   ```sh
   python main.py
   ```

## Results
- Achieved **98% accuracy** in exercise classification.
- Obtained a **5% error rate** for repetition counting.

## References
- The project is inspired by concepts from "Machine Learning for the Quantified Self" by Mark Hoogendoorn and Burkhardt Funk, leveraging sensor data for activity tracking.

## Future Improvements
- Extend the system to include more types of strength training exercises.
- Implement real-time feedback for form correction via mobile or web application interfaces.


