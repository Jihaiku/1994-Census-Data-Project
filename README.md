# 1994-Census-Data-Project

![seal-42704_1280](https://user-images.githubusercontent.com/48660919/69014771-dcd76900-095b-11ea-82af-5c133d5a30a3.png)

## Introduction
Today we're going to be looking over a dataset created by Barry Becker pertaining to the 1994 Census for the United States.

Purpose
What we're going to be figuring out with it initially is whether or not that people make over $50,000 or under that per year with the information that we obtain with the initial data. This will help us provide answers to our hypothetical employee-the government-to better tax the people by predicting their tax brackets based on their information. Which in turn may help them through more knowledgable tax policies.

## Here are some of my findings:

One of the first things we see after cleaning up the data is that there are very few officially recognized categories of ethnicities which you wouldn't particularly see in a more modern day US Census. The ramnifications of this on our census data is that either our data has Hispanic, Asian descent, or Two or more races all being put into Other, they're mixed into the other groups, or they were just not accounted for. Of which none of those answers seem to be ideal and do throw some shades of grey upon the accuracy of our data.

<br>
![Age x race](https://user-images.githubusercontent.com/48660919/69014811-26c04f00-095c-11ea-999e-5e3d958bc9c4.PNG)

Another interesting point is that while divorce is present in the dataset, many people who filled out as Divored/Separated, Never-married, and widowed were primarily between groups 2 and 5 of education which are 2: Middle School Grad, 3: High School Grad, 4: Some college, and 5: Undergraduate. Whereas the married category had a much wider spread that went all the way to 7: Doctorate. While the knee jerk reaction is to say that less educated people tend to not remain or get married, I think this moreso has to do with the census data weighing more towards having people from the Silent Era and Early Baby Boomer era not necessarily requiring a higher education than you would see in the 21st century. On top of that the categories outside of married may have some correlation to more older people or very young people which would also make sense for the education types that they have listed. 

<br>
![Martial status x education](https://user-images.githubusercontent.com/48660919/69014817-2fb12080-095c-11ea-8650-9bbdf402ef54.PNG)

With over 25 year old data, this visualization interested me the most becasue I had a misconception that the categories would be skewed in several more ways than what it came out to be. Almost every group had a majority of their applicants being between 2 and 5, which are middle school graduate and college undergraduate with the exception of Asian-Pacific Islander ranging from Elementary School graduate to docorate. This visualization does more with what it doesn't show than what it does show, and that is the sign that education in 1994 was fairly spread out amongst the people in the area that this survey was taken.
<br>

![Education x race](https://user-images.githubusercontent.com/48660919/69014815-2d4ec680-095c-11ea-9a81-7727ab932cb0.PNG)

Question from the beginning:
Can we predict whether or not someone made over $50,000 or under that per year with the information that we have?

(True Negative, False Positive)
(False Negative, True Positive)

![CFMX](https://user-images.githubusercontent.com/48660919/69014813-2aec6c80-095c-11ea-9015-cf57ce7a59a2.PNG)

Whew we're done with the Gridsearch CV and have gotten to the final part of our journey. We have cleaned up several edge case variables out of the processing phase and managed to make our final results better than what they were when many variables were highly correlated (most of which we retroactively cut out so not to make this several dozen lines longer).

## Recommendation
Given that we are 85% correct with a fairly higher Recall over Precison after extensive processing let's provide our recommendation on what is currently completed.

1. We shoulf focus on either marital status or relationship but having both within the test make our ability to determine correct results harder.
2. Capital gains and capital loss do very little for our model as separate columns but could be better if we use them as a single one.
3. We should provide proper labeling for unemployed, never worked, and so on so their data can remain in the model instead of needing to be dropped for no proper labels.

## Next Steps
With any project there are constraints found within it that we could have worked on or improved to make the test better overall. I think that there are a few optional items that given enough time I would add to this project. Those options are:
1. Perform a different machine learning algorithm with the same goal.
2. Use different feature engineering methods to improve our performance scores.
3. Refine what columns are used in the machine learning process to see which ones weaken the modelling.
Model Results
Regardless of what we could work on to improve the model, what we for sure know is that given our current standing with what we worked on we are able to predict what category of 'tax bracket' you would be 85% of the time based on our data set based on several categories including race, sex, martial status, and occupation. What this means is that we can provide a fairly strong predicted answer to the US government when determining peoples ability to pay taxes and with some refinement and secondary testing we should be able to improve this score immensely.

Thank you for your time and I hope this project was an interesting read and dive into my thought process.
