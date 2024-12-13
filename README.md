# 50.035 Computer-Vision

## File Structure

This repository contains the following file structure:

📂 data
│ ├── 📂 alignments
│ │ └── 📂 s1
│ └── 📂 s1
📂 models
📄 LipNet_2d.ipynb
📄 LipNet_3d_bilstm.ipynb
📄 LipNet_3d_gru.ipynb
📄 Lip Reading AI.pdf

📂 data/alignments/s1 contains the ground truth labels for each .mpg file.

📂 models contains the saved weights for each model respectively

📄 LipNet_2d.ipynb, 📄 LipNet_3d_bilstm.ipynb, 📄 LipNet_3d_gru.ipynb are the respective models outlined in the 📄 Lip Reading AI.pdf which is the final report.

## Code Instructions

Within each .ipynb is the code required to train and evaluate the model. If you would like to use the saved weights instead of training the model, please execute all cells except for the following cell:

> model.fit(train, validation_data=test, epochs=100, callbacks=[checkpoint_callback, schedule_callback, example_callback])
model.save('models/3dcheckpoint.weights.h5')

