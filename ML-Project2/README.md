# Bangalore Home Price Prediction

This machine learning project predicts real estate prices in Bangalore based on parameters like location, square footage, number of bedrooms (BHK), and bathrooms. It utilizes a trained Linear Regression model served via a Flask API and consumed by a responsive HTML/CSS/JavaScript frontend.

## 📂 Project Structure

```
ML-Project2/
├── client/                 # Frontend application
│   ├── app.html           # Main user interface
│   ├── app.css            # Styles
│   └── app.js             # Logic to communicate with backend
│
├── server/                 # Backend API
│   ├── artifacts/         # Trained model and column metadata
│   │   ├── banglore_home_prices_model.pickle
│   │   └── columns.json
│   ├── server.py          # Flask application entry point
│   ├── util.py            # Utility functions for loading artifacts & prediction
│   └── requirements.txt   # Python dependencies
```

## 🛠️ Tech Stack

- **Frontend**: HTML5, CSS3, JavaScript (jQuery), HTTP
- **Backend**: Python, Flask
- **Machine Learning**: Scikit-Learn (Linear Regression), NumPy, Pandas
- **Data Serialization**: Pickle, JSON

## 🚀 Setup & Installation

### Prerequisites
- Python 3.x installed

### 1. Install Backend Dependencies
Navigate to the server directory and install the required packages:

```bash
cd server
pip install -r requirements.txt
```
*Note: Key dependencies include `Flask`, `numpy`, and `scikit-learn`.*

### 2. Run the Flask Server
Start the backend server:

```bash
python3 server.py
```
You should see output indicating the server is running on `http://127.0.0.1:5000`.

### 3. Launch the Application
Simply open the `client/app.html` file in your preferred web browser.

## 📖 Usage

1. Open the web interface.
2. Select the **Area (Square Feet)**.
3. Choose the number of **BHK** (Bedrooms) and **Bathrooms**.
4. Select a **Location** from the dropdown list.
5. Click **Estimate Price**.
6. The predicted price will be displayed in Lakhs.
