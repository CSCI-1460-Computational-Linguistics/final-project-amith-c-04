Semantic Parser: Seq2Seq Encoder-Decoder Semantic Parser with Attention

Semantic Parsing is when natural language inputs are translated into logical representations and structures of themselves. This project was aiming to replicate the model created in 
"Language to Logical Form with Neural Attention" by Li Dong, Mirella Lapata. They implemented both a Seq2Seq semantic parser with attention and a Seq2Tree semantic parser. This project
only implemented the Seq2Seq parser. The model was comprised of an Encoder class, Decoder class, Attention class, and EncDec Class. The Encoder and Decoder classes used LSTM's to imbue the 
embeddings with meaning. An attention mechanism was used in the Decoder class to make sure the outputs were influenced by the Encoder. Python was the language used to implement this with 
Pytorch.

To find a more in-depth explanation of the code please go to the VideoInfo.txt for a link to a Google Drive that has a ~5 min video walking through the code. This video is also in .mp4 format 
if downloading it and viewing it locally is preferred. The actual code can be found in the jupyter notebook Amith_Chintalapati_Final_Project.ipynb or python file amith_chintalapati_final_project.py.

Enjoy!
