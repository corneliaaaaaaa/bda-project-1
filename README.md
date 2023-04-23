# big-data-and-business-analytics-mid-project

We use Yahoo! stock news from 2020-2023 to predict the rise and fall of prices of stocks from the over-the-counter market and stock exchange. The process is as follows
- r1_part1.ipynb
  1. read stock data from 2019-2023
  2. filter the dates that a specific stock rise or fall to a specific extent from 2020-2023 (e.g. rise 5% after 3 days)
  3. store the filtered dates in a csv file
- r1_part2_and_r2.ipynb
  1. read the data of Yahoo! stock news from 2019-2023
  2. filter the news that was posted on the date when the price of the specific stock rised or fell to a specific extent
  3. preprocess the news (filter keywords, remove news that is too short...)
  4. add labels to each record, and divide the data into training set and testing set
  5. pick features, train and test
      - method 1
        - tokenize with monpa
        - pick features for the group of news with df-chi2
        - train and test with Naive Bayes, kNN, Decision Tree, Random Forest, SVM...
      - method 2
        - tokenize with jieba
        - pick features for each news with tf
        - put the feature set into nltk models (Naive Bayes, SVM, Decision Tree)
