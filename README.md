# Character-Level Handwritten Text Generation using RNN

## Project Overview

This project implements a **Character-Level Recurrent Neural Network (RNN)** using PyTorch to generate handwritten-style text. The model is trained on text transcriptions from the **IAM Handwritten Text Dataset** and learns character patterns, word structures, punctuation, and sentence formations.

After training, the model can generate new text sequences character-by-character based on the learned patterns.

---

## Objectives

* Implement a Character-Level Recurrent Neural Network (RNN).
* Train the model on handwritten text transcriptions.
* Learn character-level dependencies from the dataset.
* Generate new text based on learned patterns.

---

## Dataset

**Dataset:** IAM Handwritten Text Dataset

Source:
https://huggingface.co/datasets/Teklia/IAM-line

The dataset contains:

* Handwritten line images
* Corresponding text transcriptions

For this project, only the text transcriptions are used for training the RNN.


## Github Link
https://github.com/nithika1405/customer-churn-prediction

---

## Project Structure

```text
handwriting_rnn/
│
├── data/
│   ├── dataset.json
│   └── corpus.txt
│
├── models/
│   └── char_rnn.pth
│
├── src/
│   ├── download_dataset.py
│   ├── preprocess.py
│   ├── model.py
│   ├── train.py
│   └── generate.py
│
├── requirements.txt
└── README.md
```

---

## Technologies Used

* Python 3.x
* PyTorch
* NumPy
* Requests
* tqdm

---

## Model Architecture

The Character-Level RNN consists of:

1. Embedding Layer
2. Recurrent Neural Network (RNN) Layer
3. Fully Connected Output Layer

Architecture:

```text
Input Characters
        ↓
Embedding Layer
        ↓
RNN Layer
        ↓
Fully Connected Layer
        ↓
Predicted Next Character
```

---

## Installation

### Create Virtual Environment

Windows:

```bash
python -m venv venv
venv\Scripts\activate
```

Linux/Mac:

```bash
python -m venv venv
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Running the Project

### Step 1: Download Dataset

```bash
python src/download_dataset.py
```

Output:

```text
data/dataset.json
```

### Step 2: Preprocess Dataset

```bash
python src/preprocess.py
```

Output:

```text
data/corpus.txt
```

### Step 3: Train the RNN

```bash
python src/train.py
```

Output:

```text
models/char_rnn.pth
```

### Step 4: Generate Text

```bash
python src/generate.py
```

---

## Sample Output

```text
Generated Text:

Then a report likely by Mr.
Secretary stated that the committee
would continue discussions regarding
the proposed policy changes.
```

Note: Since a simple RNN is used, the generated text may contain spelling or grammatical errors. This is expected behavior and demonstrates that the model is learning character-level patterns from the dataset.

---

## Hyperparameters

| Parameter        | Value |
| ---------------- | ----- |
| Hidden Size      | 256   |
| Number of Layers | 2     |
| Sequence Length  | 100   |
| Batch Size       | 64    |
| Learning Rate    | 0.003 |
| Epochs           | 20    |

---

## Results

The model successfully learns:

* Character sequences
* Common English words
* Sentence structure
* Punctuation usage
* Writing patterns from the IAM dataset

Generated text resembles the style of the training corpus while producing new and previously unseen sequences.

---

## Limitations

* Uses a simple RNN instead of LSTM/GRU.
* May generate grammatically incorrect text.
* Limited long-term memory due to the vanishing gradient problem.
* Uses only text transcriptions, not handwritten images.

---

## Future Improvements

* Train on the complete IAM dataset.
* Increase training epochs.
* Improve text sampling methods.
* Implement LSTM or GRU architectures.
* Extend the project to generate actual handwriting images.

---

## Conclusion

A Character-Level Recurrent Neural Network (RNN) was successfully implemented and trained on IAM handwritten text transcriptions. The model learned character patterns and generated new text sequences that resemble the style and structure of the training data, demonstrating the effectiveness of recurrent neural networks for sequence modeling and text generation tasks.

---

## Author

S J Nithika