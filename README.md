# Botnet Detection Using Machine Learning: Performance Investigation

## 📌 Project Overview
This project focuses on detecting botnet activity within a cloud or Software Defined Networking (SDN) environment using machine learning techniques. Botnets, which are networks of compromised devices, pose serious threats to network security. Traditional methods struggle to detect them effectively, especially in scalable, dynamic environments like SDN. This system uses ML models to classify traffic patterns and detect malicious behavior with high accuracy.

---

## 🎯 Objectives
- Develop an ML-based system for detecting botnet activity in SDN environments.
- Analyze how cloud-specific or SDN-specific factors affect detection performance.
- Evaluate and compare the performance of multiple machine learning models.

---

## 🛠️ Technologies & Libraries
- **Python** – Main programming language
- **Pandas, NumPy** – Data manipulation and preprocessing
- **Scikit-learn** – Model training and evaluation
- **Matplotlib, Seaborn** – Data visualization

---

## 📂 Dataset Information
The dataset includes labeled SDN network traffic with the following important features:
- **pktcount, bytecount, pktrate, tot_kbps** – Indicators of traffic volume
- **flows, packetins, Pairflow** – Related to traffic sessions
- **tx_bytes, rx_bytes, tx_kbps, rx_kbps** – Directional flow rates
- **Protocol, port_no** – Type and port used for communication
- **label** – 0 (Normal) or 1 (Botnet)

---

## 🧠 Machine Learning Models Used
1. **Logistic Regression** – Linear baseline classifier
2. **Random Forest** – Ensemble of decision trees
3. **Extra Trees Classifier** – More randomized ensemble for higher performance
4. **Multinomial Naive Bayes** – Probabilistic classifier for comparison

---

## 📊 Results
- **Extra Trees Classifier** achieved the highest accuracy (~99.99%)
- **Random Forest** performed nearly as well
- **Logistic Regression** gave reasonable baseline performance
- **Naive Bayes** underperformed due to assumptions of feature independence

---

## 📈 Visualizations
- **Correlation Matrix** using Seaborn
- **Accuracy comparison** across models
- **Confusion matrix** for error analysis

---

## ✅ Key Findings
- Ensemble models outperform simpler classifiers for this task.
- Flow-level features like packet count, duration, and rate are highly effective for detecting botnets.
- High accuracy can be achieved even without deep packet inspection.

---

## 🔮 Future Scope
- Integrate model into live SDN controllers for real-time detection.
- Test with encrypted or obfuscated traffic.
- Expand dataset for generalized learning across different attack types.
- Explore deep learning models for further accuracy improvements.

---

## 👨‍💻 Contributors
1. Vipul Kumar
2. Leena Kaushik
3. Prashant Tomar

---

## 📜 License
This project is for academic and research purposes only.
