# TextRank
In this assignment, you will be modifying or expanding on the [provided code](https://colab.research.google.com/drive/1uDudirBsq0bQ4d4EmZAwX1N4yMsvmZc7) for TextRank in order to perform better key-phrase extraction or extractive text summarization. You should include the results of tests over at least one dataset.

All your work should be in the Colab notebook. Make sure to leave comments throughout. You may interweave your code and write-up as you see fit/find convenient. If you have concerns or questions, reach out to me on Slack. I am happy to look at your code to provide feedback.

## Datasets
A number of datasets for [key-phrase extraction](https://github.com/LIAAD/KeywordExtractor-Datasets) and [extractive text summarization](https://github.com/mathsyouth/awesome-text-summarization#corpus) are available to freely download. Some datasets may take more processing than others, so you may want to take a look at several before you choose one. The pages linked above are a suggestion only - you may use other datasets not listed there if you wish.

## Assignment
For this assignment, you will be modified the provided TextRank code to perform one of the two tasks described in [the paper]((https://web.eecs.umich.edu/~mihalcea/papers/mihalcea.emnlp04.pdf). Note that the provided implementation does not match the paper’s experiments exactly.

### Steps
- Select a dataset
- Select a baseline model
- Make your own modifications to improve your chosen task.  
	Consider the following avenues of exploration:
	- How should you preprocess the data to select `text units` and relations?
	- How should you construct the TextRank graph?
	- How should you post process the output of TextRank to perform your chosen task. (This is the only step that is absolutely necessary)
- Select an evaluation metric. You should refer to the TextRank paper to decide which metric to use.
- Compare your modified model to the baseline model
- Identify and evaluate variants of your system that may provide a better result
	- Are there alternative methods to select `text units`?
	- Are there alternative methods to identify relations between `text units`?
	- How many of the results should you use?
	- Not every tweak will result in an improvement
- Present your results in your notebook.
### Variant
A variant is a small modification on your existing system. Any magic number or value in your code is a candidate for modification. Ultimately, your goal is to get a better result on the task. Any modification you can make to do this is worth trying out.

When implementing variants, make sure you can simultaneously run all your variants and the original system at the end of your notebook - ie, don’t overwrite functions.

## Grading criteria

### 8 ⭐️ - the number of stars required for an A.

> I will keep track of stars accumulated from assignments instead of some arbitrary percentages. I may offer more stars than are necessary for an A. Anything labelled with a ⚠️ is a hard requirement that I will not make up for with extra credit/bonuses.
- ⚠️ Your code should be well commented and any references you use should be listed in comments. If you forget to keep track of the references, try your best to list them at the bottom.
- ⚠️ Your assignment is submitted within a week of the deadline
- ⭐️⭐️ A working implementation of your chosen task
- ⭐️  An appropriately selected dataset, baseline, and metric to compare your implementation against
- ⭐️⭐️ Clearly presented results comparing your model against the baseline
- ⭐️⭐️ Proposed variants on your task (at least 3) with their evaluation. Your variants do not need to outperform your system or the baseline to be counted.
- ⭐️ Your assignment was completed on time.

### Extra credit
You may implement both tasks for an additional 8 ⭐️. If your second task is after the deadline, it will only be worth a maximum of 4 ⭐️. You may wish to commit a separate notebook for the second task.
