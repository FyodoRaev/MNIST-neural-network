# MNIST-neural-network
My first neural network. I created it cause i read a book , got a lot of theory and was not able to implement the easiest examples. So any hard for understanding line of code I followed with comments. 

Steps:
# ↓↓↓ why do we need to transpose matrices?(f.g. Aᵀ) ↓↓↓
'''
 1 Sometimes when we multiple VECTOR_STRING on MATRICE we want to receive VECTOR-STRING , 
   VECTOR_STRING x MATRICE = VECTOR_STRING

 2 But sometimes when we multiple MATRICE on VECTOR_COLUMN we want to get VECTOR_COLUMN
 In order to get same values (coordinates of result vector) in 2 case we must multiple transposed matrice on vector_column
'''

#3 In our network we will have 2 layers ( the zeroth one is just a input layer)

'''
 4 In our first layer we will use linear regression methods ->
   we will just use vector-matrix multiplication with input layer.
   Then we will do some very interesting stuff ,
   we will use activation function - ReLu(x),
   cause if we won't do that the first layer will be useless
   (cause we just multiple input matirce on weights vector twice and this thing called linear regression)
 5 Finally , in output layer we will use activation function - softmax(x)
 
 6 That was forward propagation now let's look at backward one. Delta for layer_2 is very obvious , it's just difference between right answer(which is 1) and network's      prediction. Delta for softmax function is differnce between right answer and prediction divided by lenght of right answer. But we used ReLu function on layer_1 so we    will not touch neurons which have 0.
   And the last one is delta for layer_0 which is basically quotient of 1 and predictions in layer_1 .
'''
 The best explanation about activation functions that I ever seen were in book "Grokking deep learning"
 so if you want to dive into it just check this book
'''
