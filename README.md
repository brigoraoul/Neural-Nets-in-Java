This is a basic implementation of an artificial neural network in Java (JDK 12). The main-class gives an example for the creation of a NeuralNet-object. All input data has to be a two-dimensional array in form of a Matrix-object from the custom Matrix class.
The class Function contains two subclasses for activation functions (sigmoid, hyperbolic tangent, rectifier linear unit and Softmax) and for loss functions (main squared error, binary cross entropy, categorical crossentropy).
Therefore, regression, binary classification and multiclass classification are supported.

The soundness of the implementation can be prooved by gradient checking. However, the implementation does not contain any optimizers or regularization techniques. As a consequence, vanishing / exploding gradients are a big problem even with a very shallow NeuralNet.
