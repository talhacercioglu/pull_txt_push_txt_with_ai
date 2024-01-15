## Real Estate Price Prediction System
This project aims to predict real estate prices based on various features such as location, property type, and size. The prediction is made using a Gradient Boosting model trained on historical real estate data.
## Run the Application:
python main.py
The application will continuously monitor the input_verileri.txt file for new input data. Once new data is detected, it will use the trained model (gradient_boosting_model_2.pkl) to predict the real estate price and write the result to predicted_price.txt.
## Provide Input Data:
Create or update the input_verileri.txt file with the necessary input data in the following format:
{
    'il_input': 'Istanbul',
    'ilce_input': 'Kadikoy',
    'mahalle_input': 'Moda',
    'konut_tipi_input': 'Apartment',
    'bulundugu_kat_input': '5',
    'Metrekare': 120,
    'OdaSayisi': 3,
    'SalonSayisi': 1
}
## View Prediction:
The predicted price will be displayed in the console, and the result will be written to predicted_price.txt.
## File Descriptions
main.py: The main script that reads input data, performs predictions, and writes results.
models/gradient_boosting_model_2.pkl: The trained Gradient Boosting model for price prediction.
data/...: Directory containing labeled data for different features used in prediction.
input_verileri.txt: File to input data for prediction.
predicted_price.txt: File containing the predicted real estate price.
### Additional Information
The get_info function in main.py retrieves information from dictionaries based on user inputs.
The tahmin_yap function loads the trained model and makes predictions using the input features.
Feel free to explore and modify the code to suit your needs. If you encounter any issues or have suggestions for improvement, please create an issue or submit a pull request.
Happy coding!
