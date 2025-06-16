# VocalUnravel
- A college project that implements the already implemented Wave-U-Net architecture for audio source separation and provides a simple UI to test the model.
- Gradio is used to provide a clean demo interface to test the model.


# Installation
- Python 3.6
- [libsndfile](http://mega-nerd.com/libsndfile/)
- [ffmpeg](https://www.ffmpeg.org/)
- CUDA

# Datasets
- [MUSDBHQ](https://sigsep.github.io/datasets/musdb.html)
- [DSD100](https://sigsep.github.io/datasets/dsd100.html)

# Setups
- Install Anaconda
- Create new virtual environment
- Install the requirements
  - `pip3 install -r requirements.txt`

# Training
Execute this command
  - `python train.py --dataset_dir /PATH/TO/MUSDB18HQ `
where the path to MUSDB18HQ dataset needs to be specified, which contains the train and test subfolders.


# Prediction
`python3.6 predict.py --load_model modelDirectory --input "audioDirectory"`

# Model Demo UI
- To run locally
  - Execute the app.ipnyb file. Before that make sure to
      - Put your trained model in the checkpoints/waveunet directory
- To run in colab
  - Upload the files in your google drive
  - Mount your drive in colab
  - Follow the steps in app.ipnyb
- Click the provided link to open the demo
      


