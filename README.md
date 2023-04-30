# facial-recognition
A Simple Python code to train a facial recognition model to identify human.

## Requirements
- Python version 3
- A webcam (your laptop’s built-in webcam or an external one)

## How to run
## Step 1: Install dependencies
Tested on MacOS, for windows, change accordingly.

    $ python -m venv venv
    $ source venv/bin/activate
    (venv) $ pip install -r requirements.txt

## Step 2: Create a custom face recognition dataset
Create a new subfolder inside the `dataset` directory using your first name, example `Sourav`, to contain your photos.

    (venv) $ python capture_image.py Sourav

When you're done, **ESC** to close the window. Repeat this step to add more friends, creating a separate folder for each person.

## Step 3: Train the model

    (venv) $ python encode_faces.py

Run this command to analyze the photos and output a new file `encodings.pickle` that contains criteria for identifying these faces.

## Step 4: Test the model

    (venv) $ python facial_req.py

Run this command to open a new webcam window. If your face is highlighted with a yellow box alongside your name, the model has been properly trained. Hit **q** to quit the program.

