# neural abstractions

In the image domain of the abstract interpretation problem, we want to be able to learn the correct
sequence that will transform an input image to its corresponding output image and from that infer which image
transformations can be generated by training an encoded image through different blocks that correspond to
different transformations. We expect that an image produced from a given sequence of transformations also has
a high probability of being found in the set of images generated from the encoder-decoder network where each
block is a neural network trained for a specific image transformation on a set of images.

The general idea is to generate a random program sequence and try to infer the random program sequence using any
form of encoder-decoder neural network architecture.

To display image transformations,
run texture_transformations.py for grayscale and texture_transformationsRGB.py for color

To generate textures, 
run gen_sequence.py

To train models, 
run train.py.

To predict program sequences that create textures,
run predict_prog.py
