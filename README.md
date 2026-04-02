# Measuring 🗣️ Speech-to-Text 👨‍💻 Accuracy (ASR Evaluation)

## 📌 Overview
Automated Speech Recognition (ASR), also known as Speech-to-Text, converts spoken audio into written text using machine learning. While powerful, ASR systems are not perfectly accurate, making it essential to evaluate transcription quality—especially in critical applications like virtual assistants, call centers, and medical dictation.

This project demonstrates how to measure ASR accuracy using standard evaluation metrics such as **Word Error Rate (WER)**.

---

## 🎯 Objectives
- Understand how speech recognition accuracy is defined
- Learn how to measure transcription quality
- Implement Word Error Rate (WER) calculation
- Evaluate machine-generated transcripts against ground truth

---

## 🧠 Key Concepts

### 📊 Speech Accuracy
Speech accuracy refers to how closely a machine-generated transcription matches a human (ground truth) transcription.

### 📄 Ground Truth
The **ground truth** is a 100% accurate transcription, typically created by humans, used as a benchmark for evaluation.

---

## 📉 Word Error Rate (WER)

WER is the industry-standard metric used to evaluate ASR systems.

### 🔢 Formula

<img width="295" height="118" alt="Wer" src="https://github.com/user-attachments/assets/3379ad82-ffa4-4ca1-8dfb-854337f3ba62" />


Where:
- **S** = Substitution errors  
- **D** = Deletion errors  
- **I** = Insertion errors  
- **N** = Total number of words in the ground truth  

### ⚠️ Error Types
- **Insertion Error**: Extra word added  
- **Substitution Error**: Incorrect word used  
- **Deletion Error**: Missing word  

> Lower WER = Higher accuracy  
> WER can exceed 100% in extreme cases

---

## 📌 Additional Metrics
- **Jaccard Index**: Measures similarity between transcripts  
- **F1 Score**: Balances precision and recall for key terms  

---

## 🔍 Workflow

### 1. Gather Audio Data
- Use realistic, representative audio samples
- Recommended: 30 minutes to 3 hours of audio

### 2. Prepare Ground Truth
- Create accurate human transcriptions
- Ensure consistency in formatting (punctuation, numbers, etc.)

### 3. Generate Machine Transcription
- Use Google Speech-to-Text API to transcribe audio

### 4. Compute WER
- Compare machine output with ground truth
- Count errors and calculate WER

---

## 🛠️ Technologies Used
- Google Cloud Speech-to-Text API
- Python (for processing and evaluation)
- WER calculation scripts (provided by Google)

---

## 📂 Project Structure

```
├── data/
│ ├── audio/ # Input audio files
│ └── transcripts/ # Ground truth transcripts
├── scripts/
│ ├── transcribe.py # Speech-to-Text processing
│ └── wer_calculation.py # WER computation
├── results/
│ └── evaluation_report.txt
└── README.md
```

---

## 🚀 How to Run

1. Clone the repository:

```
git clone https://github.com/hemant467/Measuring-Speech-to-Text-Accuracy.git

cd asr-accuracy-evaluation
```

2. Install dependencies:

```
pip install -r requirements.txt
```

3. Run transcription:

```
python scripts/transcribe.py
```

4. Calculate WER:

```
python scripts/wer_calculation.py
```

---

## 📈 Example Output

WER: 0.18 (18% error rate)
Insertions: 5
Deletions: 8
Substitutions: 10


---

## ✅ Use Cases
- Call center transcription analysis  
- Subtitle generation quality checks  
- Voice assistant performance evaluation  
- Dictation software testing  

---

## 📚 References
- Google Cloud Speech-to-Text Documentation  
- Standard ASR evaluation methodologies  

---

## 🤝 Contributing
Contributions are welcome! Feel free to open issues or submit pull requests.

---

## 📜 License
This project is licensed under the MIT License.

---

## 👨‍💻 Author

Hemant Katta

---

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com/?lines=Measuring+🗣️+Speech-to-Text+👨‍💻+Accuracy+(ASR+Evaluation)&font=Fira%20Code&color=%23FFD700&center=true&width=900&height=130&size=26&pause=1000">
</p>
