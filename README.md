# MNIST Demo

An interactive demonstration of single digit classification using deep artificial neural networks.

A web application which demonstrates the ability of both fully connected and convolutional neural networks to classify handwritten digits.

## Demonstration

Where is it?
What does it show?

Show me a gif..


## Code

### Web

The front-end is a single page web application developed with the React.js and and Redux frameworks.

### Server

The server is a python flask server which use's Google's TensorFlow library to evaluation pre-trained neural networks for handwriting recogntion.

### Neural Networks

Both the fully connnected and convolutional neural networks have been trained using TensorFlow and following the tutorials MNIST for ML beginners and Deep MNIST for Experts.
The training data used are the 60,000 training images from the MNIST database of handwritten digits.

## Getting Started

### Requirements

* Python 2.7
* pip

### Install Dependencies

Install server dependencies:

(Linux)
```bash
pip install -r requirements.txt
``` 

(Mac)
```bash
pip install -r requirements-mac.txt
``` 

Install web dependencies:

```bash
npm install
```

### Run Application

To build and run the app locally run:

```bash
npm run build && npm run gunicorn
```

The app will be running at `localhost:8000`

### Webpack front-end development server

To run the app with the front-end development server run:

```bash
npm run gunicorn
npm run dev
```

The development server will be running at `localhost:8080` and proxying requests to `localhost:8000`

### Neural Networks

The pre-trained neural networks are saved in the models directory.

To re-train the networks run:

* `python networks/fully_connected.py`
* `python networks/convolutional.py`

The trained networks will be saved to the `/tmp` directory


## Deployment




