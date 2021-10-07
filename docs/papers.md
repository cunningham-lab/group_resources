---
layout: default
---

<script src='https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.5/latest.js?config=TeX-MML-AM_CHTML' async></script>

<div class="topnav">
  <a href="../group_resources/">Home</a>
  <a class="active" href="#">Papers</a>
  <a href="code">Docs</a>
  <a href="soft_skills">Soft Skills</a>
  <a href="meeting_notes">Meeting Notes</a>
</div>

Here are papers that are of interest to our group. If adding new papers, please do so in the following format:  

```
- Author List, "Title", Journal (Year). [link](url)
  - Comments 
```

For example:  

```
- Benton, Gregory W., et al. "Loss Surface Simplexes for Mode Connecting Volumes and Fast Ensembling." arXiv preprint arXiv:2102.13042 (2021). [link](https://arxiv.org/abs/2102.13042)
  - A cool paper that reduces the computational cost of ensembling by exploiting unexpected structure in the loss landscape. 
```

In this case I just copied the MLA formatted Google Scholar `Cite` text, and added a link afterwards.    

- Benton, Gregory W., et al. "Loss Surface Simplexes for Mode Connecting Volumes and Fast Ensembling." arXiv preprint arXiv:2102.13042 (2021). [link](https://arxiv.org/abs/2102.13042)
  - A cool paper that reduces the computational cost of ensembling by exploiting unexpected structure in the loss landscape. 

## Contrastive Learning (Presentation 10/7)

- Chen, Ting, et al. "Big self-supervised models are strong semi-supervised learners." arXiv preprint arXiv:2006.10029 (2020). [link](https://arxiv.org/abs/2006.10029)
  - This paper describes the design of SimCLR version 2- they describe a protocol wherein a big model can be trained with contrastive losses, fine-tuned, and then distilled into a smaller model. 
- He, Kaiming, et al. "Momentum contrast for unsupervised visual representation learning." Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition. 2020. [link](https://arxiv.org/abs/1911.05722)
  - The paper for the MoCo algorithm - uses a memory cache to hold additional negative examples without generating inordinate batch sizes. 
- Ngiam, Jiquan, et al. "Domain adaptive transfer learning with specialist models." arXiv preprint arXiv:1811.07056 (2018). [link](https://arxiv.org/abs/1811.07056)
  - More pretraining data does not always help! The authors propose a method that evaluates data usefulness during pretraining with importance weights. 
- Raghu, Maithra, et al. "Transfusion: Understanding transfer learning for medical imaging." arXiv preprint arXiv:1902.07208 (2019). [link](https://arxiv.org/abs/1902.07208)
  - Pretraining does not always help with medical imaging data. Sometimes you're better off with a small model, and for a large model even just normalizing the weights to the right magnitude can make a huge difference. 
- Azizi, Shekoofeh, et al. "Big self-supervised models advance medical image classification." arXiv preprint arXiv:2101.05224 (2021). [link](https://arxiv.org/abs/2101.05224)
  - Hierarchical pretraining for medical imaging data. Introduces Multi-Instance Contrastive Learning for SOTA classification performance. 
- Reed, Colorado J., et al. "Self-Supervised Pretraining Improves Self-Supervised Pretraining." arXiv preprint arXiv:2103.12718 (2021). [link](https://arxiv.org/abs/2103.12718)
  - Hierarchical pretraining across 16 different datasets, with thorough experimentation with training strategies. 
- Chen, Xinlei, et al. "Improved baselines with momentum contrastive learning." arXiv preprint arXiv:2003.04297 (2020). [link](https://arxiv.org/pdf/2003.04297.pdf)
  - MoCo v2 paper, showing improved performance against SimCLRv1  baselines.   
- Wang, Tongzhou, and Phillip Isola. "Understanding contrastive representation learning through alignment and uniformity on the hypersphere." International Conference on Machine Learning. PMLR, 2020. [link](http://proceedings.mlr.press/v119/wang20k.html) 
  - How do features learned through contrastive losses differ from those learned with standardized supervised features? Is there a general principle of representation learning we can extract there? 
- Azizi, Shekoofeh, et al. "Big self-supervised models advance medical image classification." arXiv preprint arXiv:2101.05224 (2021). [link](https://arxiv.org/abs/2101.05224)  
   
   
    

