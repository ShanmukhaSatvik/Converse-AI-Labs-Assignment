# Converse AI Labs Assignment - Call Quality Analyzer

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ShanmukhaSatvik/Converse-AI-Labs-Assignment/blob/main/ConversAILabs.ipynb)

---

## 📄 Project Overview

This project implements a **Call Quality Analyzer** using Python in Google Colab. The system analyzes sales call recordings and produces key metrics to evaluate call performance. It leverages **OpenAI Whisper** for transcription and **TextBlob** for NLP-based analysis.

---

## 🚀 Features

The analyzer provides the following metrics:

1. **Talk-time ratio**  
   - Percentage of words spoken by each participant (Speaker 1 vs Speaker 2).

2. **Number of questions asked**  
   - Counts all question marks in the transcript.

3. **Longest monologue duration**  
   - Estimates the length of the longest continuous speech segment for a speaker (approx. in seconds).

4. **Call sentiment**  
   - Overall sentiment of the call: Positive, Negative, or Neutral.

5. **Actionable insight**  
   - Provides a simple recommendation based on the conversation (e.g., asking more open-ended questions).

6. **Bonus: Likely Sales Rep Identification**  
   - Uses keyword-based heuristics to detect which speaker is the sales representative.

---

## 🛠️ How It Works

1. **Upload Audio File**  
   - Users can upload a sales call recording (MP3, WAV, etc.) to the Colab notebook.

2. **Transcription**  
   - The audio is transcribed into text using **OpenAI Whisper**.

3. **Sentence Tokenization**  
   - The transcript is split into sentences using **TextBlob** for analysis.

4. **Talk-time and Monologue Analysis**  
   - Words are counted per speaker to calculate talk-time ratio.  
   - Consecutive sentences by the same speaker are grouped to compute the longest monologue duration.

5. **Sentiment Analysis**  
   - Overall polarity is computed using **TextBlob**, categorizing the call sentiment.

6. **Actionable Insight**  
   - Based on number of questions and sentiment, a simple recommendation is generated.

7. **Sales Rep Detection (Bonus)**  
   - Keywords related to sales (e.g., order, promotion, vehicle) are used to identify the likely sales representative.

---

## ⚡ How to Use

1. Open the notebook in Colab using the button above.
2. Upload your sales call audio file.
3. Run all notebook cells sequentially.
4. View the output metrics:
   - Talk-time ratio
   - Number of questions
   - Longest monologue duration
   - Call sentiment
   - Actionable insight
   - Likely sales rep (bonus)

---

## 📚 Libraries Used

- `openai-whisper` → Audio transcription  
- `textblob` → NLP tasks (tokenization, sentiment analysis)  
- `nltk` → Sentence tokenization backend (via TextBlob)  

---

## 📌 Notes

- The system is designed to work in **Google Colab free tier**.  
- Monologue duration and sales rep detection use simple heuristics for demonstration purposes.  
- For production use, speaker diarization libraries (e.g., `pyannote.audio`) can improve accuracy.

---

## 👨‍💻 Author

**Shanmukha Satvik**  
[GitHub Profile](https://github.com/ShanmukhaSatvik)
