🌊 Water Body Detection from Satellite Imagery

This project detects water bodies from satellite imagery using:

    Spectral Indices (MNDWI) based thresholding

    Deep Learning (CNN/U-Net) segmentation

    Both synthetic data and real Landsat/Sentinel data

📂 Project Structure

├── water_body_detection/
│   ├── synthetic_mndwi_detection.py   # MNDWI water detection using synthetic data
│   ├── real_landsat_mndwi_detection.py # Water detection from real Landsat data (rasterio)
│   ├── deep_learning_water_detection.py # Water segmentation using CNN (U-Net)
│   ├── README.md
│   └── requirements.txt

🚀 How to Run

    Clone the Repository

git clone https://github.com/your-username/water-body-detection.git
cd water-body-detection

    Install Dependencies

pip install -r requirements.txt

    Run Scripts

    Synthetic MNDWI Detection

python synthetic_mndwi_detection.py

Real Landsat Data Detection

python real_landsat_mndwi_detection.py

Deep Learning Water Detection

    python deep_learning_water_detection.py

📚 Methods Used
1. Spectral Index - MNDWI

    Modified Normalized Difference Water Index (MNDWI) formula:
    MNDWI=Green−SWIR1Green+SWIR1
    MNDWI=Green+SWIR1Green−SWIR1​

    Water bodies typically have MNDWI > 0.

2. CNN/U-Net Deep Learning

    U-Net model segments water bodies from satellite images.

    Trained on synthetic masks; can be extended to real-world datasets.

🛰️ Data Sources

    Synthetic Data: Randomly generated for model prototyping

    Real Data:

        USGS EarthExplorer - Landsat 8/9

        Google Earth Engine

📈 Example Results
Input Image	Ground Truth Mask	Predicted Water Mask
	
	
📋 Requirements

List of Python packages:

tensorflow
numpy
matplotlib
rasterio
scikit-learn
opencv-python

💡 Future Work

    Integrate Sentinel-2 MSI datasets

    Train CNN model on real labeled water datasets (e.g., GSW)

    Deploy using Streamlit dashboard

    Add cloud masking for Landsat/Sentinel images

👨‍💻 Author

    Your Name — GitHub | LinkedIn

📝 License

This project is licensed under the MIT License. See the LICENSE file for details.
✅ Quick Badge

    Water Detection 🔵 | Deep Learning 🧠 | Satellite Imagery 🛰️
