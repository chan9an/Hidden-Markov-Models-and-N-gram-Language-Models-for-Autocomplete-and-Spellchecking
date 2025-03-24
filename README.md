# Hidden-Markov-Models-and-N-gram-Language-Models-for-Autocomplete-and-Spellchecking

## Overview
This project explores the use of **Hidden Markov Models (HMMs) and N-gram Language Models** to enhance text input accuracy through **autocomplete and spellchecking** functionalities. By leveraging probabilistic modeling, it predicts the most likely next word and corrects spelling mistakes effectively.

## Features
- **N-gram Language Model:** Uses bigrams and trigrams to predict the next word based on context.
- **Hidden Markov Model (HMM):** Analyzes spelling errors and determines the most probable intended word.
- **Autocomplete:** Suggests relevant words based on prior input.
- **Spellchecking:** Identifies and corrects spelling mistakes while considering word likelihood.
- **Probability Estimations:** Implements smoothing techniques to handle unseen words and improve predictions.

## Implementation Details
- **Data Processing:** Tokenization, case normalization, and handling of unknown words.
- **N-gram Model:** Constructs frequency-based word sequences with smoothing methods like Laplace or Kneser-Ney.
- **HMM for Spell Correction:** Models spelling errors probabilistically and applies transition/emission probabilities.
- **Viterbi Algorithm:** Finds the most likely word sequence for spellchecking.

## Dependencies
Install the required libraries using:
```bash
pip install nltk numpy pandas
```

## Usage
### Training the Models
1. Prepare a text corpus and tokenize it.
2. Train the N-gram model to compute word probabilities.
3. Train the HMM model using known spelling error datasets.

### Running Autocomplete
```python
from autocomplete import predict_next_word
print(predict_next_word("I am going to the"))
```

### Running Spellchecker
```python
from spellchecker import correct_word
print(correct_word("hte"))  # Expected output: "the"
```

## Dataset
- Publicly available corpora like:
  - **Brown Corpus (NLTK)**
  - **Wikipedia Dump**
  - **Common Crawl**

## Future Enhancements
- Improve prediction accuracy using deep learning models (e.g., Transformers or LSTMs).
- Expand to support multiple languages.
- Integrate real-time text correction into applications.

## Contributors
- **Your Name**
- Contributions are welcome! Feel free to submit issues or pull requests.

## License
This project is released under the MIT License.

