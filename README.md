# Foul Language Detection

```markdown
# Audio Profanity Censor

This repository provides a solution to detect and censor profanity in audio files. It includes the use of both CNN and RNN models.

## Dependencies
- `pydub`
- `resampy`
- `librosa`
- `tensorflow`
- `numpy`
- `pandas`
- `tqdm`
- `keras`
- `scipy`

To install the necessary libraries, use the provided commands:

```bash
pip install pydub resampy librosa tensorflow numpy pandas tqdm keras scipy
```

## Usage

### Data Setup

1. Clone the TAPAD dataset
```bash
git clone https://github.com/profanitas/TAPAD.git
```

2. Update the path of your audio files accordingly in the code.

### Running the Models

The provided code includes the implementation of both a CNN and an RNN model. Follow the steps in the code to preprocess the data, build the model, and train it.

### Censoring Profanity

The `censor_audio` function can be used to detect and replace the profanity in audio files with a beep sound.

Example usage:

```python
censored_audio = censor_audio("path_to_audio_file.wav", model)
```

Replace `path_to_audio_file.wav` with the path to your audio file and `model` with the trained model (either CNN or RNN).

## Features

1. Audio file preprocessing: Converts audio files to suitable formats and extracts relevant features.
2. CNN and RNN models: Two types of models to detect profanity in audio files.
3. Audio censoring: A function to replace detected profanity with a beep sound.

## Known Limitations

Ensure that the audio files are either in `.mp3` or `.wav` format, as the current preprocessing functions support only these formats.

## Contribution

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License

[MIT](https://choosealicense.com/licenses/mit/)
```

This README provides an overview of the repository, how to set it up, and how to use it. You can customize it further according to your specific requirements.
