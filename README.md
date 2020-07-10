# RANKIT

RANKIT is an interactive online system for personalized rank building and data visualization. Many publically available rankings do not expose the attributes used to compose the ranking, and do not allow for users to input their own preferences to manipulate the ranking. RanKit allows users to input their preferences about a few items in the dataset, and then automatically generate a ranking over all items that reflects this personalized input. Visual feedback provides information on the learned attribute weights and confidence of the ranking model.  

RANKIT is composed of two tools: Explore and Build. To learn more about each tool, read our [guide](https://github.com/RankerToolWebsite/myRanker/wiki).

## Tool: Build

The build page is an interactive interface where users input their preferences about items to be ranked. The Build tool collects data from pairwise comparisons of sample objects completed by the user. The tool applies a pairwise learning-to-rank model to the user input to create a global ranking over all items.

## Tool: Explore

Explore is an interactive tool that allows you to view the global ranking learned by the model and the underlying model weights and data attributes.

## Getting Started

### Prerequisites:

- [Python 3](https://www.python.org)

- [Pip](https://pypi.python.org/pypi/pip)

- [npm](https://www.npmjs.com/)
	- `$ sudo apt-get install npm`
- [Node.js](http://nodejs.org/)
	- `$ sudo apt-get install -y nodejs`
- [Flask](http://flask.pocoo.org/)
	- `$ pip install Flask`


### Run: 

#### To download dependiencies:

*in myRanker directory:*

`$ pip3 install -r requirements.txt`

*[optional] you may need to also set the path to numpy if you get a cython error:*

`$ export CFLAGS=-I$<location of Python>/lib/python<version>/site-packages/numpy/core/include`

Example: `export CFLAGS=-I/Library/Frameworks/Python.framework/Versions/3.5/lib/python3.5/site-packages/numpy/core/include/`

#### To startup the server:

*run project:* `$ python3 run.py`

## Datasets

Rankit includes a number of datasets by default. Sources:
- Video Games Dataset. https://www.kaggle.com/rush4ratio/video-game-sales-with-ratings
- States Dataset. http://matters.mhtc.org
- Movies Dataset. https://www.kaggle.com/rounakbanik/the-movies-dataset
- FIFA Dataset. https://www.kaggle.com/artimous/complete-fifa-2017-player-dataset-global
- Board Games Dataset. https://www.kaggle.com/mrpantherson/board-game-data




