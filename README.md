## 🗣️ End-to-End Bengali Speech Transcription

A final year(CSE465) project focused on developing an efficient and accurate Automatic Speech Recognition (ASR) system for the Bangla language. Given the challenges of limited resources and high Word Error Rates (WER) in Bangla, we implemented and compared both custom and fine-tuned transformer-based ASR models.

### 🔍 Key Highlights
- 📌 Developed a custom CTC-based ASR model trained from scratch.
- 📌 Fine-tuned OpenAI's Whisper-Small model for Bangla speech transcription using LoRA with 8-bit quantization.
- 📌 Used Mozilla Common Voice (Bangla subset) dataset with over 64 hours of validated audio.
- 📌 Achieved a WER of **18.57%** with the fine-tuned Whisper-Small model.

### 🛠️ Technologies & Tools
- Python, PyTorch, Hugging Face Transformers, Librosa, Torchaudio, JiWER
- Google Colab Pro+ for training and experimentation

### 📊 Results
| Model             | Best WER (%) |
|------------------|---------------|
| CTC-Based Model  | 55.56         |
| Whisper-Small (LoRA) | **18.57**     |

### 📂 Dataset
- **Common Voice Bangla v11**
- 461 total hours, 64 validated hours, 20,866 unique voices

### 🤖 Model Architecture
- **Custom CTC-Based Model:** 2D CNNs → Bi-GRUs → Dense Layer → Softmax
- **Whisper-Small:** Fine-tuned with LoRA adapter (1.44% trainable parameters)

### 📈 Conclusion
Our project demonstrates that transformer-based models like Whisper can be fine-tuned effectively even with limited resources to support Bangla ASR tasks. This can be foundational for building robust Bangla voice-driven applications.

🔗 [View Full Report (PDF)](./CSE_465_final%20Project%20Report.pdf)

