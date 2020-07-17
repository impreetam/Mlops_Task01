# Task-01
Merge Git Branches using Jenkins

This task will show you how to merge Git branches using Jenkins Jobs. This task contains three jobs , jobs description is given below :-

» JOB 1:-
If developer push to dev branch then Jenkins will fetch from dev and deploy on dev-docker environment.

» JOB 2 :-
If developer push to master branch then Jenkins will fetch from master and deploy on master-docker environment. Both dev-docker and master-docker environment are on different docker containers.

» JOB 3 :-
Manually the QA team will check (test) for the website running in dev-docker environment. If it is running fine then Jenkins will merge the dev branch to master branch and will trigger #JOB 2.

› SOLUTION FOR THE ABOVE TASKS:
• JOB 1(Dev Branch) ~
For this job i have created a code using dev branch and then pushed it on GitHub repository. Then I fetch this code through Jenkins and used GitHub plugin.
code for execute shellconsole output

• JOB 2 (Master branch)~
In this job program files which was put on GitHub . Then file will fetch by the Jenkins. This job will trigger after the JOB 1.
Triggered after job 1code for execute shellconsole output

• JOB 3 (Merge both of the branches -Dev and Master branch)~
In this job , job 1 and job 2 will merge. Hence , integration of Git branches (Dev and Master) will done using Jenkins.
triggered after job 2console outputHere Job 2 is triggered after Job 1 and Job 3 is triggered by Job 2.
