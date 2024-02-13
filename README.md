# Finger-Detection-Deep-Learning
The aim of this project is to build a Convolutional Neural Network to simultaneously localize and classify the number of fingers I'm showing the camera.

The images were obtained using my laptop camera and annotations of the classes and bounding box coordinates was performed using "labelME". To increase the number of images for training and also to introduce some variability to the neural network, I also performed image augmentation with "albumentations".

A CNN was built using transfer learning with VGG16 to perform two types of tasks using the keras Functional API (regression and classification). The regression task found the coordinates to draw the bounding box arround my hand and the classification task classified the number of fingers I was showing the camera in real time. A custom training loop was built to be able to perform both of the tasks while computing the corresponding loss in each epoch for each of the tasks.

The full code is available in the repository in the form of a jupyter notebook and below are some images of the final results :)

<img src="https://github.com/brss12/Finger-Detection-Deep-Learning/assets/121204829/ee9f0738-070f-4746-97d5-0bac8301e4b0" width="300"> | <img src="https://github.com/brss12/Finger-Detection-Deep-Learning/assets/121204829/1e1c482a-1b61-404b-8a5e-bfce28115b0c" width="300"> | <img src="https://github.com/brss12/Finger-Detection-Deep-Learning/assets/121204829/82a7a63c-1627-46e1-8b45-2335d09fe94c" width="300">
<img src="https://github.com/brss12/Finger-Detection-Deep-Learning/assets/121204829/a7d9547b-7eda-4f58-9363-13754ef6458a" width="300"> | <img src="https://github.com/brss12/Finger-Detection-Deep-Learning/assets/121204829/3856db7b-bb92-479d-b4f1-44cf28c6b901" width="300"> | <img src="https://github.com/brss12/Finger-Detection-Deep-Learning/assets/121204829/7a2dedec-8aab-4f25-960b-b7d821077f31" width="300">
