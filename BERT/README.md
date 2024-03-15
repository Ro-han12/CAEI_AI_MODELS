### What is BERT?
BERT language model is an open source machine learning framework for natural language processing (NLP). BERT is designed to help computers understand the meaning of ambiguous language in text by using surrounding text to establish context. The BERT framework was pretrained using text from Wikipedia and can be fine-tuned with question-and-answer data sets.

Historically, language models could only read input text sequentially -- either left-to-right or right-to-left -- but couldn't do both at the same time. BERT is different because it's designed to read in both directions at once. The introduction of transformer models enabled this capability, which is known as bidirectionality. Using bidirectionality, BERT is pretrained on two different but related NLP tasks: masked language modeling (MLM) and next sentence prediction (NSP).

The objective of MLM training is to hide a word in a sentence and then have the program predict what word has been hidden based on the hidden word's context. The objective of NSP training is to have the program predict whether two given sentences have a logical, sequential connection or whether their relationship is simply random.

### Background and history of BERT?
Google first introduced the transformer model in 2017. At that time, language models primarily used recurrent neural networks (RNN) and convolutional neural networks (CNN) to handle NLP tasks.

CNNs and RNNs are competent models, however, they require sequences of data to be processed in a fixed order. Transformer models are considered a significant improvement because they don't require data sequences to be processed in any fixed order.

Because transformers can process data in any order, they enable training on larger amounts of data than was possible before their existence. This facilitated the creation of pretrained models like BERT, which was trained on massive amounts of language data prior to its release.

In 2018, Google introduced and open sourced BERT. In its research stages, the framework achieved state-of-the-art results in 11 natural language understanding (NLU) tasks, including sentiment analysis, semantic role labeling, text classification and the disambiguation of words with multiple meanings. Researchers at Google AI Language published a report that same year explaining these results.

Completing these tasks distinguished BERT from previous language models, such as word2vec and GloVe. Those models were limited when interpreting context and polysemous words, or words with multiple meanings. BERT effectively addresses ambiguity, which is the greatest challenge to NLU, according to research scientists in the field. It's capable of parsing language with a relatively human-like common sense.

In October 2019, Google announced that it would begin applying BERT to its U.S.-based production search algorithms.

It is estimated that BERT enhances Google's understanding of approximately 10% of U.S.-based English language Google search queries. Google recommends that organizations not try to optimize content for BERT, as BERT aims to provide a natural-feeling search experience. Users are advised to keep queries and content focused on the natural subject matter and natural user experience.

BY December 2019, BERT had been applied to more than 70 different languages. The model has had a large impact on voice search as well as text-based search, which prior to 2018 had been error-prone with Google's NLP techniques. Once BERT was applied to many languages, it improved search engine optimization; its proficiency in understanding context helps it interpret patterns that different languages share without having to completely understand the language.

BERT went on to influence many artificial intelligence systems. Various lighter versions of BERT and similar training methods have been applied to models from GPT-2 to ChatGPT.