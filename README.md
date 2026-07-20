# How Actually Git are used in Industry Level 

<h2>What is Git? </h2>
<p>Git is a vesrion control system. It tracks every change you make to your code. 
So you can go back to any previous at any time. </p>


<h2>How it look like while working with <strong>with Git or without Git </strong></h2>

# Without Git
+ main.py
+ +main_v2.py
+ main_final.py
+ main_final2.py
+ main_FINAL.PY

# With Git
main.py
+ full history of every changes 
+ who change what
+ when it was change
+ ability to go back to any version.

<h2>Step to Setup Process </h2>
<strong>Step1 :</strong> -- Install git 

#   Verify installation  -> git --version

#   Step2 : -- Configure global first
    - git config --global user.name "santosh chaudhary"
    - git config --global user.email "santosh@gmail.com

#    Verify global configuration 
    - git config --list 

#     Step3: -- Initailize git in your project / working directory
    - cd "project directory"
    - git init -> It creates empty repository in your local system. 
    - create .gitignore file in your project directory 

#    Step4 : -- Unerstand the three stages of git

# Working dir               Staging Area                    Repository
Where you write code        Files ready to be saved       Saves history permanately record  
git add . ------------------>
                            git commit -m "messge"------------->    

#    Step5 : -- Your First Commit:
        - check what files git sees
        - git status

#   Add all files to staging area
        - git add .             # it move all the project what sees in git in staging area  
        - git add filename      # but it move only specific file in staging area

#   Save with meaningful message
        - git commit -m "meaningful message"

<h1>Git Command and Daily Reference </h1>

#   CHECK----------------------------------------------
        - git status                    # What files changed 
        - git log                       # full commit history
        - git log --oneline             # compact commit history
        - git diff                      # What exactly changed in files

#   SAVE-----------------------------------------------
        - git add .                     # Add all files 
        - git add filename.py           # stage specific file
        - git commit -m "message"       # save to history

#   BRANCH---------------------------------------------
        - git branch                    # list branches 
        - git checkout -b name          # create and switch to a new branch 
        - git checkout main             # switch to main branch
        - git merge branch-name         # merge branch 

#   GIT HUB--------------------------------------------
        - git push origin main          # upload to github
        - git pull origin main / git clone         # download from github 
        - git clone url                 # download full repository. 


#   UNDO--------------------------------------------- 
        - git checkout filename       # undo changes in a file 
        - git reset HEAD1             # undo last commit

Note: Does not track empyt folder by git. 

 
