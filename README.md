# Mutual information for fine-grained analysis of neural networks

## Abstract
With the rise of neural networks, there has been a focus shift from
feature design to architecture design. Recent research suggests to automate neural architecture search (NAS) using search methods like
Bayesian Optimization, Reinforcement learning or evolutionary algorithms. Given a data set, these methods are applied to search for a
(local) maximum on the function that maps the architectures to an accuracy on the data set. Some of these searches have already delivered
architectures, that compete with state-of-the art human-generated ones.

However, the above-mentioned methods are generally expensive. This
also comes from the fact that they evaluate neural networks at the granularity of the whole network: Evaluating a network by a metric like
accuracy doesn’t inform about how well individual parts of the network perform and what parts need to be changed.

In previous research, neural networks have already been analyzed using mutual information. Because the mutual information measures
arbitrary dependencies between random variables, it is suitable for assessing the “information content” of the layers in complex classification
tasks. However, in this work we will show that mutual information per
se is not sufficient for neural architecture search tasks - at least not
when estimated with MINEs, a current state of the art method.

The above finding is shown in two experiments. In the first experiment,
we try to predict a distribution over good architectures on a data set
given an architecture and its MI on the data set. In the second experiment, we try to predict good sampling distributions for Hyperbands,
given an architecture and its MI on the data set the sampled architectures should perform well on. In both experiments, a neural network
predictor leveraging the MI was not able to compete with simple base
lines. We suggest that this is due to mutual information not being
expressive enough for such complex tasks


## Background
I did this project as my Bachelor thesis in 2019 with Andreas Krause. For more details on method and results, please refer to the [report](report.pdf).

For code and correspondence, please reach me via the following email:

![Alt text](https://hmorcg.db.files.1drv.com/y4m7hoqm11M2LgHMoSkPBZMcsCdblmlxls_kyZMBzGSMwIX-QE8As8HDGejSuvRCHYF_hsXf1uEt02kzujHiJ0vj9e-V4cmQbjaP0mvyXo2AphueGlPnLafAQs_ZeLw4VM--2YRw2UZzntEJTvbtlGYIFpqnhKKFsPAGG5ZQ1X8-Ca0k_qzMFJLLA7b1xM3-Wo1A2tAqC8upPSkGsgz7pcd9w?width=149&height=23&cropmode=none)

