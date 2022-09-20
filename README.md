setup

```bash
python3 -m venv python-aubio-librosa
. python-aubio-librosa/bin/activate
pip3 install -r requirements.txt
```

osx 
```bash

brew install portaudio
pip3 install --global-option='build_ext' --global-option='-I/opt/homebrew/Cellar/portaudio/19.7.0/include' --global-option='-L/opt/homebrew/Cellar/portaudio/19.7.0/lib' pyaudio
```

m1 specific problems
```bash
mkdir  python-aubio-librosa/lib/python3.9/site-packages/_soundfile_data
cp /opt/homebrew/Cellar/libsndfile/1.1.0_1/lib/libsndfile.1.dylib python-aubio-librosa/lib/python3.9/site-packages/_soundfile_data/
cp /opt/homebrew/Cellar/libsndfile/1.1.0_1/lib/libsndfile.dylib python-aubio-librosa/lib/python3.9/site-packages/_soundfile_data/
```

