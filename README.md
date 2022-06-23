# NLP Tasks

### Task - 1 : Speech to Text
- Used python *speech_recognition* module to convert text to speech.
- First the given .wav file is loaded.
- Then the large file is converted to chunks and saved into a folder.
- Then using the *speech_recognition* module, these chunks are converted to text.

### Task - 2: Train an NLU model to classify intents and recognize entities

##### Task - 2.1 : Intent classification
  - It is a binary classification.
  - The classes are 'Intro' and 'Purpose'
  - Used Support Vector Machine for text classification.
  
##### Task - 2.2 : Named Entity Recognition  
- Python *spacy* module is used for training the model.
- There are entities like person, company and product.
- Initially, a blank english model is created.
- Then, the model is loaded using spacy.
- TRAINING DATA is created.
- NER model is trained using training data.


### Task - 3: Separate the sentences in the output of task 1. On each sentence, apply the
model trained in task 2 to classify its intent and recognize the entities present in it
### Task - 3: Export results to JSON file
- Separate the sentences in the output of task 1. It was done using python split() funcation.
- On each sentence, Task - 2 is applied.
- And results are stored in JSON file.
### Task - 4: Text Summarization

- Pretrained *transformers* model*tf-small* is used for text summarization.
- Basically, text summarization is 2 types.
- 1. Extractive summarization, 2. Abstractive Summarization
- As name suggests, extractive summarization extracts  sentences from the original text and returns as summary.
- Abstractive summarization on other hand generates overall summary of the original text.

### Steps to reproduce the results :
- Upload the .wav file to the environment (google colab in this case.)
- Install the required modules 
>  * !pip install transformers==2.8.0
>  * !pip install torch==1.4.0
>  * !pip install -U spacy
>  * !pip3 install SpeechRecognition pydub
>  * !python -m spacy download en_core_web_sm
>  * !pip install plac
 - Then run the code.
