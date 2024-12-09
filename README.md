# Fact-Audio-Generator

This project demonstrates a complete pipeline for generating facts using a GPT-2 model, cleaning the generated text, identifying and correcting errors, and finally converting the corrected text into speech.

## Features

1. **Fact Generation**:
   - Leverages the GPT-2 language model to generate interesting facts or sentences.

2. **Text Cleaning**:
   - Removes unwanted characters (e.g., punctuation, brackets) and ensures the text is in a clean, single-sentence format.

3. **Error Detection and Correction**:
   - Implements two methods to identify and correct grammatical and spelling errors:
     - **Method 1**: Using `transformers` pipeline for text correction.
     - **Method 2**: (if applicable) An additional approach for comparison.

4. **Text-to-Speech Conversion**:
   - Converts the corrected text into audio using a text-to-speech pipeline.

---

## Project Workflow

1. **Generate Facts**:
   - The notebook uses a pre-trained GPT-2 model to generate text-based facts.

2. **Clean Text**:
   - The raw generated text is cleaned by removing unwanted characters like `, . " ) ( { }`.
   - Outputs a simplified version of the text.

3. **Error Detection and Correction**:
   - Uses error correction models to fix grammatical and spelling issues in the cleaned text.

4. **Generate Audio**:
   - Converts the final corrected text into audio and saves it as a `.wav` file.
   - Plays the audio file in the notebook for immediate feedback.

---

## Getting Started

### Prerequisites

- Python 3.8 or above
- Libraries:
  - `transformers`
  - `torch`
  - `datasets`
  - `soundfile`
  - `IPython`

Install dependencies using:

```bash
pip install transformers torch datasets soundfile ipython
