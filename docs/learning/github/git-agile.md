Besides the benefits of flexibility and distribution, there are key functions of Git that support and enhance agile development. Think of Git as a component of agile development; changes can get pushed down the deployment pipeline faster than working with monolithic releases and centralized version control systems. Git works the way your agile team works (and should strive to work).

#####PRO TIP:
> Git is Distributed Version Control System (DVCS). Unlike CVS or Subversion (SVN) repositories, Git allows developers to create their own, personal copy of the team's repository, hosted alongside the main codebase. These copies are called forks and when work is complete on a fork, it's easy to bring changes back to the main codebase.

###Tip 1: Start thinking about tasks as Git branches
Git comes into play after features have been fleshed out, added to a product roadmap, and the development team is ready. But to take a step back here is a quick crash course in agile feature development: product, design, quality assurance (QA), and engineering hold a feature kick-off meeting to come up with a shared understanding of what a feature will be (think requirements), scope of the project, and what tasks that the feature needs to be broken down into to complete it. These tasks – are also known as user stories – are then assigned to individual developers.

Git starts fitting into your agile workflow at this point. At Atlassian, we create a new branch for every single issue. Whether it's a new feature, a bug fix, or a small improvement to some existing code, every code change gets its own branch.

Branching is straightforwards and allows teams to easily collaborate inside one central codebase. When a developer create a branch, they effectively have their own isolated version of the codebase in which to make changes. For an agile team this means that by breaking features into user stories and then branches, the development team has the ability to tackle tasks individually and work more efficiently on the same code but in different repositories; there is no doubling up of work and since individuals are able to focus on small chunks of work in repositories separate from the main repository there are not as many dependencies slowing down the development process.  