
# SafeCue
SafeCue is an assistive technology project designed to improve environmental sound awareness for deaf and hard-of-hearing (DHH) individuals. The system detects safety-critical sounds, such as fire alarms, smoke alarms, sirens, and screaming, and communicates detected sounds through visual LED alerts. By combining machine learning with hardware integration, SafeCue aims to provide accessible, real-time sound awareness while minimizing privacy risks associated with cloud-based audio processing.

# Machine Learning Model
SafeCue uses a custom-trained machine learning model to classify environmental sounds into predefined audio categories. The audio dataset is split into appropriate subsets for model development and evaluation, and the audio samples are converted into Mel spectrograms—time-frequency representations of sound that can be processed as image-like inputs by a classifier. The trained model predicts the sound category from these representations and is deployed locally on the Qualcomm Arduino UNO Q for on-device inference.

<img width="678" height="452" alt="mel" src="https://github.com/user-attachments/assets/026169a0-b028-4ab7-ace1-91b3c94d19ee" />

# Hardware Implementation
The system uses the Qualcomm Arduino UNO Q to run the trained model and connect software predictions to a physical LED circuit. When a sound is classified, the corresponding hardware output provides a visual cue to represent the detected category. This integration demonstrates how embedded computing and machine learning can work together to translate environmental audio into accessible visual feedback.
