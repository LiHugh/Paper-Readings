# [On The Power of Curriculum Learning in Training Deep Networks](https://arxiv.org/pdf/1904.03626.pdf)
To employ curriculum learning, the training algorithm must resolve 2 problems: (i)
sort the training examples by difficulty; (ii) compute a series of mini-batches that exhibit an increasing level of difficulty. 

The author address these challenge by (i)using two methods: transfer learning from some competitive “teacher” network, and bootstrapping. (ii)investigating different pacing functions to guide the sampling.

The author deccompse CL into two separate -- but closely related -- sub-tasks and their corresponding functions.

## Scoring function
This determines the "difficulty" or "complexity" of each example in the data. The socring function makes it possible to sort the training examples by difficulty, the present to the network the easier example first. 

## Pacing function
This determines the pace by which data is presented to the network. The pace may depdend on both the data itself and the learner.


