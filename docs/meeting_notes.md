---
layout: default
---

<script src='https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.5/latest.js?config=TeX-MML-AM_CHTML' async></script>
<div class="topnav">
  <a href="../group_resources/">Home</a>
  <a href="papers">Papers</a>
  <a href="code">Code</a>
  <a href="soft_skills">Soft Skills</a>
  <a class="active" href="#">Meeting Notes</a>
</div>

Notes for our group meetings. 

# Meeting 9/30/21 

Here are the results for our survey on group meeting format: 

- Would you like to have group meetings? 
    - 6/6 responded yes
- If yes, how often would you like to have group meetings: 
    - 4/6 weekly 
    - 2/6 biweekly
- Interesting topics for discussion? 
    - Fun scientific ideas in general
    - Research topics
        - Statistical Machine Learning
            - New model architectures
                - Transformer architectures
                - Off-the-shelf WGAN
                - Efficient Ensembling
            - Learning paradigms 
                - Continual learning
                - Contrastive learning
            - Understanding/improving generalization
                - Out of Distribution detection
                - Generalization in deep models
                - Reliable deep learning
                - Understanding the loss landscape
        - Neuroscience applications  
            - Null hypothesis tests for learning in biological processes 
            - Steve Scott group papers on feedback dynamics
            - Neuro Latents Benchmarks
    - Skills topics
        - Templates: 
            - Code template
            - Paper template
            - Response to reviewer template
        - Software:
            - Gpytorch 
            - Spark
            - NeuroCAAS (Thanks!)
            - Cloud usage 
            - Team Git
        - Simulations: 
            - Let's say you want to start building a new tool. What are the steps you take in the first week?
            - Let's say you want to start a new project. How do you structure paper reading, writing, etc? 
            - Coding challenges
            - Pair programming sessions
        - Coding Best Practices 
            - CI/CD 
            - Test Driven Development
            - Joel Gru Anti-Notebook talk 
        - Soft skills  
            - Team management
- Presenters/Facilitator Per Meeting 
    - 6/6 yes
    - 3/6 Pairs
    - 2/6 Don't Care
    - 1/6 Individual
- Soft Meetings
    - 5/6 Yes 
    - 1/6 Maybe 
- Field Trip Suggestions     
    - Camping 
    - National Part Visit 
    - Laser Tag
    - Picnic
    - Fun
    - Field trips to parks
    - End of Semester events (Lunches?)
- What's one thing you want out of group meeting by the end of the year?      
    - Building a strong, supportive research community: 
        - Be more connected with lab members.   
        - Understand the research expertise of others and build positive institutional psychology 
        - Positive feedback loop of zeal
        - Motivation to publish
    - Learning how to be more effective researchers from each other:  
        - Understand other learning/working styles
        - Gain new knowledge from the literature 
        - Gain new coding skills


## Summary of Survey

- Strong mandate to have group meetings. 
    - Main objectives: 
        - build a strong and supportive community  
        - learning how to be more effective researchers. 
        - Suggestion: If we agree on these goals, let's be proactive in making sure that they happen. If some part of the format is not working, we should discuss.  
- Meeting format: 
    - Healthy support for weekly meetings.  
    - Lots of interest in skills (coding, soft skills like management) that are less common for our research settings. It's worth devoting some time to figuring out the best format for this kind of meeting.   
        - Suggestion: Approach this through simulations in addition to traditional presentations. Introduce a problem, give everyone time to think on their own, and then compare answers.  
    - Research topics are mostly statistical machine learning, with some neuroscience topics as well.  
    - Suggestion: Let's make a schedule of topics (research and skills) that covers the semester, and people can opt in to whatever topic they want (as individuals, as pairs). We can also plan field trips here!  



## Post-meeting summary

- Soft skills

  - Time / project / paper management skills (could be an app, methodologies)
  - Coding skills (IDE, Jupyter Notebook)

- Self-assessment 

  - IDP https://myidp.sciencecareers.org/?AspxAutoDetectCookieSupport=1

- Next week's plan

  - Taiga and Luhuan will present on contrastive learning

# Meeting 10/7/21    

Today Luhuan and Taiga presented an overview of contrastive learning, with some applications to pretraining for real datasets. 
There were lots of interesting discussion points, summarized in what follows: 

- A key difference between the MoCo and SimCLR frameworks is that MoCo has “two” networks: a query network, whose representations will be learned via gradient descent, and a key network, which has its parameters updated as a convex combination of its current parameters, and the query network’s new parameters. This is the “momentum” aspect of the momentum update. In contrast, SimCLR only has one network, and draws samples from it without concern for keys vs. queries. Although the momentum component, nonlinear projection head, and other features of both frameworks have been intermingled in successive papers, I don’t think this difference has ever been resolved. 
- It’s hard to understand why a lot of these implementation details work. Consider, for example the MLP projection head used by SimCLR. How should we understand the value of this projection head in improving the encoded representations? Dan mentioned an analogy with VAEs/Vanilla AutoEncoders. One perspective on VAEs is that it encourages latent representations to group together through a prior distribution- is something like that happening implicitly here?  
- Is it a good idea to do contrastive learning in datasets where you have some structure? (I.e. video). 
- How is contrastive learning more than just a fancy wrapper for data augmentation? What is the value of doing it beyond doing the same data augmentations in a supervised setting? 
- The whole point of ML is to learn functions of the data that we don’t know how to describe mathematically. This philosophy is clear in doing classification. Is it as clear here? If we’re doing instance contrastive learning, aren’t we just creating data representations that are invariant to the particular data augmentations that we choose? Writing down invariant representations seems like something that we could just do mathematically instead. What is the value of learning these invariant representations w.r.t. a given data distribution? Uniformity of the representations in your learned feature space? 

# Meeting 10/14/21
 
Happy Hour!

# Meeting 10/28/21

Today we're going over the results of Geoff's self assessment survey: [link](https://docs.google.com/forms/d/17U6Iiz2l3WRnam-Ufrt1dY_RORAZX2fAOTCbTv7Mt_Y/edit#re)

There are a wide spread of results. We can ignore the topics where everyone has a good understanding, but it would be very interesting to spend time on those places where a sizeable portion of the group has self evaluated as needing to improve.  

For those topics on which a significant part of the group would like to improve, we could consider different formats: 
- Traditional presentation with slides on a certain tool, method, etc. 
- "Panel discussion" going over bigger picture stuff that is less defined.    
- Brainstorming session to tackle particular issues. 

Summary of Results: 

What the most common things that people want to develop further? 

## 5/7 
- Starting a new project 
- Starting a new piece of software
- Balancing multiple projects 
- Efficiently reading papers  
- Keeping an organized notebook 
 
## 4/7 
- Assessing/identifying opportunities or areas for improvement to acheive goals more effectivelyo
- Motivating and/or mentoring others to accomplish goals
- Writing rebuttals that actually improve reviews
- Collaboratively writing software/code with others
 
## 3/7 
- Using software development best practices (test driven design, continuous integration, etc.)
- Explaining complex or theoretical concepts/ideas in basic terms and language
- Choosing an appropriate set of experiments for a paper
- Designing effective figures and tables
- Writing thoughtful, polite, and thorough reviews (and reviewing papers efficiently)
- Performing a thorough literature search, ranging from seminal works to hot-off-the-press
- Prioritizing tasks while maintaining flexibility to address potential/unexpected problems
 
