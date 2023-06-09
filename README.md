# DeepLearning.AI TensorFlow Developer

## C1 - Introduction to TensorFlow for Artificial Intelligence, Machine Learning, and Deep Learning

## Week 1

### Assignment

- Housing Prices _(C1W1_Assignment.ipynb)_

### Ungraded Labs

1. Hello World Neural Network _(C1_W1_Lab_1_hello_world_nn.ipynb)_

## Week 2

### Assignment

- Handwriting Recognition _(C1W2_Assignment.ipynb)_

### Ungraded Labs

1. Beyond Hello World, A Computer Vision Example _(C1_W2_Lab_1_beyond_hello_world.ipynb)_
2. Callbacks _(C1_W2_Lab_2_callbacks.ipynb)_

## Week 3

### Assignment

- Improve MNIST with Convolutions _(C1W3_Assignment.ipynb)_

### Ungraded Labs

1. Improving Accuracy with Convolutions _(C1_W3_Lab_1_improving_accuracy_using_convolutions.ipynb)_
2. Exploring Convolutions _(C1_W3_Lab_2_exploring_convolutions.ipynb)_

## Week 4

### Assignment

- Handling Complex Images _(C1W4_Assignment.ipynb)_

### Ungraded Labs

1. Image Generator _(C1_W4_Lab_1_image_generator_no_validation.ipynb)_
2. Image Generator with Validation _(C1_W4_Lab_2_image_generator_with_validation.ipynb)_
3. Compacted Images _(C1_W4_Lab_3_compacted_images.ipynb)_


***  


## C2 - Convolutional Neural Networks in TensorFlow

## Week 1

### Assignment

- Cats vs. Dogs _(C2W1_Assignment.ipynb)_

### Ungraded Labs

1. Using more sophisticated images with Convolutional Neural Networks _(C2_W1_Lab_1_cats_vs_dogs.ipynb)_

## Week 2

### Assignment

- Cats vs. Dogs using Augmentation _(C2W2_Assignment.ipynb)_

### Ungraded Labs

1. Cats vs. Dogs with Augmentation _(C2_W2_Lab_1_cats_v_dogs_augmentation.ipynb)_
2. Horses vs. Humans with Augmentation _(C2_W2_Lab_2_horses_v_humans_augmentation.ipynb)_

## Week 3 

### Assignment

- Horses vs. Humans using Transfer Learning _(C2W3_Assignment.ipynb)_

### Ungraded Labs

1. Exploring Transfer Learning _(C2_W3_Lab_1_transfer_learning.ipynb)_

## Week 4

### Assignment

- Multi-class Classifier _(C2W4_Assignment.ipynb)_

### Ungraded Labs

1. Classifying Rock, Paper, and Scissors _(C2_W4_Lab_1_multi_class_classifier.ipynb)_


*** 



## C3 - Natural Language Processing in TensorFlow

## Week 1

### Assignment 

- Explore the BBC News Archive _(C3W1_Assignment.ipynb)_

### Ungraded Labs

1. Simple Tokenizing _(C3_W1_Lab_1_tokenize_basic.ipynb)_
2. Simple Sequences _(C3_W1_Lab_2_sequences_basic.ipynb)_
3. Sarcasm _(C3_W1_Lab_3_sarcasm.ipynb)_

***
### Resume :
* Lab 1 - Explain about tokenizing. its about text to number so the machine can process it (?)
* Lab 2 - 
  - Explain from tokenizing text to sequences, soo from word_index each of word get the key and make it into sequences from the text (?)  
  - Pad the sequences into a uniform length because that is what your model expects
  - Explain about OOV, it's about the word is not in the list from var word_index so the key will get OOV (Out of Vocabulary)
* Lab 3 - Tokenizing Real world Data from sarcasm dataset using json.
* Assignment :
  - Implementation Tokenizing with remove_stopword.
  - Can Filter the word and output the exclude all of the stopwords.

## Week 2

### Assignment 

- Categorizing the BBC News Archive _(C3W2_Assignment.ipynb)_

### Ungraded Labs

1. Positive or Negative IMDB Reviews _(C3_W2_Lab_1_imdb.ipynb)_
2. Sarcasm Classifier _(C3_W2_Lab_2_sarcasm_classifier.ipynb)_
3. IMDB Review Subwords _(C3_W2_Lab_3_imdb_subwords.ipynb)_

***

### Resume :
* Lab 1 - Training Binary with IMDB datasets - Word Embedding Compile the model using Embedding layers
* Lab 2 - Training Binary with sarcasm datasets - build a binary classifier.
  - tokenizing datasets from scratch and you're treating the vocab size as a hyperparameter. 
  - Furthermore, you're tokenizing the texts by building a vocabulary of full words.
* Lab 3 - Subword tokenization -
  - subword text encoding can be a robust technique to avoid out-of-vocabulary tokens
* Assignment :
  - Struggle on Validation Split
  - implemented a neural network capable of classifying text and also learned about embeddings and tokenization
## Week 3

### Assignment 

- Exploring Overfitting in NLP _(C3W3_Assignment.ipynb)_

### Ungraded Labs

1. IMDB Subwords 8K with Single Layer LSTM _(C3_W3_Lab_1_single_layer_LSTM.ipynb)_
2. IMDB Subwords 8K with Multi Layer LSTM _(C3_W3_Lab_2_multiple_layer_LSTM.ipynb)_
3. IMDB Subwords 8K with 1D Convolutional Layer _(C3_W3_Lab_3_Conv1D.ipynb)_
4. IMDB Reviews with GRU (and optional LSTM and Conv1D) _(C3_W3_Lab_4_imdb_reviews_with_GRU_LSTM_Conv1D.ipynb)_
5. Sarcasm with Bidirectional LSTM _(C3_W3_Lab_5_sarcasm_with_bi_LSTM.ipynb)_
6. Sarcasm with 1D Convolutional Layer _(C3_W3_Lab_6_sarcasm_with_1D_convolutional.ipynb)_

### Resume :
Model / Architecture can use for text classification :  
Embedding - LSTM - GRU / RNN - Convolutional Network  

* Lab 1 - IMDB Subwords 8K with with Single Layer LSTM 
  -  Change Flatten or GlobalConvolutional1D to LSTM layer / Bidirectional Function.
  
* Lab 2  - IMDB Subwords 8K with with Multiple Layer LSTM
  - Additional LSTM Layer will make lengthen the training compared with previous lab.
  
* Lab 3 - IMDB Subwords 8K with 1D convolutional Layer.
  - Build the model by simply appending the conv & pooling layer after embedding layer.
* Lab 4 - Building Models for the IMDB Datasets
  - Build with Flatten() -> Very fast to train.
  - Build with LSTM -> slower to train but useful in applications where the order of the tokens is important
  - Build with GRU -> a simpler version of the LSTM. It can be used in applications where the sequence is important but you want faster results and can sacrifice some accuracy
  - Build with Conv1D -> extract features from your dataset
  - Each layers have a diff function 
  - GlobalMaxPooling1D - layer to reduce the results before passing it on to the dense layers
* Lab 5 - Training a Sarcasm Detection Model using Bidirectional LSTMs
  
* Lab 6 - Training a Sarcasm Detection Model using a Convolution Layer
## Week 4

### Assignment

- Writing Shakespeare with LSTMs _(C3W4_Assignment.ipynb)_

### Ungraded Labs

1. NLP with Irish Music _(C3_W4_Lab_1.ipynb)_
2. Generating Poetry from Irish Lyrics _(C3_W4_Lab_2_irish_lyrics.ipynb)_


*** 


## C4 - Sequences, Time Series and Prediction

## Week 1

### Assignment

- Create and Predict Synthetic Data _(C4W1_Assignment.ipynb)_

### Ungraded Labs

1. Time Series _(C4_W1_Lab_1_time_series.ipynb)_
2. Forecasting _(C4_W1_Lab_2_forecasting.ipynb)_

## Week 2

### Assignment  

- Predict with a DNN _(C4W2_Assignment.ipynb)_

### Ungraded Labs

1. Preparing Features and Labels _(C4_W2_Lab_1_features_and_labels.ipynb)_
2. Single Layer Neural Network _(C4_W2_Lab_2_single_layer_NN.ipynb)_
3. Deep Neural Network _(C4_W2_Lab_3_deep_NN.ipynb)_

## Week 3

### Assignment

- Using RNN's and LSTM's for time series _(C4W3_Assignment.ipynb)_

### Ungraded Labs

1. Recurrent Neural Network (RNN) _(C4_W3_Lab_1_RNN.ipynb)_
2. Long Short-Term Memory (LSTM) _(C4_W3_Lab_2_LSTM.ipynb)_

## Week 4

### Assignment

- Daily Minimum Temperatures in Melbourne - Real Life Data _(C4W4_Assignment.ipynb)_

### Ungraded Labs

1. Long Short-Term Memory (LSTM) _(C4_W4_Lab_1_LSTM.ipynb)_
2. Sunspots _(C4_W4_Lab_2_Sunspots.ipynb)_
3. Sunspots - DNN Only _(C4_W4_Lab_3_DNN_only.ipynb)_
