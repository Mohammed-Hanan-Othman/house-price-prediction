# 🏡 Household Price Prediction

This project focuses on building a regression model to predict household prices based on various features.The analysis and modeling are done using Python in a Jupyter Notebook, with the final model saved in the `models/` folder for reuse.

## 📁 Project Structure

<pre>
.
├── data/ lData set links
├── models/ # Saved trained models (pickle file)
├── notebooks/ # Jupyter Notebook used for analysis
│ └── house_price_prediction.ipynb
├── README.md # This file
└── .gitignore # Files to ignore
</pre>


##  📊 Dataset
The dataset includes various features influencing household prices. A few columns:
- `date`: The date when the property was sold.
- `price`: The target variable (Sale price of the house in USD).
- `bedrooms`: The number of bedrooms in the house.
- `bathrooms`: The number of bathrooms in the house.
- `sqft_living`: The size of the living area (in square feet).
- `sqft_lot`: The size of the lot (in square feet).
- `floors`: The number of floors of the house.
- `sqft_basement`: The size of the basement (in square feet).
- `city`: The city where the property is located.

Refer to the `data/` folder for details


## 🚀 How to Run

1. **Clone the repository:**
```bash
git clone https://github.com/Mohammed-Hanan-Othman/house-price-prediction.git
cd house-price-prediction
```

2. **Installation and Setup:**
This assumes an anaconda environment.

3. **Open notebook**
``` bash
jupyter notebook notebooks/house_price_prediction.ipynb
```

4. **Run:**
    - Run all cells to reproduce the results.
    - Alternatively, create a new `.py` file and load the saved models from the `.models/` folder to make predictions



## 🧠 Model Overview

Different models would be used here:
1. **Base Model:**
    - Model type: Regression (using Ridge Regression with cross validation).
    - Notebook: [Base Model](./notebooks/house_price_prediction.ipynb)
    - Preprocessing:
        - Handling missing values.
        - One-hot encoding categorical features with `OneHotEncoder`.
        - Feature scaling using `Standard Scaler`.
    - Evaulation Metrics:
        - Mean Absolute Error
    - Model Output: Model trained and saved as a `.pkl` file in `.models/` folder.
    - Comments and issues:
        - Outliers removed before test_train split.
        - Removed outliers leading to reduced data points for training.
    - 📈 Results:
        - Baseline MAE: 156483.52018618677
        - Training MAE: 83527.15396181149


## 📌 Future Improvements
- Try more advanced models (e.g. Gradient Boosting).
- Evaluate model on new unseen data or deploy via a simple web API.

## Contributing
Contributions are welcome. To contribute:

- Fork the repository
- Create a new branch (git checkout -b feature-xyz)
- Commit your changes (git commit -am 'Add new feature')
- Push to the branch (git push origin feature-xyz)
- Open a Pull Request

Contributors
- GitHub: @your-username – Initial work

Feel free to open issues or suggestions via GitHub Issues.

## 📄 License
This project is for educational purposes only. Feel free to use and share.

## 👨‍💻 Author
- GitHub: @Mohammed-Hanan-Othman