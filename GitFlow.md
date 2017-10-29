---
    title:Git Workflow
    tags:none
    notebook:none
---


# Git Workflow

![none](https://raw.githubusercontent.com/thunderup012/Git-Flow/1ba12b569f9d0824befb72d75346f4dc38618c31/gitflow/1.png)

- **Definition**

 **GitHub Flow** is a lightweight, branch-based workflow that supports teams and projects where deployments are made regularly.

---
## Three classifications of **Git Workflow**

- Git Flow
- Github Flow
- Gitlab Flow

**Common** 

Feature-driven development(abbr. *FDD*),
 a model-driven short-iteration process that consists of five basic activities 

 - Develop overall model
 - Build feature list
 - Plan by feature
 - Design by feature
 - Build by feature



 ---


## Git Flow
- first developed
- widely adopted

![none](https://raw.githubusercontent.com/thunderup012/Git-Flow/1ba12b569f9d0824befb72d75346f4dc38618c31/gitflow/2.png)

### Two Features



- Long Term Branch
- Short Term Branch

#### Long Term Branch
- master, used to store the released version
- develop, used to do day-to-day development

#### Short Term Branch
- feature branch
- hotfix branch
- release branch

Once developed, they are merged into *develop*  or *master* and then deleted.

### Evaluation

- clear
- controllable
- a little complicated, two long-term branches need to be maintained simultaneously


-----
## Github Flow
Simplified version of **Git Flow**(used in Github.com)

![none](https://raw.githubusercontent.com/thunderup012/Git-Flow/1ba12b569f9d0824befb72d75346f4dc38618c31/gitflow/3.png)

### Feature

- only one long term branch----*master*

### Steps
- create a branch
- open a pull request
- discuss any review
- merge and deploy

### Evaluation
- easy to use
- good for continuous releasing

### Shortage

If the code needs to be reviewed and some new code is committed during the review process, there will be some difference with the code on the *master* branch.

-----

## Gitlab Flow 
Combination of **Git Flow** and **Github Flow**(recommended in Gitlab.com)

![none](https://raw.githubusercontent.com/thunderup012/Git-Flow/1ba12b569f9d0824befb72d75346f4dc38618c31/gitflow/4.png)

### The most Important Principle ----- **Upstream First Policy**

There is only one master branch *master*, which is the upstream of all the other branches. Only if the changes of the code are adopted by the upstream branch, these changes can be applied to the other branches.


### Version Release

For the 'release' project, it is recommend that each stable version should be pulled from the *master* branch.

![none](https://raw.githubusercontent.com/thunderup012/Git-Flow/1ba12b569f9d0824befb72d75346f4dc38618c31/gitflow/5.png)

------

# Thanks!




 