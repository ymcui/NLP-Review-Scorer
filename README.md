# NLP Review Scorer

**Disclamer: This is only a toy. You should seriously treat your rebuttal despite the what scores are give below. Wish you good luck for your paper submission!**

I know some of you are thinking about how to conver my review to numerical score.
Yes, the time has come.

In this notebook, you will be able to **convert your review to overall score (hopefully in range 1~5) as well as reviewer confidence.**

**As the notebook will run under YOUR CONTROL, please rest assured that your review won't be recorded in any form and I have no access to it.**

## Quick introduction
The model is trained on 3K real reviews from [PeerRead dataset](https://github.com/allenai/PeerRead) as well as in-house collected reviews for training. 
The implementation was based on `run_classifier.py` in [BERT repository](https://github.com/google-research/bert) with slight modifications.

Included venue: ACL, EMNLP, CoNLL, NAACL, COLING, ICLR (scores are scaled to 1~5)

**As the review data is rather private, I won't be able to release them.**

## Prerequisites
- Copy (do not need to download) the latest model to your Google Drive: https://drive.google.com/open?id=1WsMm_h_cHgj0gEDvfELmLzklVul9GOjU
- You should know how to use [Google Colab](http://colab.research.google.com)
- You are somewhat familiar with [BERT](https://github.com/google-research/bert)

## How-To
- Download all contents (*.py) in this repository.
- [Go to Google Colab for further instructions](https://colab.research.google.com/drive/1AmmRUJa3_ZhFrpRsz7ovar6-L-sV62tU)

## Sample Output
```
**************REVIEW***********
this is a very good paper, outstanding paper, brilliant paper. 
I have never seen such a good paper before. 
It was well-written and the models are novel. 
The evaluations are sound and the results achieve state-of-the-art performance. 
It should be definitely accepted or I will be angry.
**************SCORE***********
paper   recommendation  confidence
emnlp2019   3.4766932   3.4420846
********************************
```
​
```
**************REVIEW***********
The paper was rather bad that I don't want to see it again. 
The idea was trivial and the evaluations are not convincing to me at all. 
We should reject this paper or I won't review for this venue in the future,
**************SCORE***********
paper   recommendation  confidence
emnlp2019   2.011398    3.8701794
********************************
```

## Disclaimer
This is not a product by HFL. 

## Issue
If there is any problem, please submit a GitHub Issue.