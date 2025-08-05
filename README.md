# Farm-to-Folk

This model is the first step in the "Farm to Folk" pipeline. Its primary objective is to recommend the most suitable crop for cultivation based on a specific set of soil and environmental conditions. This helps farmers make a quick and data-informed decision about what to plant.

Input Features
The model takes the following seven numerical input features:

N (Nitrogen): The content of Nitrogen in the soil.

P (Phosphorus): The content of Phosphorus in the soil.

K (Potassium): The content of Potassium in the soil.

temperature: The average temperature in Celsius.

humidity: The percentage of humidity in the air.

ph: The pH value of the soil.

tds: Total Dissolved Solids in parts per million (ppm).

Output
The model outputs a single categorical value: the recommended crop_type (e.g., "Tomato", "Rice", "Maize").

Model Implementation
The model is a supervised machine learning classifier, trained on a dataset containing the input features listed above and their corresponding crop_type. The trained model is serialized and saved as crop_prediction_model.joblib for easy loading and deployment.
