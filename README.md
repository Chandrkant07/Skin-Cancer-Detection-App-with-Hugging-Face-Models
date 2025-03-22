# Skin Cancer Detection System

![Skin Cancer Detection System Banner](https://raw.githubusercontent.com/username/skin-cancer-detection/main/assets/banner.png)

## 🔬 Overview

The Skin Cancer Detection System is an advanced AI-powered web application designed to analyze skin lesion images and identify potential skin cancers and other skin conditions. This tool leverages deep learning and computer vision techniques to provide accessible skin lesion screening capabilities.

**Authors:**
- Subrata (Lead AI Developer)
- Chandrakanta (Medical Imaging Specialist)

## 🌟 Key Features

- **Advanced Image Analysis**: Utilizes a Vision Transformer (ViT) model specialized for skin lesion classification
- **ABCDE Rule Implementation**: Automated analysis of Asymmetry, Border, Color, Diameter, and Evolution
- **Comprehensive Results**: Provides detailed information about detected conditions with risk levels
- **Interactive Visualization**: Color-coded lesion detection and measurement visualizations
- **Educational Content**: Includes informational resources about different skin conditions
- **User-Friendly Interface**: Simple and intuitive design for users with any level of technical knowledge
- **Offline Capability**: Caches models locally for faster processing and offline use

## 📊 Technologies Used

- **Frontend**: Streamlit
- **Backend**: Python
- **Deep Learning**: PyTorch, Hugging Face Transformers
- **Computer Vision**: OpenCV, PIL
- **Data Visualization**: Plotly, Matplotlib
- **Image Processing**: NumPy, SciPy

## 📋 Requirements

```
python >= 3.8
streamlit >= 1.20.0
torch >= 1.10.0
torchvision >= 0.11.0
transformers >= 4.25.1
pillow >= 9.0.0
numpy >= 1.20.0
pandas >= 1.3.0
plotly >= 5.5.0
matplotlib >= 3.5.0
opencv-python >= 4.5.5
huggingface-hub >= 0.12.0
requests >= 2.27.0
```

## 🚀 Installation & Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/username/skin-cancer-detection.git
   cd skin-cancer-detection
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

4. Configure your Hugging Face API token:
   - Create a `.streamlit/secrets.toml` file with your token:
     ```toml
     hf_token = "your_hugging_face_token"
     ```

5. Run the application:
   ```bash
   streamlit run app.py
   ```

## 🔍 How It Works

### The Application Flow:

1. **Image Upload**: User uploads a skin lesion image or selects from examples
2. **Preprocessing**: The image is enhanced and prepared for analysis
3. **AI Analysis**: The processed image is passed through the skin lesion classifier model
4. **Feature Extraction**: Computer vision techniques extract key features for ABCDE analysis
5. **Risk Assessment**: The system evaluates the results and assigns a risk level
6. **Results Display**: Comprehensive results are shown with visual aids and recommendations

### The Model:

The core of the system is a fine-tuned Vision Transformer (ViT) model trained on the ISIC (International Skin Imaging Collaboration) dataset. This model can recognize various skin conditions including:

- Melanoma
- Basal Cell Carcinoma
- Squamous Cell Carcinoma
- Nevus (common mole)
- Seborrheic Keratosis
- Actinic Keratosis

## 📱 Usage

1. Launch the application
2. Upload a skin lesion image or select an example
3. Click the "Analyze Image" button
4. Review the detailed analysis results
5. Check the lesion detection visualization and ABCDE assessment
6. Read the condition information and follow-up recommendations

## ⚠️ Disclaimer

This tool is for educational and screening purposes only. It is not intended to replace professional medical advice, diagnosis, or treatment. Always consult a qualified healthcare provider for proper evaluation of skin conditions.

## 🔧 Troubleshooting

If you encounter issues with model downloading:
1. Ensure your Hugging Face token is correctly set up
2. Check your internet connection
3. The application includes fallback models that will be used automatically if the primary model fails

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request or open an Issue to suggest improvements or report bugs.

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🔗 Citations

If you use this code in your research, please cite:

```
@software{SubrataChandrakanta2023,
  author = {Subrata, and Chandrakanta},
  title = {Skin Cancer Detection System},
  year = {2023},
  url = {https://github.com/username/skin-cancer-detection}
}
```

