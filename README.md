# CNN-Recolorization
Image re-colorization with CNN / Generative text model with LSTM

CNN recolorization will color the grayscale images of different birds. 

For the consideration of computational power and runtime efficiency, K-means algorithm is used here to first reduce the RGB color of 32*32*3 down to only k colors. Otherwise it will be too slow.

The validation loss after training is rought 0.45 and the result of recolorized images are shown at the bottom in comparsion with the input (grayscale images).
The following comparsions are the result.
![download](https://user-images.githubusercontent.com/25105806/109872512-61b5c700-7c21-11eb-9932-0689bee035b0.png)

The following comparsions are the reflection of increasing k to 32 in k-means algorithm
![k-means32](https://user-images.githubusercontent.com/25105806/109872519-64b0b780-7c21-11eb-830d-583a49125dee.png)
