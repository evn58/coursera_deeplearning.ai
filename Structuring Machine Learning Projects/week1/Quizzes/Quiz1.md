### 1. Note: Having three evaluation metrics makes it harder for you to quickly choose between two different algorithms, and will slow down the speed with which your team can iterate. True/False?
**True**

### 2. If you had the three following models, which one would you choose?
**Test Accuracy 98%	Runtime	9 sec Memory  9MB**

### 3. Based on the city’s requests, which of the following would you say is true?
**Accuracy is an optimizing metric; running time and memory size are a satisficing metrics.**

### 4. Before implementing your algorithm, you need to split your data into train/dev/test sets. Which of these do you think is the best choice?
**Train	9,500,000 Dev 250,000 Test 250,000**

### 5. You should not add the citizens’ data to the training set, because this will cause the training and dev/test set distributions to become different, thus hurting dev and test set performance. True/False?
**False**

### 6. One member of the City Council knows a little about machine learning, and thinks you should add the 1,000,000 citizens’ data images to the test set. You object because:
* **This would cause the dev and test set distributions to become different. This is a bad idea because you’re not aiming where you want to hit.**
* **The test set no longer reflects the distribution of data (security cameras) you most care about.**

### 7. This suggests that one good avenue for improving performance is to train a bigger network so as to drive down the 4.0% training error. Do you agree?
**No, because there is insufficient information to tell.**

### 8. You ask a few people to label the dataset so as to find out what is human-level performance. You find the following levels of accuracy:
**0.3% (accuracy of expert #1)**

### 9. Which of the following statements do you agree with?
**A learning algorithm’s performance can be better human-level performance but it can never be better than Bayes error.**

### 10.Based on the evidence you have, which two of the following four options seem the most promising to try? (Check two options.)
* **Train a bigger model to try to do better on the training set.**
* **Try decreasing regularization.**

### 11. What does this mean? (Check the two best options.)
* ** You have overfit to the dev set.**
* **You should try to get a bigger dev set.**

### 12. What can you conclude? (Check all that apply.)
* **It is now harder to measure avoidable bias, thus progress will be slower going forward.**
* **If the test set is big enough for the 0.05% error estimate to be accurate, this implies Bayes error is ≤0.05**

### 13. It turns out Peacetopia has hired one of your competitors to build a system as well. Your system and your competitor both deliver systems with about the same running time and memory size. However, your system has higher accuracy! However, when Peacetopia tries out your and your competitor’s systems, they conclude they actually like your competitor’s system better, because even though you have higher overall accuracy, you have more false negatives (failing to raise an alarm when a bird is in the air). What should you do?
**Rethink the appropriate metric for this task, and ask your team to tune to the new metric.**

### 14. You’ve handily beaten your competitor, and your system is now deployed in Peacetopia and is protecting the citizens from birds! But over the last few months, a new species of bird has been slowly migrating into the area, so the performance of your system slowly degrades because your data is being tested on a new type of data.
**Use the data you have to define a new evaluation metric (using a new dev/test set) taking into account the new species, and use that to drive further progress for your team.**

### 15. The City Council thinks that having more Cats in the city would help scare off birds. They are so happy with your work on the Bird detector that they also hire you to build a Cat detector. (Wow Cat detectors are just incredibly useful aren’t they.) Because of years of working on Cat detectors, you have such a huge dataset of 100,000,000 cat images that training on this data takes about two weeks. Which of the statements do you agree with? (Check all that agree.)
* **If 100,000,000 examples is enough to build a good enough Cat detector, you might be better of training with just 10,000,000 examples to gain a ≈10x improvement in how quickly you can run experiments, even if each model performs a bit worse because it’s trained on less data.**
* **Buying faster computers could speed up your teams’ iteration speed and thus your team’s productivity.**
* **Needing two weeks to train will limit the speed at which you can iterate.**