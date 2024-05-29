############

Project Name: Fortune-Gen

############

Project Definition: Fortune-Gen is a generator for fortune poems 
in the style found in some Turkish brand gums.

############

Problem Definition: Poems that come with the gums are few in
number and it is common to get the same poem from different gums.
They also lack diversity in themes, sticking only to love life
related fortunes.

I sought to diversify the fortune poems in number and theme by
automating the writing proccess.

############

Usage: This project includes a BERT model trained on Turkish data to classify 
fortunes into love or money themes. Sentences are first generated using an
Ngram model. The classification process then selects sentences matching the
desired theme until a 4-line poem is created. To generate classified 
fortunes please follow the steps below:

0. download the model.safetensors from the google drive and put it under the model file
https://drive.google.com/drive/folders/1KB6B6h3KQOJ9E_yow8cn-wZ6SX-N7nSI?usp=sharing
2. pip install -r requirements.txt to download the required libraries and packages
3. do the imports
4. execute the provided codes for data preprocessing, trigram model creation, and starter
word generation.
5. execute the codes for preparing the data for training the model and evaluation 
(do not train the model if you will use the saved model)
6. run the pre-trained model (or train the model)
7. use the generatePoem function to generate fortune poems, entering the desired theme 
as an argument, available themes are "love" and "money".
8. use printPoem to post-process and print the generated and classified fortune poem.

############

Evaluation: The classification model has a built-in accuracy check
that works well. 

As for text generation, sentences created are
satisfactory in qualitative evaluation done by asking my friends
for their thoughts.

A further evaluation metric I thought of is checking whether 
lines rhyme or not. I couldn't implement it due to time restrictions.

############

Reflection on the project: I think this project was very fun and
informative to put together. 

One big problem I faced was the lack of available data to put together 
a satisfactorily large corpus, especially regarding data for non-love-related poems.
I had to find workarounds to maximize the limited data I had.

############

