# Question-answering-BERT-model

### Summary

This project includes the implementation of a BERT-based model which returns “an answer”, given a user question and a
passage which includes the answer of the question. For this question answering task, I used the [SQuAD 2.0](https://rajpurkar.github.io/SQuAD-explorer/) dataset. I started with the BERT-base pretrained model “bert-base-uncased” and fine-tune it to have a question answering task.


### What is SQuAD?

Stanford Question Answering Dataset (SQuAD) is a reading comprehension dataset, consisting of questions posed by crowdworkers on a set of Wikipedia articles, where the answer to every question is a segment of text, or span, from the corresponding reading passage, or the question might be unanswerable.

### Example of how the model works

* Data given:

`data = {"data":
    [
        {"title": "Tesla's Biography",
         "paragraphs": [
             {
                 "context": "Romeo and Juliet is a tragedy written by William Shakespeare early in his career"
                            "about two young Italian star-crossed lovers whose deaths ultimately reconcile their feuding families."
                            "It was among Shakespeare's most popular plays during his lifetime and, along with Hamlet,"
                            "is one of his most frequently performed plays.",
                            
                 "qas": [
                     {"question": "Who wrote Romeo and Juliet?",
                      "id": "Q1",
                      "answers":""
                      },
                 ]}]}]} `

* Answer:

Q: Who wrote Romeo and Juliet?
A: William Shakespeare
----------------------------------------

