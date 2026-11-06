# Git Fundamentals and Branching Strategies

Imagine, you are a devops engg and working on production application.

- one engineer changed nginx config
- another engineer updated the deployment script.

That is why Git.

Version Control?

- A system that records the changes made to the files over time, allows the developers to compare version, restrore previous versions and collaborate.

helloworld.cpp
helloworld_v2.cpp
helloworld_final.cpp
helloworld_fixed.cpp

with Git:

Helloworld.cpp
    |
    |--------> commit 1: Inital Development
    |
    |--------> commit 2: Add logs
    |
    |--------> commit 3: fix presentation
    |


Git                                     Github
Version control software                Git repo hosting platform
Runs locally                            Hosts the repo's onlinee
Works without internet                  Sharing requires internet
Creates commits and branches            Provides Pull Requests, Reviews, CI/CD integration


Where Git fits in Devops:

                                                    Developer changes the code
                                                                |
                                                    Git repo - Push changes
                                                                |
                                                    CI/CD pipeline - build and test
                                                                |
                                                    Deploy to staging/ production

# Git Architecture 


        Working Directory           Staging area                Local Repository
            Edit files           Selecting the changes               Save Commits
                    ---------------->          --------------------->
                         git add                       git commit
                                        |
                                    git push
                                        |
                                    Remote Repo (Gitlab or Github)                    


# Branching and Merging

A prod website is working fine but you want to add there new diwali banner.

We will create a seperate branch.

Branch ---- Movable pointer to a sequence of commit, allowing to isolate the dev work.


----------------------------------------------------------------
main            |                              | merge
                |------------------------------|
                Diwalibanner

Diwali Offer : 30% off.


A prod website is working fine but you want to add there new diwali banner.

We will create a seperate branch.

Branch ---- Movable pointer to a sequence of commit, allowing to isolate the dev work.


----------------------------------------------------------------
main            |                              | merge
                |------------------------------|
                Diwalibanner

Diwali Offer : 20% off.