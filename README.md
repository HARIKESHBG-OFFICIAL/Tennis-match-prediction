# Tennis-match-prediction
Dataset credit:https://www.kaggle.com/datasets/dissfya/atp-tennis-2000-2023daily-pull


I have wanted to build a machine learning model which could predict matches for a game or sport like  chess,tennis and badminton etc.
My goal of this project is to build a tennis match predictor.

I used pandas and scikit-learn to build a Random Forest model.
I used a dataset from kaggle for training this.

The encoding techniques I used here are OneHotEncoding,Binary Encoding.
I  converted the categorical target into a binary label by mapping Player 1 wins to 1 and losses to 0 for the output feature.
I extracted details from date using the datetime library .
For the Score column, I did not apply a standard encoding technique.
Instead, I parsed the match score text and engineered numerical features such as total games won, total games lost, number of sets played, and the absolute game difference. 
This transforms unstructured score strings into structured numeric data that can be used by a machine learning model. This approach is best described as text-based feature engineering or domain-specific feature extraction rather than categorical encoding.
I  used numeric features such as the players’ ranks (Rank_1, Rank_2), points (Pts_1, Pts_2), and betting odds (Odd_1, Odd_2) directly.
