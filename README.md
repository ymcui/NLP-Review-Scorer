# NLP Review Scorer

**Disclamer: This is only a toy. You should seriously treat your rebuttal despite the what scores are give below. Wish you good luck for your paper submission!**

I know some of you are thinking about how to conver my review to numerical score.
Yes, the time has come.

In this notebook, you will be able to **convert your review to overall score (hopefully in range 1~5) as well as reviewer confidence.**

## Quick introduction
The model is trained on 3K real reviews from [PeerRead dataset](https://github.com/allenai/PeerRead) as well as in-house collected reviews for training. 
The implementation was based on `run_classifier.py` in [BERT repository](https://github.com/google-research/bert) with slight modifications.

**As the review data is rather private, I won't be able to release them. **

## Prerequisites
- You should know how to use [Google Colab](http://colab.research.google.com)
- You are somewhat familiar with [BERT](https://github.com/google-research/bert)

## How-To
- Download all contents in this repository.
- [Go to Google Colab for further instructions](https://colab.research.google.com/drive/1AmmRUJa3_ZhFrpRsz7ovar6-L-sV62tU)

## Issue
If there is any problem, please submit a GitHub Issue.