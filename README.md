
# 🧱 3D Model Generation from Image or Text

This project generates 3D models either from an **image** (via depth estimation and mesh reconstruction) or from a **text prompt** (using OpenAI's Shap-E).

---

## 📦 Requirements

Install all dependencies by running:

```bash
pip install torch torchvision torchaudio transformers pillow matplotlib open3d accelerate trimesh pyrender
pip install git+https://github.com/openai/shap-e.git
```

---

## 📁 Project Structure

```
3d_model/
├── 3d_model.ipynb         # Main Jupyter notebook
├── requirements.txt       # List of required Python packages
└── README.md              # This file
```

---

## 🚀 How to Run

1. **Launch Jupyter Notebook** in the `3d_model` folder:

   ```bash
   jupyter notebook
   ```

2. **Open** the `3d_model.ipynb` file.

3. **Run all cells** in order.

4. **Follow the prompt**:
   - Enter `image` when asked for mode.
   - Provide the **full path** to a `.jpg` file, like:

     ```
     C:\Users\Snehith Kumar\DATA\my_desk.jpg
     ```

     ⚠️ Do **not** include any quotes (`"`), and make sure the image is in `.jpg` format.

---

## 📌 Notes

- The `image` mode uses a depth estimation model to generate a 3D mesh from a single image.
- The `text` mode uses OpenAI's Shap-E to create a 3D mesh based on a descriptive prompt (e.g., *"a futuristic car"*).
- Output meshes are saved in the `output/` directory.

---

## 📝 License

This project is for educational and research purposes only. Use the models responsibly.
