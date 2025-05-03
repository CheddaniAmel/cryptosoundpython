# 🔐 Hybrid Audio Encryption with Visualization

This project demonstrates a **hybrid encryption system** for audio files, using **AES + RSA**, implemented and tested on **Google Colab**. It includes visualization of the waveform before and after encryption, and optionally uses **Whisper by OpenAI** to transcribe the audio content.

---

## 🎯 Objectives

- Encrypt audio signals using **AES symmetric encryption**
- Secure the AES key using **RSA asymmetric encryption**
- Visualize the **original** and **simulated encrypted** audio waveforms
- Transcribe the audio file using **OpenAI Whisper** (optional)

---

## 🧪 What We Did

### ✅ Step 1: Load and Visualize the Original Audio

- Imported a `.wav` file (converted from `.mp3` if needed)
- Used `scipy.io.wavfile` and `matplotlib` to extract and plot the original waveform

### ✅ Step 2: Hybrid Encryption of the Audio

- Generated a **random AES key** to encrypt the audio data (in EAX mode)
- Created an **RSA key pair**
- Encrypted the AES key with the **RSA public key**
- Result: AES-encrypted audio + RSA-encrypted key

### ✅ Step 3: Simulated Visualization of Encrypted Signal

- Encrypted audio is binary and unreadable
- Simulated a waveform using scrambled amplitude values to compare with original

### ✅ Step 4 (Optional): Transcription with Whisper

- Used OpenAI’s Whisper model to transcribe the `.wav` file
- Verified original voice content (before encryption)

---

## 📁 Files
- `test.wav`: Example audio file used for testing
- `README.md`: Project documentation

---


