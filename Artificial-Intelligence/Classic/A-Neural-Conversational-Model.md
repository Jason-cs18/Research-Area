# Notes on <A Neural Conversational Model, Oriol Vinyals, Quoc V.Le, ICML Deep Learning Workshop 2015>

1. What is the paper about? what is the issue the authors are trying to solve?

The paper focused on applying seq2seq framework on conversational tasks. The author mainly used deep neural recurrent model to solve the automatic reply in the conversational chatbot. 

2. What was the start of the world before this paper? How did this change that?

Before this paper, engineers often use human-ruled approach to construct the converational chatbot. In this paper, authors trained the deep recurrent model end2end with two real datasets and use it as conversational model.

3. How do the authors go about trying to solve the issue? What's main idea? What are the paper's main contribution?

Authors mainly utilized the seq2seq framework to train the deep recurrent model end2end. In seq2seq, they inputed the previous sentences as the context and use the output as reply messages. Compared to the traditional approach, author found that the seq2seq model is automatic and efficient method in conversational tasks.

4. How did the authors do? Is the evaluation sound and unbiased? Are the authors' result sufficiently justified in the paper?

Authors experimented the recurrent model on two real datasets: IT helpdesk troubleshooting dataset (closed-domain) and movie transcript dataset (open-source). Due to the lackness of the common measurement on this task, authors used the perplexity as the metrix. Compared to the N-gram model and human-ruled approaches, the seq2seq framework performs better. To make evaildation more strong, they adopt the human evaluation. In evaluation, they picked 200 questions from dataset and show the answers from human-ruled and seq2seq approaches to four people. If three out of four people judges agrees, they record the score. But from my perspective, this results are biased because they may piched questions biased and different people would be interest on different views of answers.

5. How well is the paper written?

The paper is written in such clear flow and makes reader read smoothly.