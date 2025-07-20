### **Project Title and Team**
*   **Project Name:** CleanTech - Transforming Waste Management through Transfer Learning
*   **Team ID:** LTVIP2025TMID45663
*   **Team Size:**4
*   **Team Leader:**Nasiruddin Sayyad
*   **Team Members:** Himasree, Dlisha Begum, Nasiruddin Sayyad, Dharmesh (as per Sprint Planning section).

### **Project Overview**
*   **Goal:** To develop a smart waste classification system that automatically identifies and categorizes waste as recyclable or non-recyclable using deep learning techniques.
*   **Technology:** Leverages image data and Transfer Learning with pre-trained CNN architectures (ResNet50, EfficientNetB0, and VGG16 as per source code) fine-tuned for waste classification.
*   **Purpose:** To support sustainable waste management practices by enabling smart segregation at the source, minimize human intervention, and promote environmentally friendly practices.

### **Features**
*   **Automated Waste Classification:** Classifies waste into recyclable and non-recyclable categories.
*   **Transfer Learning Application:** Utilizes pre-trained models (ResNet50, EfficientNetB0, VGG16) to train a robust classification model with limited data, saving computational time and effort.
*   **User-Friendly Web Interface:** Allows users to upload waste images and receive real-time classification results.
*   **Performance Metrics:** Assesses model effectiveness using accuracy, precision, recall, and F1-score.
*   **Scalability:** Designed to be scalable for a large user base and data volume, adaptable for other classification tasks, and easily scalable across cities and regions.
*   **Reporting and Analytics:** Provides visual waste statistics, downloadable reports, and trend analysis over time.
*   **User Feedback Mechanism:** Allows users to submit ratings and comments for classifications.
*   **Admin Module:** Enables viewing all classifications, managing users, and managing feedback.

### **Project Structure (Implied from Source Code and Description)**
*   **Root Directory (Implied):** `CleanTech_App/` (or similar)
    *   `app.py`: Main Flask application script for the web interface and prediction API.
    *   `vgg16.h5`: The trained deep learning model file (specifically VGG16 mentioned in the source code).
    *   `templates/`: Contains HTML templates.
        *   `index.html` (mentioned as the single-page application served).
    *   `static/`: Contains static assets.
        *   `uploads/`: Directory for temporarily storing uploaded images.

### **Installation and Setup (Local - Inferred from `app.py` comments)**
*   **Prerequisites:** Python, Flask, TensorFlow, NumPy, Pillow, Werkzeug.
*   **Setup Instructions:**
    *   Save `app.py` in the project's root directory.
    *   Ensure `vgg16.h5` is in the same directory as `app.py`.
    *   Ensure `templates` folder (with `index.html`) and `static` folder (with `uploads` subfolder) exist.
    *   Install required Python libraries: `pip install Flask tensorflow numpy Pillow werkzeug`
    *   Run the application: `python app.py`
    *   Access in browser: `http://127.0.0.1:2222`

### **Usage**
*   Users can upload waste images through the web interface.
*   The system classifies the image as recyclable or non-recyclable.
*   Real-time classification results are displayed.
*   Users can view visual statistics and download reports.

### **Model Details**
*   **Architecture:** Utilizes pre-trained CNN architectures such as ResNet50, EfficientNetB0, and specifically VGG16 (as per the provided `app.py` source code).
*   **Dataset:** Not explicitly detailed in terms of size or source, but implies image data of waste items.
*   **Training:** Trained using transfer learning on Google Colab.
*   **Accuracy:** Test Accuracy Score: 0.7436.
*   **Loss:** Test Loss: 0.5594.
*   **Confusion Matrix:**
    *   True Positives: 18 (Recyclable), 12 (Non-Recyclable)
    *   False Positives: 5 (incorrectly classified as Recyclable), 5 (incorrectly classified as Non-Recyclable)
    *   Total test samples: 40.
*   **Model File:** `vgg16.h5` (as per the provided `app.py` source code).

### **Deployment**
*   **Cloud Deployment:** Future scope includes hosting the model on cloud platforms for scalability and accessibility.
*   **Project Demo Link:** `https://drive.google.com/file/d/1N6nkJQK2RcWDZplj65A0YhFGgxv-rvwR/view?usp=drive_link`
*   **GitHub Link:** `https://github.com/DharmeshNageti/CleanTech-Transforming-Waste-Management-with-Transfer-Learning`

### **Future Scope**
*   Dataset Expansion
*   Mobile App Development
*   Active Learning
*   Integration with Smart Bins
*   Analytics Dashboard
*   Multi-class Classification
*   Cloud Deployment
