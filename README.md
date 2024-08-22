# ASL Detector
This project uses computer vision and mediapipe's customizable gesture recognition to detect American Sign Language in a live video feed. 

To use the detecor, run the main file **ASL_detector.py**. The file will use open your webcam and use the pretrained **asl.task** to detect any sign language in the feed. Detected letters will appear on the webcam window. Once a letter is detected, the user can press the enter key on their keyboard to write this letter (or a space) to a text file. Once the program is ended, a txt file with the messaged will be saved in the users directory.

**Note:** The program follows conventional ASL gestures with the exception of "J" and "Z" as they involve the tracking of a moving gesture which was outside the scope of this project. To resolve this issue, custom gestures were made for this letters which can be viewed in the dataset.

Included in this repo:
- **ASL folder** - Custom dataset of close to 3,000 ASL gestures used to train the model.
- **ASL_Detector.py** - main file
- **asl.task** - Trained Mediapipe task for use in the main file.
- **ASL_Detection_example** - Example video of program.
- **train_task.py** - Mediapipe's method of training a model from images.