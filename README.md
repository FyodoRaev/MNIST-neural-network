# MNIST-neural-network
My first neural network.This is a neural network which predicts integer that stays in photo , but when I was making it I have not used any libraries except NumPy and Pandas.So I can call it Mnist-Neural-Network from scratch. I created it cause i read a book , got a lot of theory and was not able to implement the easiest examples. So any hard for understanding line of code I followed with comments. 

Edit: I returned to this repo after almost 6 months. I was a pretty cocky guy... I just copied the model from [this](https://youtu.be/w8yWXqWQYmU) youtube video. Now I wanted to rewrite this NN in terms of PyTorch and see how less it will be. 



* In our network we will have 2 layers ( the zeroth one is just a input layer)
* In our first layer we will use linear regression methods ->
   we will just use vector-matrix multiplication with input layer.
   Then we will do some very interesting stuff ,
   we will use activation function - ReLu(x),
   cause if we won't do that the first layer will be useless
   (cause we just multiple input matirce on weights vector twice and this thing called linear regression)
 * Finally , in output layer we will use activation function - softmax(x)
 * That was forward propagation now let's look at backward one. Delta for layer_2 is very obvious , it's just difference between right answer(which is 1) and network's      prediction. Delta for softmax function is differnce between right answer and prediction divided by lenght of right answer. But we used ReLu function on layer_1 so we    will not touch neurons which have 0. And the last one is delta for layer_0 which is basically quotient of 1 and predictions in layer_1 .

<hr> 

The best explanation about activation functions that I ever seen were in book "Grokking deep learning"
 so if you want to dive into it just check this book

