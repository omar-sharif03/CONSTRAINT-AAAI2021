<img title="" src="Figures/image-constraint.PNG" alt="">

## Combating Hostility: Covid-19 Fake News and Hostile Post Detection in Social Media

**Author:** Omar Sharif, Eftekhar Hossain and Mohammed Moshiul Hoque

**Venue:** Shared task description paper of CONSTRAINT workshop collocated with AAAI-2021 . [CONSTRAINT@AAAI 2021](https://constraint-shared-task-2021.github.io/)

**Paper Link:** [https://arxiv.org/abs/2101.03291](https://arxiv.org/abs/2101.03291)

`Code and dataset of the tasks are released here. In order to use the dataset interested ones have to follow policy of workshop organizers`

## Abstract

This paper illustrates a detail description of the system and its results that developed as a part of the participation at CONSTRAINT shared task in AAAI-2021. The shared task comprises two tasks: a) COVID19 fake news detection in English b) Hostile post detection in Hindi. Task-A is a binary classification problem with fake and real class, while task-B is a multi-label multi-class classification task with five hostile classes (i.e. defame, fake, hate, offense, non-hostile). Various techniques are used to perform the classification task, including SVM, CNN, BiLSTM, and CNN+BiLSTM with tf-idf and Word2Vec embedding techniques. Results indicate that SVM with tf-idf features achieved the highest 94.39% weighted f1 score on the test set in task-A. Label powerset SVM with n-gram features obtained the maximum coarse-grained and fine-grained f1 score of 86.03% and 50.98% on the task-B test set respectively.

## Contribution
- Develop various machine learning and deep learning-based models to detect hostile texts in social media.
- Present performance analysis and qualitative error analysis of the system.

## Task Description

The CONSTRAINT shared task comprises of two tasks: task-A and task-B. The goal of task-A is to identify whether a tweet contains real or fake information. The tweets are related to the Covid-19 pandemic and written in English. In task-B, we have to perform multi-label multi-class classication on five hostile dimensions such as fake news, hate speech, ofensive, defamation and non-hostile.

- **Fake**: Articles, posts and tweets provide information or make claims which are verified not to be true.
- **Real**: The articles, posts and tweets which provided verified information and make authentic claims.
- **Hate speech**: Post having the malicious intention of spreading hate and violence against specific group or person based on some specific characteristics such as religious beliefs, ethnicity, and race.
- **Offensive**: A post contains vulgar, rude, impolite and obscene languages to insult a targeted individual or a group.
- **Defamation**: Posts spread misinformation against a group or individuals
which aim to damage their social identity publicly.
- **Non-hostile**: Posts without any hostility.

## Dataset Analysis

The number of instances used to train, validate and test the models summarized in table 1.

<img title="" src="Figures/Table1.PNG" alt="">

To get the useful insights, we investigated the train set. Statistics of the train set exhibited in table 2.

<img title="" src="Figures/Table2.PNG" alt="">

Figure 1 depicts the number of texts fall in various length range.
<img title="" src="Figures/Fig1.PNG" alt="">

## System Overview
Figure 2 presents the schematic diagram of our system, which has three major phases: preprocessing, feature extraction and classification.
<img title="" src="Figures/Fig2.PNG" alt="">

## Results 
Table 3 presents the evaluation results of task-A on the test set.
<img title="" src="Figures/Table3.PNG" alt="">

Evaluation results of task-B on the test set are presented in table 4.
<img title="" src="Figures/Table4.PNG" alt="">

Tables 5a-5f represent the confusion matrices of the classes for task-A and B.
<img title="" src="Figures/Table5.PNG" alt="">

Some misclassified examples with there actual (A) and predicted label (P) presented in table 6.
<img title="" src="Figures/Table6.PNG" alt="">

## Conclusion
This paper presents the system description with detailed results and error analysis developed in the CONSTRAINT 2021 shared task. Various learning technique have explored with tf-idf feature extraction, andWord2Vec embedding technique to accomplish the tasks A and B. Results shows that SVM with tf-idf achieved the highest of 94.39% f1 scores for the task-A and LPSVM with n-gram (1, 3) obtained the highest of 86.03% f1 scores for the task-B. However, the BERT pre-trained model provided the 98% accuracy in task-A and 97% accuracy in task-B. Since CNN and BiLSTM did not achieve satisfactory accuracy, it will be interesting to see how they perform after applying ensemble technique or adding attention layer. Increasing the number of posts in hostile classes can help to improve the performance of the models. These issues will address in future work.

## Ackonwlegement
Without my teammate [Eftekhar Hossain's](https://eftekhar-hossain.github.io/portfolio/) support and dedication this work would not be possible. Finally, thanks to [Prof. Dr. Mohammed Moshiul Hoque](https://www.researchgate.net/profile/Moshiul_Hoque) for his valuable guidance.

## Note
`If you find any anomaly or have any query/suggestion feel free to ping.`
