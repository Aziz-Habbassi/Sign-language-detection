# Sign-language-detection

> **Sign language recognition** using Python, OpenCV, MediaPipe, and
> Scikit-Learn.\
> Includes scripts for collecting images, creating a dataset, training
> the model, and testing predictions.

## Prerequisites

-   Python 3.10 (recommended and tested)
-   A webcam
-   Dependencies listed in `requirements.txt`

## Installation

``` bash
git clone https://github.com/Aziz-Habbassi/Sign-language-detection.git
cd Sign-language-detection

python3.10 -m venv venv

# Windows
venv\Scripts\activate
# macOS / Linux
source venv/bin/activate

pip install --upgrade pip
pip install -r requirements.txt
```

## Usage

### 1) Collect images --- `collect_imgs.py`

Captures webcam images and creates a folder for each sign.

``` bash
python collect_imgs.py
```

### 2) Create dataset --- `create_dataset.py`

Extracts hand landmarks using MediaPipe and builds the dataset.

``` bash
python create_dataset.py
```

### 3) Train the model --- `train_classifier.py`

Trains a Scikit-Learn classifier.

``` bash
python train_classifier.py
```

### 4) Test the model --- `test_classifier.py`

Runs real-time predictions using the webcam.

``` bash
python test_classifier.py
```

## Tips

-   Use good lighting when collecting images
-   Capture several angles and distances
-   Keep background simple for better detection

## Contact

Feel free to open issues or contribute to the project!
