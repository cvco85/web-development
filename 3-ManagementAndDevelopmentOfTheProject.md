# Management and development of the project

There are a lot of things we can talk about management and developing a project, however, I've chosen X to talk about.

## Methodology

Nowadays, most of the companies work with Agile methodologies. (Write topic on agile).

However, almost all software management methods follow some guidelines:

- Requirements (business and product related)
Deals with the business objectives and tries to define what the "product owner" wants to achieve with the selected product or feature

- Change management (more technical, including software developers)
Match between product and tech. Trying to have time previsions about when features are going to be launched. Negotiation to get the better features for the available time span.

- Software development 

- Release management
Multiple releases to various environments during the whole software development process. Quality assurance, user acceptance tests.

### Agile

The term "agile" in software development is used to describe processes that tend to be faster, recurring to a lot of iterations and making incremental changes in a product, delivering working software with frequency and keeping business people in touch with developers.

There are a lot of different methodologies inside agile, however, **Scrum** is one of the most used ones.

The [Agile Manifesto](http://agilemanifesto.org/) defines some principles about this methodology:

- Individuals and interactions over processes and tools
- Working software over comprehensive documentation
- Customer collaboration over contract negotiation
- Responding to change over following a plan

[More detail](http://agilemanifesto.org/principles.html)

### How SCRUM works

**Sprint** - a time box with a clearly defined set of objectives. A period where working software should be delivered. After a sprint ending, another one starts. Tend to have period from 1 to 3 weeks to enable fast reaction and multiple iterations.

**Sprint planning** - Happens once per sprint, it's a meeting where people from business and developers compromise themselves and estimate the time needed to accomplish tasks. Can be a small feature, a improvement, a set of bugs. Mainly about time estimation and work management. 

**Daily SCRUM** - Daily meeting where people from the same team keep in sync with each other, define what's blocking them and what they (or someone should do) to unblock the work. Simplifying, it's a daily sync.

**Sprint review** - Meeting to gather feedback and ideas about how was the sprint, define the room for improvements, and what could be done to optimize value. Checks if sprint goals were met and answers possible questions.

**Sprint retrospective** - Define and note what gone well during the sprint, what could be improved, talk about the next sprint in a more informal way. Define action points to improve the process in the next sprint.

## Progress tracking

There are a lot of software used to keep track of what's being done during the software development process. The majority of them are integrated with the VCSs.

- Jira
- Trello
- Asana
- ...

There are a lot of project management tools. An example of a feature development process could be.

1. Business owners decide the bigger company goals
2. Product managers together with the business owners decide what should the team do to accomplish those goals.
3. Product managers together with managers define a feature's roadmap.
4. The roadmap is estimated, giving a not very precise timespan for the features to be done.
5. In a "sprint based", roadmap's features are estimated and given to developers in small parts so everything is trackable and achievable.
6. Product managers test and define new iterations for the features done.
7. Back to step 5.

## Version control

Nowadays, is non-sense to develop software without some kind of Version Control System (VCS), and it is a critical skill to any developer. 

A VCS is a software that keeps track of changes made to files (normally code). Enables the team keep track of what's being done, as well as to work in a collaborative way, having people working either in different things that end up together or in different areas of the same feature.

There are different types of VCS:

- Local

![local][LocalVCS]

- Centralized

![local][CentralizedVCS]

- Distributed

![local][DistributedVCS]

[LocalVCS]: https://git-scm.com/book/en/v2/images/local.png
[CentralizedVCS]: https://git-scm.com/book/en/v2/images/centralized.png
[DistributedVCS]: https://git-scm.com/book/en/v2/images/distributed.png

The most known and used VCS is [*git*](https://git-scm.com).

### git

[What is git?](https://git-scm.com/about)

**Branches**
Are like "different" copies of the same code in different times. Branches are independent from each other.

- They allow *Frictionless Context Switching* - Change between branches without any problem, keep different states, try new things without being concerned about loosing what you've done.

- Ease of deployment process - Easy to keep different states and separate what's in production from what's in dev, per example.

- Separate features per branches - Allows to have different contexts, completely independent features can work in parallel. Also allows to have "sub-features" developed by different people and then merged.

- Allow experimentation - Can easily create local branches, try new things, share them with teammates, and delete at any time without any problem.

**Speed**
Git is fast, does almost all operations using local processing power. Was created to handle linux kernel, so it is done from the beginning to keep a lot of files.

![Git vs SVN][gitVsSVN]

[gitVsSVN]: https://chart.googleapis.com/chart?chxt=x&cht=bvs&chl=git|svn&chd=t:1.53,24.7&chds=0,24.7&chs=100x125&chco=E09FA0|E05F49&chf=bg,s,fcfcfa&chtt=Commit%20B

**Distributed**

- Multiple backups - Each instance (user) of git is a backup of the server. If there are a lot of people working in a repository, each one of them have a "copy" of the whole repository, keeping it *distributed*.

- Any workflow - Because of the strong git branching model, teams are able to adjust and to find the workflow that suits them better.

**Data assurance**

Git assures *the cryptographic integrity of every bit of your project*. Every file and commit is checksummed and it grants what you put there is what you get. Every commit has an ID, granting that if you change anything in a commit, even if you *overwrite* you will end up with a different id, so, the old state and the new state are never taken as the same.

**Staging area**

In git, the *staging area* is like an intermediate step between you sending for the centralized repository and having it in your local system. Allows you to organize your files and commits, stage some parts and leave others to better group your changes.

**Open source**

Git is free, open source, this means that it's always being developed and improved, and of course also means you don't need to pay anything to use it. You can even *fork* it and create your own git version.

