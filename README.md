# Smart Traffic Prediction System

A deep learning project that predicts Los Angeles highway
traffic speeds 30 minutes into the future using LSTM networks.

## Results
| Metric   | Value     |
|----------|-----------|
| MAE      | 5.46 mph  |
| RMSE     | 12.41 mph |
| MAPE     | 10.98 %   |
| Accuracy | 89.02 %   |

## Dataset
- METR-LA (207 sensors, 119 days, Los Angeles highways)
- Download from Kaggle:
  https://www.kaggle.com/datasets/annnnguyen/metr-la-dataset
- Place METR-LA.h5 and adj_METR-LA.pkl inside data/ folder

## Model Architecture
- Type         : 2 Layer LSTM
- Hidden units : 128
- Input        : 12 time steps (1 hour of history)
- Output       : 6 time steps  (30 minutes forecast)
- Parameters   : 1,024,512

## How to Run
1. Clone this repository
2. Install dependencies
3. Download dataset from Kaggle link above
4. Open notebook/smart_traffic_prediction.ipynb
5. Run all cells in order

## Installation
pip install -r requirements.txt

## Technologies Used
- Python 3.13
- PyTorch
- NumPy / Pandas
- Matplotlib / Seaborn
- Scikit-learn
- H5py

## Real World Applications
- Navigation apps like Google Maps
- Smart traffic signal control
- Emergency vehicle routing
- Ride sharing ETA prediction
- City traffic planning

## Future Improvements
- Add GCN layer for spatial road network learning
- Train on GPU for faster deeper training
- Include weather and event data as features
- Deploy as real time REST API using Flask
