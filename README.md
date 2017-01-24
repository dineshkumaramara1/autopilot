# Autopilot-TensorFlow
A TensorFlow implementation of this [Nvidia paper](https://arxiv.org/pdf/1604.07316.pdf) with some changes.

#How to Use
Download the [dataset](https://drive.google.com/file/d/0B-KJCaaF7ellQUkzdkpsQkloenM/view?usp=sharing) and extract into the repository folder

Use `python train.py` to train the model

Use `python run.py` to run the model on a live webcam feed

Use `python run_dataset.py` to run the model on the dataset

To visualize training using Tensorboard use `tensorboard --logdir=./logs`, then open http://0.0.0.0:6006/ into your web browser.




##Custom commands

Default training:
python train.py




Predicting on Udacity dataset:
python run_dataset.py -i train_center.csv --data /vol/data --delimiter ',' --units rad

Predicting on Autopilot dataset:
python run_dataset.py -i data.csv --data /vol/driving_dataset --delimiter ' ' --units deg

TODO: Confirm deg and rad on these 2 commands!!
