# StressDetetction

### **Overview**

This system detects stress levels based on real-time physiological data collected from a **GSR (Galvanic Skin Response) sensor** and a **temperature sensor** using an **ESP32 microcontroller**. The ESP32 transmits the data via its **Wi-Fi module** to a web-based platform, where machine learning (ML) models analyze the data to determine the user's stress level.

### **How It Works**

1. **User Authentication**:
    - Users log in or sign up on the web platform.
    - Their personal data and baseline values are stored securely.
2. **Baseline Calculation (30-90 seconds)**:
    - When the user visits the webpage and clicks **"Calculate Baseline"**, the system collects GSR and temperature sensor data while the user is in a relaxed state.
    - The ML model determines the user’s baseline values for **normal physiological conditions**.
    - These baseline values are stored in a database for future stress evaluations.
3. **Real-Time Stress Measurement**:
    - When the user clicks **"Measure Stress Level"**, new sensor readings are taken and transmitted via ESP32 Wi-Fi.
    - The ML model, trained on a labeled dataset, compares these values to the baseline and predicts the stress level as **Level 1 (Low), Level 2 (Moderate), or Level 3 (High)**.
    - The stress level is displayed on the web dashboard.

### **Key Features**

✅ **ESP32 with Wi-Fi Communication**

✅ **Machine Learning-Based Stress Prediction**

✅ **User Authentication for Personalized Data**

✅ **Baseline Calculation for Individualized Stress Detection**

✅ **Real-Time Sensor Data Visualization on Web Dashboard**
