Project Management Options

We would like to have a set of tools to help us coordinate our work with each other and with stakeholders. 
We have identified some options. There is a collection of tools that work well with GitHub and provide elements 
we would like to have.

ZenHub    -   This is a scrum friendly tool that combines with the normal GitHub issues system to 
              allow higher level management of work items. It supports the typical agile process workflows
              using a backlog and a column pipeline for easy visual assessment of status. It also provides
              a burndown chart integrated with the GitHub milestones feature.
              
Review Ninja  This integrates code review support with the GitHub pull request mechanism, so that team members
              can review and approve pull requests and then merge approved pulls. It integrates with Slack, our
              preferred high bandwidth collaboration tool so that we get notifications as needed.
              

Both of these require that the GitHub organization that owns the repo authorize the use of the tool. So there
are two obvious ways that we can use these tools. One is to ask an administrator (owner) of Humanify repository
to activate the tools. The other is for us to use a repository that we own and control for daily churn, and then 
to push updates from our repository to the Humanify repository. 

Humanify GitHub
Pros             All copies of the source remain either on your GitHub account or on our development machines.
                 As a practical matter there isn't much difference between a local repo on our development 
                 machines and a private repo on GitHub managed by us, but there more be more issues than just
                 practical considerations.
                 
                 Humanify can use it for other project work.
                 
Cons             Humanify would have to either restrict usage of the tool to certain people, or pay the per user
                 price for each organization member. That is $5 per user per month, minimum 5 users. Review Ninja
                 is free at the moment.
                 
Separate GitHub  
Pros             I (Dennis) will manage and pay for the hosting and the integration apps as needed, and will
                 not have to impose any burden on the Humanify resources.
                 
                 Simpler status in "master" repository. We are going to be using the "GitFlow" git 
                 management policy, so we would push from the separate "working" repository to the Humanify 
                 "master" repository only when we have successful integration of feature branches. That means that 
                 every commit to the master is working code.
                 
Cons             The hour by hour sequence is not captured in the Humanify repo. Changes would appear there less frequently,
                 typically about once or twice per day (we try to keep tickets that small). 
                 
                 Whatever issues anyone at Humanify might have with the github repo. Key people at Humanify (DJ at minimum)
                 would have ownership rights to the repo, so that Humanify could delete the repo at any time should the 
                 project end suddenly and unexpectedly. The repo would be deleted at the normal end of the project. Still,
                 meanwhile there would be a repo in use that is not part of Humanify.
                 

If neither of the above two options is satisfactory, we can use a standalone board system such as trello. That would be 
useful, though it would require team members to either track tasks in two places (trello and github) or else not have the 
work fully tracked in github.

