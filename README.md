# Keras
ML using Keras

Keras is high-level library for buiding neural network in python with only a few lines of code.

In1----->()----()----
In2----->()----()----> OUT
    ---  ()----()---- 

# creating a simple sequential model:
model = keras.models.Sequential();
# add a layer with 3 nodes. input_dim => there are two input nodes.
model.add(Dense(3, input_dim=2))
# add another layer with 3 nodes.
model.add(Dense(3))
# add output layer with one node
//-------------- enhancement -------------
# # customizing neural network in Keras
model = keras.models.Sequential();
# add a layer with 3 nodes. input_dim => there are two input nodes.
model.add(Dense(3, input_dim=2, activation='relu'))
# add another layer with 3 nodes.
model.add(Dense(3, activation='relu'))
//----------------------------------------

## Final step
# optimizer algorithm that is used to train the neural network --> here it is 'adam'
# loss function --> here it is 'mse'
model.compile(optimizer='adam', loss='mse')



