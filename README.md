# Auto-encoder
An autoencoder consists of 3 components: encoder, code and decoder. The encoder compresses the input and produces the code, the decoder then reconstructs the input only using this code.

To build an autoencoder we need 3 things: an encoding method, decoding method, and a loss function to compare the output with the target. 
In this example, we will implement an autoencoder for the following architecture, 1 hidden layer in the encoder and decoder.
We will use MNIST dataset as input. It contains black-and-white images of handwritten digits. And then we will now implement the autoencoder with Keras.
Secondly, we will force the autoencoder to learn useful features, which is adding random noise to its inputs and making it recover the original noise-free data. This is called a denoising autoencoder.
We presented two approaches to guide the autoencoder in acquiring meaningful features: enforcing a compact code size and employing denoising autoencoders. Another technique involves incorporating regularization. By imposing a sparsity constraint, we can regulate the autoencoder to ensure that only a portion of its nodes exhibit non-zero values, referred to as active nodes.
Then, we are goig to visualizet the labels on the plots help differentiate between the distributions of the two models. This type of visualization can provide insights into how regularization affects the distribution of encoded representations in comparison to a standard autoencoder model.
