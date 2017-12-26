### 1. You are just getting started on this project. What is the first thing you do? Assume each of the steps below would take about an equal amount of time (a few days).
**Answer:** Spend a few days training a basic model and see what mistakes it makes.

### 2. For the output layer, a softmax activation would be a good choice for the output layer because this is a multi-task learning problem. True/False?
**Answer:** True

### 3. You are carrying out error analysis and counting up what errors the algorithm makes. Which of these datasets do you think you should manually go through and carefully examine, one image at a time?
**Answer: ** 500 images on which the algorithm made a mistake

### 4. After working on the data for several weeks, your team ends up with the following data:
**Answer: ** false

### 5. The distribution of data you care about contains images from your car’s front-facing camera; which comes from a different distribution than the images you were able to find and download off the internet. How should you split the dataset into train/dev/test sets?
**Answer: ** Choose the training set to be the 900,000 images from the internet along with 80,000 images from your car’s front-facing camera. The 20,000 remaining images will be split equally in dev and test sets.

### 6. Assume you’ve finally chosen the following split between of the data:
**Answer: ** 
* **Your algorithm overfits the dev set because the error of the dev and test sets are very close.**
* **You have a large data-mismatch problem because your model does a lot better on the training-dev set than on the dev set**

### 7. Based on table from the previous question, a friend thinks that the training data distribution is much easier than the dev/test distribution. What do you think?
**Answer: ** false

### 8. The results from this analysis implies that the team’s highest priority should be to bring more foggy pictures into the training set so as to address the 8.0% of errors in that category. True/False?
**Answer: ** False because this would depend on how easy it is to add this data and how much you think your team thinks it’ll help.

### 9. You can buy a specially designed windshield wiper that help wipe off some of the raindrops on the front-facing camera. Based on the table from the previous question, which of the following statements do you agree with?
**Answer: ** 2.2% would be a reasonable estimate of the maximum amount this windshield wiper could improve performance.

### 10. You decide to use data augmentation to address foggy images. You find 1,000 pictures of fog off the internet, and “add” them to clean images to synthesize foggy days, like this: Which of the following statements do you agree with?
**Answer: ** So long as the synthesized fog looks realistic to the human eye, you can be confident that the synthesized data is accurately capturing the distribution of real foggy images, since human vision is very accurate for the problem you’re solving.

### 11. So long as the synthesized fog looks realistic to the human eye, you can be confident that the synthesized data is accurately capturing the distribution of real foggy images, since human vision is very accurate for the problem you’re solving.
**Answer: ** 
* **You should also correct the incorrectly labeled data in the test set, so that the dev and test sets continue to come from the same distribution**
* **You should not correct incorrectly labeled data in the training set as well so as to avoid your training set now being even more different from your dev set.**

### 12. So far your algorithm only recognizes red and green traffic lights. One of your colleagues in the startup is starting to work on recognizing a yellow traffic light. (Some countries call it an orange light rather than a yellow light; we’ll use the US convention of calling it yellow.) Images containing yellow lights are quite rare, and she doesn’t have enough data to build a good model. She hopes you can help her out using transfer learning.
What do you tell your colleague?
**Answer: ** She should try using weights pre-trained on your dataset, and fine-tuning further with the yellow-light dataset.

### 13. Another colleague wants to use microphones placed outside the car to better hear if there’re other vehicles around you. For example, if there is a police vehicle behind you, you would be able to hear their siren. However, they don’t have much to train this audio system. How can you help?
**Answer: ** Neither transfer learning nor multi-task learning seems promising.

### 14. Between these two, Approach B is more of an end-to-end approach because it has distinct steps for the input end and the output end. True/False?
**Answer: ** false

### 15. Approach A (in the question above) tends to be more promising than approach B if you have a ________ (fill in the blank).
**Answer: ** Large training set

