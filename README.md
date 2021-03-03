# CNN-Recolorization-and-LSTM
Image re-colorization with CNN / Generative text model with LSTM

CNN recolorization will color the grayscale images of different birds. 

For the consideration of computational power and runtime efficiency, K-means algorithm is used here to first reduce the RGB color of 32*32*3 down to only k colors. Otherwise it will be too slow.

The validation loss after training is rought 0.45 and the result of recolorized images are shown at the bottom in comparsion with the input (grayscale images).
The following comparsions are the result.
![download](https://user-images.githubusercontent.com/25105806/109872512-61b5c700-7c21-11eb-9932-0689bee035b0.png)

The following comparsions are the reflection of increasing k to 32 in k-means algorithm
![k-means32](https://user-images.githubusercontent.com/25105806/109872519-64b0b780-7c21-11eb-830d-583a49125dee.png)




LSTM generative text model will mimic the writing style of poet Bertrand Russell.

Again, for the consideration of computational power and runtime efficiency, LSTM will learn character by character instead of word by word of the published articles.

The books used are MYSTICISM AND LOGIC AND OTHER ESSAYS (MLOE), THE ANALYSIS OF MIND (TAM), The Problems of Philosophy (TPP) and Our Knowledge of the External World as a Field for Scientific Method in Philosophy (OKEWFSMP)

LSTM at the end will be given a starting string of text and keep writing to the text character by character until it reaches the pre-defined length. It will use previous texts to predict/mimic the next most possible character.

The following are the generated text.
" there are those who take mental phenomena naively just as they would physical phenomena this school of psychologists tends not to emphasize the object which is the same as the shnple in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the state of affairs in the "
