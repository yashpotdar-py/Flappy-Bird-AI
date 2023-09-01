 ## Flappy Bird AI using NEAT

This is a recreation of the classic Flappy Bird game using the NEAT algorithm to train a neural network to play the game and PyGame.

### Prerequisites

* Python 3.6 or later
* Pygame
* NEAT-python
* Graphviz (optional, for visualizing the neural network)
* Matplotlib (optional, for plotting the fitness statistics)

### Installation

1. Install Python 3.6 or later.
2. Install Pygame: `pip install pygame`
3. Install NEAT-python: `pip install neat-python`
4. Install Graphviz (optional): `pip install graphviz`
5. Install Matplotlib (optional): `pip install matplotlib`

### Usage

1. Clone this repository.
2. Run the game: `python game.py`
3. The game will start running and the neural network will begin to train.
4. You can watch the progress of the training by observing the graphs that are generated.
5. The game will automatically save the best neural network to a file called `best.pickle`.
6. You can load the best neural network and watch it play the game by running `python game.py --load best.pickle`

### Code Explanation

The code is divided into three main files:

* `config-feedforward.txt`: This file contains the configuration for the NEAT algorithm.
* `game.py`: This file contains the code for the Flappy Bird game.
* `visualize.py`: This file contains the code for visualizing the neural network and the fitness statistics.

The `config-feedforward.txt` file contains the following parameters:

* `fitness_criterion`: The fitness criterion to use. In this case, we are using the "max" criterion, which means that the fitness of a genome is the maximum score that it achieves.
* `fitness_threshold`: The fitness threshold to use. In this case, we are using a threshold of 100, which means that the algorithm will stop training once a genome reaches a score of 100.
* `pop_size`: The size of the population to use. In this case, we are using a population size of 50.
* `reset_on_extinction`: Whether or not to reset the population if it goes extinct