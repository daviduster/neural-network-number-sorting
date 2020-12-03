# Task

Encoder-decoder architecture (RNN/LSTM/Transformer-based) for number sorting.

## Comments
This is an interesting problem, more as an intellectual challenge than as a really practical solution (the existing algorithms for sorting, Quicksort and so on, are surely going to be faster and do not need the previous training time). I can think of (as the statement suggests) architectures for series. The good thing about a problem of this type is that it has not
data limit (you can use as many as you want). At first, I looked for some references like this [Paper](https://arxiv.org/pdf/1812.03928.pdf) (4.1 Sorting numbers) and this [discussion] (https://ai.stackexchange.com/questions/1508/which-neural-network-has-capabilities-of-sorting-input) but I think it is too complex, and a simple model is enough, using one RNN (or LSTM) as encoder, and then two or three dense layers, there should be no major problem for learn. You can find the implementation of the encoder-decoder arquitecture for sorting numbers in the jupyter notebook attached, as a reference for the implementation [Keras](https://blog.keras.io/a-ten-minute-introduction-to-sequence-to-sequence-learning-in-keras.html). Also frameworks like TensorFlow and Keras take care of the backpropagation step automatically and you can safely assume that it is implemented correctly so there is no need to use gradient checking.


## Installation of requirements

```python
# Installing virtualenv
pip3 install --user virtualenv

# Creating a virtual environment
python3 -m virtualenv env

# Activating a virtual environment
source env/bin/activate

# After activate the virtual environment you can install the necessary dependencies in your virtual env and use the notebook!
pip3 install -r requirements.txt

# Once you are finish 
deactivate

```

## License
[MIT](https://choosealicense.com/licenses/mit/)