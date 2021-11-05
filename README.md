# FOTS

datasets

https://www.robots.ox.ac.uk/~vgg/data/scenetext/

https://rrc.cvc.uab.es/?ch=4&com=tasks

Use inference or fots_demo to use (Weights are not available).

Data generator to generate data and pipelines are used to give output image for an input with text detection and recognition.

Text detection and recognition (also known as Text Spotting) from an image is a very useful and challenging problem that deep learning researchers have been working on since many years because of its practical applications in fields like document scanning, robot navigation and image retrieval, etc. Almost all the methods consisted of two separate stages so far: 1) Text detection 2) Text recognition. Text detection just finds out where the text is located in the given image and on these results, text recognition actually recognizes the characters from the text. Because of these two stages, two separate models were required to be trained and hence prediction time was a bit higher. Because of higher test time, the models were not suitable for real time applications. Contrary to this, FOTS solves this two stage problem using a unified end to end trainable model/network by detecting and recognizing text simultaneously. It uses shared convolutional features between text detection and recognition tasks which learns more generic features and improves the test time such that it can be useful in real time applications such as OCR from video streams at higher FPS. FOTS also improves text detection on scenes having aligned/rotated texts because of its special component named “RoIRotate” (Region of Interest Rotate), which rotates the aligned text by keeping aspect ratio the same and then applies text recognition.
