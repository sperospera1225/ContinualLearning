# Distributed Classification Model of Streaming Tweets based on Dynamic Model Update

M. -S. Kim and H. -Y. Kwon, "Distributed Classification Model of Streaming Tweets based on Dynamic Model Update," 2022 IEEE International Conference on Big Data and Smart Computing (BigComp), 2022, pp. 47-51, doi: 10.1109/BigComp54360.2022.00019.

![image](https://user-images.githubusercontent.com/67995592/191178037-4ec5f14d-e8f7-4485-b16f-e8e8ec6c6215.png)
![image](https://user-images.githubusercontent.com/67995592/191178185-eab7dbf1-2bfb-4b5f-bc99-1e6a460ede9f.png)


#
Abstract:
In this study, we propose a distributed architecture that dynamically updates the model for classifying tweet streams generated in real time. Our architecture ingests data streams through Apache Kafka and classifies them based on Apache Spark Streaming. In order to dynamically reflect input stream changes into the classification model, we design the classification model that can be dynamically updated by updating the tokenizer and classifier for new tweet streams. The proposed architecture can provide effective classification for data streams due to the dynamic update and can efficiently process through parallel processing of distributed environments. Through experiments using cyberattack-related tweets, we show that our classification model gradually improves the classification accuracy from 0.8869 when the initial 50,000 tweets are used to 0.9094 when 200,000 tweets are accumulated by F1-score.

Published in: 2022 IEEE International Conference on Big Data and Smart Computing (BigComp)
