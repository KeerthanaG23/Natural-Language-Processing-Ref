#### https://colab.research.google.com/drive/1FTIeFD9PjcHgO3i8DFsapYL9Vl5u5UyH?usp=sharing
#### Code Mixed - https://github.com/dharun-narayanan/Code-Mixed-Data
#### Tense conversion - https://www.kaggle.com/code/pabasar/present-continuous-sentences-into-simple-present
#### Links that help you get a partially verified 8th question:
tense identification: https://stackoverflow.com/a/77072352
tense conversion (continuous present - simple present): https://pabasar.medium.com/changing-the-tense-with-nlp-techniques-turning-present-continuous-tense-sentences-into-simple-da14870fff47
#### Summarisation - https://github.com/smruthi49/Sem6-Projects/tree/main/Summarization
#### Grammar correction - https://github.com/MuthuPalaniappan925/NLP-Dump/tree/main
#### RR - https://github.com/Mr-Appu/College-Dump/tree/main/NLP
#### Fake news generation - https://github.com/oneturkmen/news-generation/blob/master/src/model_ngrams.py / https://github.com/mk-khalil/automated-news-generation-app
#### Sentence genration model - https://github.com/joshualoehr/ngram-language-model
#### Sent gen2 - https://github.com/shruthimohan03/Basic-Sentence-Generation-using-ngram/blob/main/Basic%20Sentence%20Generation%20using%20ngram%20approach.ipynb
![image](https://github.com/KeerthanaG23/Natural-Language-Processing-Ref/assets/116378322/1d22c432-de6a-44ca-ba6d-6f6408d3b8df)
#### Hugging face models -  https://github.com/laxmimerit/NLP-Tutorials-with-HuggingFace
#### https://ai.google.dev/tutorials/python_quickstart
#### Ref -  https://www.youtube.com/watch?v=NLvQ5oj-Sg4
#### Q&A - Llama fine tune - https://colab.research.google.com/drive/10X-R4nIDPc_P9egafd4wnGK8s2nEy7Ra?usp=sharing
#### https://jalammar.github.io/illustrated-bert/
#### GPT VS LLAMA VS BART https://medium.com/@reyhaneh.esmailbeigi/bert-gpt-and-bart-a-short-comparison-5d6a57175fca 
#### Grammer correction - https://github.com/PrithivirajDamodaran/Gramformer
#### 
![image](https://github.com/KeerthanaG23/Natural-Language-Processing-Ref/assets/116378322/3acadb3b-c4b4-4538-a28d-0b46a1cd47fb)
#### Sentiment analysis -  https://drive.google.com/drive/folders/1TK9k41RT8Nf3IhzerNWHpEqWztsk2gAP
#### https://colab.research.google.com/drive/1xyaAMav_gTo_KvpHrO05zWFhmUaILfEd?usp=sharing#scrollTo=fsFWSTQeJnrn

#### LSTM - https://kgptalkie.com/text-generation-using-tensorflow-keras-and-lstm/
#### https://github.com/entbappy/NLP-Projects-Notebooks/blob/master/En_Hi_language_translation.ipynb
#### Active to passive - https://github.com/rishiagarwal2000/Active-to-Passive-Voice
Code:

import spacy
nlp = spacy.load('en_core_web_sm')
doc = nlp("They make cars in Detroit")
s = list(doc)
tmp,temp,sub = "","",-1
for i in doc:
    if i.pos_ == 'VERB':
        s[i.i] = i
    elif i.dep_ == 'nsubj':
        sub = i.i
        temp = i
    elif i.dep_ == 'dobj':
        tmp = i.text.capitalize()
        s[i.i] = temp
        s.insert(i.i,"by")

s[sub] = tmp
print(' '.join(str(e) for e in s))

https://www.phind.com/search?cache=i5ry16qms58dq70cibykva7l
https://huggingface.co/docs/transformers/en/model_doc/bert
### Text reordering - https://github.com/gioelecrispo/text-reorderer/blob/master/text-reorderer.ipynb
