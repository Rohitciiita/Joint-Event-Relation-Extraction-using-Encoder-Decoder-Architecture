# Joint-Event-Relation-Extraction-using-Encoder-Decoder-Architecture

Introduction:

Joint Event-Relation Extraction using Encoder-Decoder Architecture is an NLP approach that extracts events and relations from text simultaneously. It utilizes an encoder-decoder model, with the encoder capturing contextual information and the decoder generating event and relation sequences. This joint extraction improves understanding by capturing complex interactions between entities and events. It enables structured information extraction from unstructured text, benefiting applications like information retrieval and knowledge graph construction.


System Requirements:

Python 3.5 +
Pytorch 1.1.0
CUDA 8.0


Datasets:

The data is available at: https://drive.google.com/drive/u/1/folders/1fYP9PUQYRV0JWBa-N3CwuGkOCeBielT9
To obtain the Word2Vec embeddings and BERT embeddings, download 'w2v.txt' and 'BERT_embeddings.txt' from the aforementioned link.



Running the Code:

Python3: python3  Joint_Event_Extraction.py  gpu_id  random_seed  source_data_dir  target_data_dir  train/test  w2v/bert

IPython: Run individual cells of NLP_Proj6_Grp_19.ipynb

set the data folder and the output saving folder: src_data_folder = path trg_data_folder = path + 'Model'

for switching between training and testing phases, set the following parameters under if __name__ == "__main__":, job_mode = 'train' or job_mode = 'test'

for switching between Word2Vec and BERT embeddings, set the following parameters under if __name__ == "__main__":, embedding_type = 'w2v' or embedding_type = 'bert'

