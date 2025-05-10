
## 🤖 Human Activity Recognition with CNN-LSTM

Hi! This project is about recognizing human activities (like walking, sitting, and lying down) using data from smartphone sensors — and it’s built with a mix of **Convolutional Neural Networks (CNN)** and **LSTM**.

---

### 📂 What’s this dataset?

We used the **UCI HAR Dataset**, which was collected from people doing normal activities while carrying a smartphone in their pocket.  
The phone recorded motion through its sensors — accelerometer and gyroscope — and that’s what we use to figure out what the person was doing.

The activities we’re predicting are:
- Walking  
- Walking Upstairs  
- Walking Downstairs  
- Sitting  
- Standing  
- Laying

---

### 🧠 How does the model work?

The model uses a **CNN-LSTM** architecture:

- **CNN (Conv1D)** helps extract patterns from the sensor signals — like which direction the body is moving in.
- **LSTM** is used to understand how those patterns change over time (for example, walking has a repeating rhythm).

It’s like the CNN understands “what” is happening, and the LSTM understands “how” it changes with time.

---

### 📈 How well does it perform?

- The final accuracy on the test set was **89%**.  
- We also show:
  - Training and validation accuracy/loss plots  
  - A confusion matrix to see where the model gets confused  
  - Sensor signal plots to get a feel for the data

---

### 🖥️ How to run this?

If you want to try it out:

```bash
pip install numpy pandas matplotlib seaborn tensorflow
python activity_recognition.py
```

Make sure the UCI HAR Dataset is in the same directory (or adjust the paths accordingly).

---

### 🧰 Tools used

- Python  
- TensorFlow + Keras  
- Pandas, NumPy  
- Matplotlib & Seaborn for visualization

---

### 🙋‍♀️ Why this project?

This project is a good example of combining spatial and temporal deep learning techniques to solve real-world problems. Human Activity Recognition has applications in:
- Fitness tracking  
- Health monitoring  
- Smart homes  
- Elderly care

---

Hope you find it useful or interesting. Feel free to clone the repo, play around, or ask questions!
