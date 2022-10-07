# Part 1
## a) output:
```
Epoch 1/20
469/469 [==============================] - 7s 13ms/step - loss: 0.2444 - accuracy: 0.9250 - val_loss: 0.1244 - val_accuracy: 0.9612
Epoch 2/20
469/469 [==============================] - 6s 14ms/step - loss: 0.1017 - accuracy: 0.9691 - val_loss: 0.0888 - val_accuracy: 0.9751
Epoch 3/20
469/469 [==============================] - 7s 14ms/step - loss: 0.0738 - accuracy: 0.9778 - val_loss: 0.0690 - val_accuracy: 0.9810
Epoch 4/20
469/469 [==============================] - 6s 13ms/step - loss: 0.0588 - accuracy: 0.9821 - val_loss: 0.0808 - val_accuracy: 0.9775
Epoch 5/20
469/469 [==============================] - 6s 14ms/step - loss: 0.0515 - accuracy: 0.9846 - val_loss: 0.0744 - val_accuracy: 0.9803
Epoch 6/20
469/469 [==============================] - 7s 15ms/step - loss: 0.0425 - accuracy: 0.9871 - val_loss: 0.0791 - val_accuracy: 0.9812
Epoch 7/20
469/469 [==============================] - 7s 15ms/step - loss: 0.0371 - accuracy: 0.9889 - val_loss: 0.0785 - val_accuracy: 0.9810
Epoch 8/20
469/469 [==============================] - 6s 14ms/step - loss: 0.0331 - accuracy: 0.9904 - val_loss: 0.0833 - val_accuracy: 0.9821
Epoch 9/20
469/469 [==============================] - 9s 19ms/step - loss: 0.0313 - accuracy: 0.9907 - val_loss: 0.1032 - val_accuracy: 0.9794
Epoch 10/20
469/469 [==============================] - 6s 14ms/step - loss: 0.0283 - accuracy: 0.9918 - val_loss: 0.0965 - val_accuracy: 0.9808
Epoch 11/20
469/469 [==============================] - 6s 13ms/step - loss: 0.0250 - accuracy: 0.9927 - val_loss: 0.0920 - val_accuracy: 0.9823
Epoch 12/20
469/469 [==============================] - 7s 16ms/step - loss: 0.0251 - accuracy: 0.9925 - val_loss: 0.0852 - val_accuracy: 0.9837
Epoch 13/20
469/469 [==============================] - 7s 14ms/step - loss: 0.0232 - accuracy: 0.9933 - val_loss: 0.1020 - val_accuracy: 0.9845
Epoch 14/20
469/469 [==============================] - 6s 13ms/step - loss: 0.0232 - accuracy: 0.9934 - val_loss: 0.0936 - val_accuracy: 0.9841
Epoch 15/20
469/469 [==============================] - 6s 14ms/step - loss: 0.0217 - accuracy: 0.9934 - val_loss: 0.1147 - val_accuracy: 0.9826
Epoch 16/20
469/469 [==============================] - 7s 14ms/step - loss: 0.0206 - accuracy: 0.9943 - val_loss: 0.0987 - val_accuracy: 0.9832
Epoch 17/20
469/469 [==============================] - 8s 16ms/step - loss: 0.0182 - accuracy: 0.9949 - val_loss: 0.1205 - val_accuracy: 0.9815
Epoch 18/20
469/469 [==============================] - 8s 16ms/step - loss: 0.0206 - accuracy: 0.9945 - val_loss: 0.1147 - val_accuracy: 0.9833
Epoch 19/20
469/469 [==============================] - 7s 14ms/step - loss: 0.0177 - accuracy: 0.9950 - val_loss: 0.1271 - val_accuracy: 0.9819
Epoch 20/20
469/469 [==============================] - 6s 13ms/step - loss: 0.0167 - accuracy: 0.9954 - val_loss: 0.1409 - val_accuracy: 0.9807
Test loss: 0.14094342291355133
Test accuracy: 0.9807000160217285

Process finished with exit code 0
```

## b) Leave it with only one hidden layer, remove the dropouts and run it again.
### b.1) activation='softmax'
```
Model: "sequential"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 dense (Dense)               (None, 512)               401920    
                                                                 
 dense_1 (Dense)             (None, 10)                5130      
                                                                 
=================================================================
Total params: 407,050
Trainable params: 407,050
Non-trainable params: 0
_________________________________________________________________
Epoch 1/20
469/469 [==============================] - 4s 7ms/step - loss: 0.2518 - accuracy: 0.9276 - val_loss: 0.1313 - val_accuracy: 0.9584
Epoch 2/20
469/469 [==============================] - 3s 7ms/step - loss: 0.1029 - accuracy: 0.9697 - val_loss: 0.0970 - val_accuracy: 0.9711
Epoch 3/20
469/469 [==============================] - 3s 7ms/step - loss: 0.0688 - accuracy: 0.9790 - val_loss: 0.0720 - val_accuracy: 0.9789
Epoch 4/20
469/469 [==============================] - 3s 7ms/step - loss: 0.0495 - accuracy: 0.9852 - val_loss: 0.0675 - val_accuracy: 0.9787
Epoch 5/20
469/469 [==============================] - 3s 7ms/step - loss: 0.0380 - accuracy: 0.9888 - val_loss: 0.0683 - val_accuracy: 0.9799
Epoch 6/20
469/469 [==============================] - 3s 7ms/step - loss: 0.0290 - accuracy: 0.9914 - val_loss: 0.0693 - val_accuracy: 0.9815
Epoch 7/20
469/469 [==============================] - 3s 7ms/step - loss: 0.0223 - accuracy: 0.9935 - val_loss: 0.0615 - val_accuracy: 0.9823
Epoch 8/20
469/469 [==============================] - 3s 7ms/step - loss: 0.0173 - accuracy: 0.9949 - val_loss: 0.0726 - val_accuracy: 0.9808
Epoch 9/20
469/469 [==============================] - 3s 7ms/step - loss: 0.0129 - accuracy: 0.9962 - val_loss: 0.0686 - val_accuracy: 0.9805
Epoch 10/20
469/469 [==============================] - 3s 7ms/step - loss: 0.0103 - accuracy: 0.9970 - val_loss: 0.0722 - val_accuracy: 0.9811
Epoch 11/20
469/469 [==============================] - 3s 7ms/step - loss: 0.0079 - accuracy: 0.9979 - val_loss: 0.0716 - val_accuracy: 0.9816
Epoch 12/20
469/469 [==============================] - 3s 7ms/step - loss: 0.0063 - accuracy: 0.9984 - val_loss: 0.0735 - val_accuracy: 0.9820
Epoch 13/20
469/469 [==============================] - 3s 7ms/step - loss: 0.0048 - accuracy: 0.9988 - val_loss: 0.0860 - val_accuracy: 0.9810
Epoch 14/20
469/469 [==============================] - 3s 7ms/step - loss: 0.0039 - accuracy: 0.9991 - val_loss: 0.0845 - val_accuracy: 0.9804
Epoch 15/20
469/469 [==============================] - 3s 7ms/step - loss: 0.0029 - accuracy: 0.9992 - val_loss: 0.0845 - val_accuracy: 0.9823
Epoch 16/20
469/469 [==============================] - 3s 7ms/step - loss: 0.0025 - accuracy: 0.9993 - val_loss: 0.0956 - val_accuracy: 0.9806
Epoch 17/20
469/469 [==============================] - 3s 7ms/step - loss: 0.0019 - accuracy: 0.9996 - val_loss: 0.0895 - val_accuracy: 0.9830
Epoch 18/20
469/469 [==============================] - 3s 7ms/step - loss: 0.0014 - accuracy: 0.9997 - val_loss: 0.0907 - val_accuracy: 0.9817
Epoch 19/20
469/469 [==============================] - 3s 7ms/step - loss: 0.0012 - accuracy: 0.9997 - val_loss: 0.0939 - val_accuracy: 0.9831
Epoch 20/20
469/469 [==============================] - 4s 8ms/step - loss: 9.2041e-04 - accuracy: 0.9997 - val_loss: 0.0929 - val_accuracy: 0.9828
Test loss: 0.09286054968833923
Test accuracy: 0.9828000068664551
```
### b.2) activation='softmax'
