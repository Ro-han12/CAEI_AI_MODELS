### What is BERT?
BERT: BIDIRECTIONAL ENCODER REPRESENTAION OF TRANSFORMERS.
BERT language model is an open source machine learning framework for natural language processing (NLP). BERT is designed to help computers understand the meaning of ambiguous language in text by using surrounding text to establish context. The BERT framework was pretrained using text from Wikipedia and can be fine-tuned with question-and-answer data sets.

![image](https://github.com/Ro-han12/CAEI_AI_MODELS/assets/95674406/49e77494-ceb1-4f41-9493-31892bd56afc)


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

### How BERT works?
The goal of any given NLP technique is to understand human language as it is spoken naturally. In BERT's case, this means predicting a word in a blank. To do this, models typically train using a large repository of specialized, labeled training data. This process involves linguists doing laborious manual data labeling.

BERT, however, was pretrained using only a collection of unlabeled, plain text, namely the entirety of English Wikipedia and the Brown Corpus. It continues to learn through unsupervised learning from unlabeled text and improves even as it's being used in practical applications such as Google search.

BERT's pretraining serves as a base layer of knowledge from which it can build its responses. From there, BERT can adapt to the ever-growing body of searchable content and queries, and it can be fine-tuned to a user's specifications. This process is known as transfer learning. Aside from this pretraining process, BERT has multiple other aspects it relies on to function as intended, including the following:
1.Transformers
Google's work on transformers made BERT possible. The transformer is the part of the model that gives BERT its increased capacity for understanding context and ambiguity in language. The transformer processes any given word in relation to all other words in a sentence, rather than processing them one at a time. By looking at all surrounding words, the transformer enables BERT to understand the full context of the word and therefore better understand searcher intent.

This is contrasted against the traditional method of language processing, known as word embedding. This approach was used in models such as GloVe and word2vec. It would map every single word to a vector, which represented only one dimension of that word's meaning.

### Masked language modeling
Word embedding models require large data sets of structured data. While they are adept at many general NLP tasks, they fail at the context-heavy, predictive nature of question answering because all words are in some sense fixed to a vector or meaning.

BERT uses an MLM method to keep the word in focus from seeing itself, or having a fixed meaning independent of its context. BERT is forced to identify the masked word based on context alone. In BERT, words are defined by their surroundings, not by a prefixed identity 

### Self-attention mechanisms
BERT also relies on a self-attention mechanism that captures and understands relationships among words in a sentence. The bidirectional transformers at the center of BERT's design make this possible. This is significant because often, a word may change meaning as a sentence develops. Each word added augments the overall meaning of the word the NLP algorithm is focusing on. The more words that are present in each sentence or phrase, the more ambiguous the word in focus becomes. BERT accounts for the augmented meaning by reading bidirectionally, accounting for the effect of all other words in a sentence on the focus word and eliminating the left-to-right momentum that biases words towards a certain meaning as a sentence progresses.
Diagram showing how BERT identifies meanings of words
BERT examines individual words in context to determine the meaning of ambiguous language.

For example, in the image above, BERT is determining which prior word in the sentence the word "it" refers to, and then using the self-attention mechanism to weigh the options. The word with the highest calculated score is deemed the correct association. In this example, "it" refers to "animal", not "street". If this phrase was a search query, the results would reflect this subtler, more precise understanding BERT reached.

### Next sentence prediction
NSP is a training technique that teaches BERT to predict whether a certain sentence follows a previous sentence to test its knowledge of relationships between sentences. Specifically, BERT is given both sentence pairs that are correctly paired and pairs that are wrongly paired so it gets better at understanding the difference. Over time, BERT gets better at predicting next sentences accurately. Typically, both NSP and MLM techniques are used simultaneously.
![image](https://github.com/Ro-han12/CAEI_AI_MODELS/assets/95674406/1efae604-2d3a-4fa1-8f02-ff01440c2d91)

### Applications and Usage of BERT

1. Natural Language Understanding (NLU): BERT is widely used in NLU tasks such as sentiment analysis, semantic role labeling, text classification, and word sense disambiguation. Its ability to capture context and ambiguity in language makes it effective in understanding the meaning of text.

2. Search Engine Optimization (SEO): Google applies BERT to its search algorithms, enhancing the understanding of search queries and providing more relevant search results. BERT's ability to interpret context and user intent improves the search experience by delivering more accurate and useful results.

3. Question Answering Systems: BERT can be fine-tuned for question answering systems, where it understands the context of questions and retrieves relevant answers from large text corpora. It powers virtual assistants, chatbots, and FAQ systems, providing accurate responses to user queries.

4. Natural Language Generation (NLG): BERT can be used in NLG tasks to generate human-like text based on given prompts or contexts. It understands the nuances of language and can generate coherent and contextually appropriate responses.

5. Text Summarization: BERT can be leveraged for text summarization tasks, where it condenses large amounts of text into shorter, more concise summaries while preserving key information and context.

6. Named Entity Recognition (NER): BERT is effective in NER tasks, where it identifies and classifies named entities such as persons, organizations, locations, dates, and numerical expressions in text. It improves the accuracy of information extraction systems.

7. Machine Translation: BERT can enhance machine translation systems by improving the understanding of context and idiomatic expressions in source and target languages. It contributes to more accurate and fluent translations between languages.

8. Sentiment Analysis: BERT can analyze the sentiment expressed in text, determining whether the sentiment is positive, negative, or neutral. It is used in social media monitoring, customer feedback analysis, and opinion mining applications.

9. Document Classification: BERT can classify documents into predefined categories or topics based on their content. It is used in document management systems, news categorization, and content recommendation engines.

10. Conversational AI: BERT powers conversational AI systems by enabling more natural and context-aware interactions between users and virtual assistants, chatbots, or dialogue systems. It improves the understanding and generation of human-like responses in conversations.

Overall, BERT's versatility and effectiveness in various NLP tasks make it a foundational tool in natural language processing, driving advancements in AI applications across industries such as healthcare, finance, e-commerce, education, and more. Its ability to understand context, ambiguity, and user intent revolutionizes how computers interact with and comprehend human language.