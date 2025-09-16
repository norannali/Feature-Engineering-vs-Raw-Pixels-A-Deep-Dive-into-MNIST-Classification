# MNIST: Features, Baseline, and Autoencoders

This project explores **MNIST handwritten digit classification** using different approaches:

1. **Engineered Features** – centroid, statistical features, symmetry, sparsity, and projections.  
2. **Raw Pixels (Baseline Model)** – using only flattened normalized pixel values.  
3. **Combined Model** – leveraging both engineered features and raw pixels.  
4. **Autoencoder** – for dimensionality reduction and latent space visualization using t-SNE.

---

## 📊 Dataset
- **MNIST** dataset of 70,000 grayscale handwritten digit images (28×28 pixels).  
- Split into:
  - **60,000 training images**
  - **10,000 testing images**

---

## ⚙️ Project Workflow
1. **Data Exploration & Visualization**  
   - Display random digit samples from MNIST.  
   - Count distribution of training & testing labels.  

2. **Feature Engineering**  
   - Extract centroid, intensity distribution, kurtosis, skewness, sparsity, and symmetry.  
   - Create a feature vector of **61 features per image**.

3. **Neural Network Models**  
   - Build and train:
     - Engineered Features Model  
     - Raw Pixel Baseline Model  
     - Combined Features Model  

4. **Autoencoder**  
   - Train an encoder-decoder to reconstruct images.  
   - Visualize latent space using **t-SNE**.

5. **Performance Comparison**  
   - Compare accuracy across models.  
   - Visualize results with bar charts and training history plots.

---

## 📈 Results

| Model                | Test Accuracy |
|-----------------------|---------------|
| Engineered Features   | ~0.941         |
| Raw Pixels Baseline   | ~0.979         |
| Combined Model        | ~0.983        |

- **Engineered features** capture spatial & statistical information.  
- **Baseline pixels** still perform strongly.  
- **Combined features** give the best performance.  
- **Autoencoder** successfully reconstructs digits and provides a meaningful latent representation.

---

## 🚀 Installation & Usage

### 1. Clone Repository
```bash
git clone https://github.com/norannali/Feature-Engineering-vs-Raw-Pixels-A-Deep-Dive-into-MNIST-Classification.git
cd mnist-features-autoencoder
````

### 2. Install Requirements

Make sure you have Python 3.x. Then install dependencies:

```bash
pip install -r requirements.txt
```

Example `requirements.txt`:

```
numpy
pandas
matplotlib
scikit-learn
scipy
tensorflow
keras
```

### 3. Run Notebook

Open the Jupyter Notebook:

```bash
jupyter notebook MNIST_Features_Autoencoder.ipynb
```

---

## 🖼️ Visualizations

* Sample MNIST digits
* Training vs Validation Loss/Accuracy plots
* Model performance comparison bar chart
* Autoencoder reconstruction (original vs reconstructed)
* t-SNE Latent Space visualization

---

## 📌 Key Takeaways

* Feature engineering can enrich model performance by capturing **spatial/statistical properties**.
* Baseline raw pixel models still perform strongly due to neural networks’ ability to learn directly from data.
* Combining both **handcrafted + learned features** yields better results.
* Autoencoders provide **compact latent representations** and meaningful visualizations.

---

## ✨ Future Work

* Experiment with **CNNs** for improved accuracy.
* Use **Variational Autoencoders (VAEs)** for generative tasks.
* Explore other dimensionality reduction methods (PCA, UMAP).

---

## 📝 Author

👤 Developed by Noran Ali (https://github.com/norannali)
💡 For educational purposes in **Deep Learning & Feature Engineering**.
