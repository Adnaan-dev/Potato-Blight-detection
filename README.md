# 🥔 Potato Blight Detection Web App

An AI-powered web application that detects potato blight diseases using machine learning. The app can identify Early Blight, Late Blight, and healthy potato leaves with high accuracy.

## 🌟 Features

- **AI-Powered Detection**: Uses a trained TensorFlow model for accurate disease detection
- **Modern UI/UX**: Beautiful, responsive design with drag-and-drop file upload
- **Real-time Preview**: See your uploaded image before analysis
- **Detailed Results**: Get confidence scores and treatment recommendations
- **Error Handling**: Comprehensive validation and user-friendly error messages
- **Mobile Responsive**: Works perfectly on all devices

### Screenshots 
![User Interface](https://github.com/user-attachments/assets/d7f765b7-37ad-4cb1-a44f-6c016007501a)
![Analyzing Disease](https://github.com/user-attachments/assets/ffc14633-175e-40f3-9708-140a84d2e55d)
![Results](https://github.com/user-attachments/assets/2a9c760f-8e35-43ea-9600-aa1470fc733b)


## 🚀 Quick Start

### Prerequisites

- Python 3.7 or higher
- pip (Python package installer)

### Installation

1. **Clone or download this repository**
   ```bash
   git clone <your-repo-url>
   cd potato-blight-detection
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Ensure your model file is present**
   - Make sure `potato_blight_detection_model.h5` is in the root directory
   - This should be your trained TensorFlow model

4. **Run the application**
   ```bash
   python app.py
   ```

5. **Open your browser**
   - Navigate to `http://localhost:5000`
   - Start uploading potato leaf images!

## 📁 Project Structure

```
potato-blight-detection/
├── app.py                              # Main Flask application
├── potato_blight_detection_model.h5    # Trained TensorFlow model
├── requirements.txt                    # Python dependencies
├── README.md                          # This file
└── templates/
    └── index.html                     # Web interface template
```

## 🔧 Configuration

### Model Requirements
- Input size: 180x180 pixels
- Color channels: RGB (3 channels)
- Normalization: Values scaled to 0-1 range
- Classes: ['Potato___Early_blight', 'Potato___Late_blight', 'Potato___healthy']

### File Upload Settings
- **Supported formats**: PNG, JPG, JPEG, GIF, BMP
- **Maximum file size**: 16MB
- **Image processing**: Automatically resized to 180x180 pixels

## 🎯 How to Use

1. **Upload an Image**
   - Click the upload area or drag and drop a potato leaf image
   - Supported formats: PNG, JPG, JPEG, GIF, BMP

2. **Preview & Analyze**
   - Review your uploaded image
   - Click "Analyze Image" to run the detection

3. **View Results**
   - Get the disease classification (Healthy, Early Blight, or Late Blight)
   - See confidence percentage
   - Read treatment recommendations if disease is detected

## 🛠️ Technical Details

### Backend (Flask)
- **Framework**: Flask 2.3.3
- **ML Library**: TensorFlow 2.13.0
- **Image Processing**: Pillow 10.0.0
- **File Handling**: Werkzeug 2.3.7

### Frontend
- **HTML5**: Semantic markup
- **CSS3**: Modern styling with gradients and animations
- **JavaScript**: Interactive file upload and preview
- **Font Awesome**: Icons for better UX

### Model Architecture
- **Type**: Convolutional Neural Network (CNN)
- **Input**: 180x180x3 RGB images
- **Output**: 3-class classification
- **Preprocessing**: Image normalization and resizing

## 🔒 Security Features

- **File Validation**: Only image files are accepted
- **Size Limits**: Maximum 16MB file size
- **Secure Filenames**: Prevents directory traversal attacks
- **Temporary Storage**: Images are deleted after processing
- **No Data Persistence**: User images are not stored permanently

## 🐛 Troubleshooting

### Common Issues

1. **Model not loading**
   - Ensure `potato_blight_detection_model.h5` exists in the root directory
   - Check that the model file is not corrupted
   - Verify TensorFlow version compatibility

2. **File upload errors**
   - Check file format (must be image file)
   - Ensure file size is under 16MB
   - Try a different image format

3. **Prediction errors**
   - Verify image quality and clarity
   - Ensure the image shows a potato leaf
   - Try cropping the image to focus on the leaf

### Error Messages

- **"Model not loaded properly"**: Check model file presence and integrity
- **"Invalid file type"**: Upload only image files (PNG, JPG, etc.)
- **"No file selected"**: Select a file before clicking analyze
- **"Error processing image"**: Image may be corrupted or unsupported

## 📊 Performance

- **Prediction Time**: ~1-3 seconds per image
- **Memory Usage**: ~200-500MB (depending on model size)
- **Concurrent Users**: Supports multiple simultaneous users
- **File Processing**: Automatic resizing and optimization

## 🔮 Future Enhancements

- [ ] Batch image processing
- [ ] Model accuracy metrics display
- [ ] Historical prediction logs
- [ ] API endpoint for external integration
- [ ] Mobile app version
- [ ] Additional crop disease detection

## 📝 License

This project is open source and available under the MIT License.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📞 Support

If you encounter any issues or have questions:
1. Check the troubleshooting section above
2. Review the error messages in the application
3. Ensure all dependencies are properly installed
4. Verify your model file is compatible

---


## 📢 Connect with Me
[![GitHub](https://img.shields.io/badge/GitHub-black?logo=github&logoColor=white)](https://github.com/Adnaan-dev)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jan-adnan-farooq-b216b7321/)

⭐ **Star this repository if you find it useful!** 🚀


**Happy Farming! 🌱**

*Built with ❤️ by Adnan for potato farmers worldwide*

