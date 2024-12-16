Semantic Parser: Seq2Seq Encoder-Decoder Semantic Parser with Attention

This project implemented a Seq2Seq Semantic Parser with Attention to take natural language inputs and form structured logical form outputs. This was all done based on the work of Dong and Lapata (2016).
The project leveraged an encoder-decoder architecture with the encoder and decoder made of lstm-layers with attention mechanisms.

Key Features:
- The model used encoder-decoder architecture with an attention mechanism
- LSTMs were used in both the Encoder and Decoder
- Dropout was implemented due to the small size of the dataset to combat overfitting
- Negative-Log-Likelihood Loss was used as the loss function

DataSet used:
- The dataset used was the Jobs dataset as the paper also used it and the accuracies could be compared. Like the paper, the model for this project only had 1 layer for the LSTMs to ensure authenticity.

Model Design:
- Encoder: The encoder started with an embedding layer to first turn the natural language inputs into vector embeddings. There were then the LSTM layers to imbue meaning to the embeddings.
- Decoder: The decoder also started with an embedding layer to turn the target vocab into embeddings. Then it had an LSTM layer to imbue meaning along with attention to get context from the Encoder.
- Attention: The attention mechanism was implemented by taking in the encoder outputs and a hidden state of the decoder. Then, attention_scores for the encoder outputs were calculated and used to make 
context vectors along with the decoder hidden state. The decoder hidden state and context vectors were then used along with learned weights and a softmax, tanh function to output probabilities for the next target token.

Repo Info and Running:

To find a more in-depth explanation of the code please go to the VideoInfo.txt for a link to a Google Drive that has a ~5 min video walking through the code. This video is also in .mp4 format 
if downloading it and viewing it locally is preferred. The actual code can be found in the jupyter notebook Amith_Chintalapati_Final_Project.ipynb or Python file amith_chintalapati_final_project.py.
To run, just run all on the jupyter notebook.

Future Work:
The paper also implemented a Seq2Tree semantic parser which seemed really interesting and complicated. It would be a great extension to try and implement that next!

Acknowledgements:
As previously stated all of this code was based on the paper "Language to Logical Form with Neural Attention" by Li Dong, and Mirella Lapata (2016) which provides clear and insightful instructions on implementation.

Enjoy!
