# FashionLens 👗👕

An AI-powered **content-based image recommender system** that suggests similar fashion items using **ResNet50 feature extraction** and **k-NN search**.

## 📌 Features
- **ResNet50** (ImageNet pretrained) for feature extraction
- **k-Nearest Neighbors** for finding visually similar images
- **Streamlit** web interface for easy interaction
- **OpenCV** & **PIL** for image handling
- **Pickle**-based storage for precomputed embeddings

---

## 📂 Project Structure
```
├── app.py              # Extracts features from images & saves embeddings
├── main.py             # Streamlit UI for uploading and recommending
├── test.py             # Testing recommendation on a sample image
├── images/             # Fashion dataset images
├── uploads/            # Uploaded images folder
├── embeddings.pkl      # Precomputed feature vectors
├── filenames.pkl       # Corresponding image filenames
├── requirements.txt    # Dependencies
└── README.md
```

---

## 🚀 How to Run

### 1️⃣ Clone the repository
```bash
git clone https://github.com/VRAJ2202/FashionLens.git
cd FashionLens
```

### 2️⃣ Install dependencies
```bash
pip install -r requirements.txt
```

### 3️⃣ Download Dataset
We use the **Fashion Product Images Dataset** from Kaggle:
🔗 [Download from Kaggle](https://www.kaggle.com/datasets/paramaggarwal/fashion-product-images-dataset)

Place the downloaded images inside the `images/` folder.

### 4️⃣ Extract features
```bash
python app.py
```
This will generate:
- `embeddings.pkl`
- `filenames.pkl`

### 5️⃣ Run the Streamlit app
```bash
streamlit run main.py
```

### 6️⃣ Test with a sample image (optional)
```bash
python test.py
```

---

## 📷 Screenshot
![Working Demo](assets/working_screenshot.png)

> The above screenshot shows the interface where you can upload an image and receive visually similar fashion item recommendations.

---

## 🛠 Tech Stack
- **Python 3.8+**
- **TensorFlow / Keras**
- **Streamlit**
- **scikit-learn**
- **NumPy / PIL / OpenCV**

---

## 📜 License
This project is licensed under the MIT License.
