# Emotion_Detection_Roberta
Tweet Emotion Detection using Encoder model RoBERTa-base

RoBERTa-base:
RoBERTa shares the same encoder-only, Transformer-based architecture as BERT, with identical layers and attention heads. Both BERT-base and RoBERTa-base consist of 12 layers, a 768-dimensional hidden size, and 12 attention heads. However, BERT-base has approximately 110 million parameters, while RoBERTa-base has around 125 million parameters.
RoBERTa is an optimised version of BERT, designed to address limitations in BERT’s training methodology. BERT’s training objectives include Masked Language Modeling (MLM) and Next Sentence Prediction (NSP). In contrast, RoBERTa removes the NSP objective, focusing solely on the MLM task, which has been shown to improve downstream performance. Additionally, RoBERTa uses dynamic masking, where different words are masked in each training epoch, providing the model with varied contexts. This differs from BERT’s static masking, in which certain words are randomly selected to be masked, and the masking pattern remains fixed across all training epochs.
Moreover, RoBERTa is trained on a much larger dataset—approximately 160GB, or around 10 times the size of BERT’s 16GB dataset—allowing for richer language representation. It is also trained with more epochs and larger batch sizes, further enhancing its robustness and effectiveness for natural language understanding tasks.

After calculating the optimal thresholds, the following is the model performance observed in each case:
RoBERTa-base
{'f1_micro': 0.6978361669242659,
 'f1_macro': 0.6184752027930999,
 'accuracy_label': 0.8619593998234775,
 'accuracy_all': 0.2226537216828479}

RoBERTa-base:
<img width="324" alt="image" src="https://github.com/user-attachments/assets/42cce29c-d4f4-462f-aa5a-d4795c20a623" />





