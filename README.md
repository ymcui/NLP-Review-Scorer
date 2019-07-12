# NLP Review Scorer

**Disclaimer: This is only a toy. You should seriously treat your rebuttal despite the what scores are given below. Wish you good luck with your paper submission!**

**Also, as the notebook will run under YOUR CONTROL, please rest assured that your review won't be recorded in any form and I have no access to it.**

I know some of you are thinking about how to convert paper review to a numerical score.
Yes, the time has come.

In this notebook, you will be able to **convert your paper review to overall score (hopefully in range 1~5) as well as reviewer confidence.**

In my own experience, the prediction on reviewer confidence is not that accurate.

## News
**July 12, 2019	New model trained on 5.7K reviews is available. *Seems to be more accurate*. **
July 11, 2019	Initial version released, trained on 3K reviews.

## Quick Introduction
The model is trained on real reviews from [PeerRead dataset](https://github.com/allenai/PeerRead) as well as in-house collected reviews for training. Note that, we only include the reviews with open access, and the private reviews without author permissions are not included. 
The implementation was based on `run_classifier.py` in [BERT repository](https://github.com/google-research/bert) with slight modifications.

**As the review data is rather private, I won't be able to release them.**

## Prerequisites
- You should know how to use [Google Colab](http://colab.research.google.com)
- You are somewhat familiar with [BERT](https://github.com/google-research/bert)

## How-To
1. Copy (do not need to download) the one of the following model to your Google Drive
- V2, latest version trained with 5.7K reviews: [Google Drive](https://drive.google.com/open?id=1HBauWO1kjvhyQcerXbq9NPzJaBAcW0bZ)
- V1, initial version trained with 3K reviews: [Google Drive](https://drive.google.com/open?id=1WsMm_h_cHgj0gEDvfELmLzklVul9GOjU)

2. Then, [go to Google Colab for further instructions](https://colab.research.google.com/drive/1AmmRUJa3_ZhFrpRsz7ovar6-L-sV62tU)


## Sample Output (v2 version)
Note that, in real situations, your input review will be much longer than these examples!

```
***********REVIEW**************
This is a very good paper, outstanding paper, brilliant paper.
I have never seen such a good paper before.
It was well-written and the models are novel.
The evaluations are sound and the results achieve state-of-the-art performance.
It should be definitely accepted or I will be angry.
***********SCORE***************
Paper	Recommendation	Confidence
EMNLP	4.5141506	3.8331783
********************************
```
​
```
***********REVIEW**************
The paper was rather bad that I don't want to see it again.
The idea was trivial and the evaluations are not convincing to me at all.
We should reject this paper or I won't review for this venue in the future.
***********SCORE***************
Paper	Recommendation	Confidence
EMNLP	1.3770846	4.0270653
********************************
```

## Disclaimer
This is not a product by Joint Laboratory of HIT and iFLYTEK Research (HFL). 

## Acknowledgement
I personally thank Google Colab for providing free computing resources for researchers.

## Issue
If there is any problem, please submit a GitHub Issue.
