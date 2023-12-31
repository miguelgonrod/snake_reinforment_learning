# snake_reinforment_learning

## Table of contents
* [Description](#description)
* [Demostration](#demostration)
* [Technologies](#technologies)
* [Conda](#conda)
* [Setup](#setup)
* [Licence](#licence)

## Description
Explore the realm of Reinforcement Learning with this Python repository, powered by PyTorch and Pygame. The project focuses on training an artificial intelligence to independently navigate and excel in the iconic Snake game. Leveraging PyTorch for neural network model creation and training, and Pygame for a visually engaging game interface, this repository provides a hands-on opportunity to delve into the nuances of reinforcement learning. Dive into the fascinating world of artificial intelligence, guiding an AI to mastery in the game of Snake through experimentation with hyperparameters, algorithms, and neural network architectures.

## Demostration

Still in development...


## Technologies
This project was created with:
* python: 3.10.12
* conda: 23.7.4
* pytorch: 2.1.2

## Conda
To run this project is recomended to create a conda venv, but if you wnat to run the project without conda you can skip this section.

To install conda you have to download your version in the oficial page: https://www.anaconda.com/download/
And now you have to execute the script
```
$ sudo apt install python3 python3-pip
$ cd ~/Downloads
$ chmod u+x Anaconda*.sh
$ sudo ./Anaconda*.sh
```
when asked to accept the licence terms, input yes
to install to all users when asked to select the location use '/opt/anaconda3' and when asked to enable input 'no'
Now you have to create a group for anaconda and make it available to the required user:
```
$ sudo groupadd anaconda
$ sudo chgrp -R anaconda /opt/anaconda3
$ sudo chmod 770 -R /opt/anaconda3
$ sudo usermod -aG anaconda [User]
```
And open a new terminal.

Finally you have to enable conda and create the environment for this project:
```
$ source /opt/anaconda3/bin/activate
$ conda init
$ conda create -n snake_env python=3.10.12
$ conda activate snake_env
```

If you are getting an error similar to this GLIBCXX_3.4.30 you have to instal gcc for conda:
```
$ conda install -c conda-forge gcc=12.1.0
```

With all this steps done you are ready to go.

## Setup
To run this project you need to clone this repository first
```
$ git clone https://github.com/miguelgonrod/snake_reinforment_learning.git
$ cd snake_reinforcement_learning
```

Now you have to use pip to install the requirements:
```
$ pip install -r requirements.txt
```

Also you need to install pytorch using the official page: https://pytorch.org/ or using my recomended option:
```
$ pip3 install torch torchvision --index-url https://download.pytorch.org/whl/cpu
```

Lastly you can run the program using:
```
$ python3 agent.py
```

If you are getting any other error not stated in this readme open an issue to further help.

## Licence
snake_reinforment_learning is available under the BSD-3-Clause license. See the LICENSE file for more details.
