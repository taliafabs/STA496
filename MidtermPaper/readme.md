# Post-2024 U.S. Presidential Election Vote Choice Analysis

## Objective & overview 🔍
Why did Americans elect Trump (again) in 2024? This project aims to identify key predictors of vote choice among 2024 Cooperative Election Study (CES) respondents and build on the work of Algara et al., Kuriwaki et al., and Camatarri. I approached vote choice modeling as a binary classification task and built and trained a two-layer logistic MLP using TensorFlow and keras to perform binary classification (identify Harris and Trump voters) in the 2024 CES survey dataset. I found that approval (or lack thereof) of incumbent President Joe Biden and economic conditions heavily influenced voters' decisions. Additionally, the interaction effects between race and region, race and the rural-urban divide, race and education, and race and gender had statistically significance effects on vote choice, but were not nearly as influential as the economy and incumbent presidential approval. My model achieved 92.8% validation accuracy after training via minibatch gradient descent using batch size 32, learning rate 0.05, L2-penalty 0.0001, and 100 epochs.

## Data 📊
* I primarily used the 2024 Cooperative Election Study (CES) Common Content dataset for this project. I downloaded it from Harvard dataverse via url. It can be found using this link: https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/X11EP6
* Additionally, I obtained historical presidential results data from FiveThirtyEight. I downloaded it from their GitHub repo via url and it can be found using this link: https://github.com/fivethirtyeight/election-results/blob/main/election_results_presidential.csv

## Inspirations 🧠
This project was inspired by the works of Kuriwaki et al., Algara et al., and Camatarri. Their publications can be found using the following links:
* https://www.cambridge.org/core/journals/american-political-science-review/article/geography-of-racially-polarized-voting-calibrating-surveys-at-the-district-level/6BEF8C3000B763699C27A4F9E8590516
* https://www.cambridge.org/core/journals/ps-political-science-and-politics/article/forecasting-partisan-collective-accountability-during-the-2024-us-presidential-and-congressional-elections/9D6C577734D4FDB6CEED4256C60EE4BD
* https://www.cambridge.org/core/journals/ps-political-science-and-politics/article/predicting-popularvote-shares-in-us-presidential-elections-a-modelbased-strategy-relying-on-anes-data/CC6B59BAC456CAC43C96F27FBAAF2290#article


## Contents 📚
* `code` contains the python notebooks with data cleaning and model training/optimization code. Note: the MidtermPaperCode.ipynb notebook won't render in GitHub (I believe that this is because PyMC was used for model diagnostics), but I've included the link to the Google Colaboratory. Alternatively, it can be downloaded.
* `data` contains the cleaned data that I used for analysis purposes
* `visualizations` contains .png versions of the visualizations included in the Exploratory Data Analysis section
  
## Links 🔗
* Midterm Paper Code: https://colab.research.google.com/drive/1Nv13U3kmJRq9LVnxUBEQtNX9y1gTxjlX?usp=sharing
* Model training and optimization learning diary: https://colab.research.google.com/drive/1hoV7zWkXoaG13T8iA9hn7XKn85SvQDwM?usp=sharing

## LLM Usage 🤖
Chat GPT 3.5 was used for latex formatting, IEEE citations, and code debugging.
