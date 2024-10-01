# Voice-Based Medical Diagnostic System Using Bayesian Networks and Speech Recognition

---

## Overview

This project demonstrates a **voice-based medical diagnostic system** that integrates **Bayesian networks** for probabilistic reasoning and **speech recognition** for user interaction. The system helps diagnose common conditions like **Flu**, **COVID-19**, **Heart Disease**, and **Pneumonia** by interpreting spoken symptoms. Using Python's `pgmpy` and `SpeechRecognition` libraries, it processes voice input, identifies symptoms, and applies Bayesian inference to provide diagnostic results.

---

## Introduction

Voice-activated diagnostic tools are becoming an important part of modern healthcare, enabling hands-free and accessible patient interaction. This project combines **speech recognition** to gather patient responses and **Bayesian networks** to analyze symptoms, offering real-time diagnostic suggestions. The system uses voice-based interactions to ask patients about symptoms and performs probabilistic reasoning to make accurate diagnostic predictions.

---

## Methodology

1. **Speech Recognition**: The system captures spoken input via the microphone, converts it into text, and processes simple "Yes" or "No" answers using the **SpeechRecognition** library.
2. **Bayesian Network**: A **Bayesian network** is constructed to model relationships between diseases and symptoms. The network performs probabilistic reasoning to infer the most likely diagnosis based on the symptoms provided by the patient.
3. **Inference Process**: Once the symptoms are mapped, the system uses **variable elimination** in the Bayesian network to compute the likelihood of each disease, providing a diagnosis.

---

## How It Works

1. The system asks the patient a series of questions (e.g., "Do you have a fever?").
2. The patient responds using voice, and the system captures the answer ("Yes" or "No").
3. The Bayesian network processes these responses to infer the most probable disease.
4. The system returns a diagnosis based on the patient's symptoms.

---

## Results

In controlled tests, the system successfully provided accurate diagnoses based on the patient's spoken symptoms. The speech recognition component performed well in a quiet environment, and the Bayesian network accurately predicted diagnoses for conditions like COVID-19 and Heart Disease.

---

## Future Improvements

- **Noise Handling**: Improve speech recognition in noisy environments.
- **Expanded Diagnoses**: Add more diseases and symptoms to the Bayesian network.
- **Multilingual Support**: Extend the system to support multiple languages for broader use.

---

## Conclusion

This project illustrates the potential of combining **Bayesian networks** with **speech recognition** for a voice-based medical diagnostic system. The system offers an accessible, real-time solution for preliminary medical diagnosis, suitable for remote healthcare applications.

---

## Dependencies

- **pgmpy**: For building and working with **Bayesian networks**.
- **SpeechRecognition**: For **speech-to-text** conversion using the **Google Web Speech API**.
- **Python Libraries**: `sklearn`, `matplotlib`, and `seaborn` for evaluation and visualization.

---

## References

- Pearl, J. (1988). *Probabilistic Reasoning in Intelligent Systems*.
- Korb, K. B., & Nicholson, A. E. (2010). *Bayesian Artificial Intelligence*.
- Davis, S., & Mermelstein, P. (1980). *Parametric Representations for Monosyllabic Word Recognition*.
- Rabiner, L. R., & Juang, B. H. (1993). *Fundamentals of Speech Recognition*.
