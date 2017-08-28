# EEOB/BCB 546X Unix Git Exercise

This exercise will take you through the process of using Git and Unix. For this, you will first create a GitHub account. Once you have done that, you will 'fork' this repository to your account. Then you can clone your version of the repository to the class cluster (or your own machine) and then follow the Unix tasks on the cluster. Once you have completed the Unix part of the exercise, you will push the changes to your repository.

## Get a GitHub User Account

First, you must make a user account on GitHub if you don't have one already. Be sure to choose a user ID that you are happy using for the rest of your professional career as a bioinformatician. GitHub is a very important tool for computational biology and if you continue working in data-intensive fields, you will be using this account again in the future. Join GitHub here:
[https://github.com/join](https://github.com/join).


## Git Exercise Part 1

### Fork the Repository

Now that you have your own GitHub account you can fork [this](https://github.com/EEOB-BioData/Unix-Git-Exercise) repository by clicking the **_Fork_** button at the upper right corner of the repository page.

<img src="https://help.github.com/assets/images/help/repository/fork_button.jpg">

This will take you to the GitHub page for your very own GitHub repository! It should have the URL (where `<your GitHub ID>` should be your new GitHub ID):

```
https://github.com/<your GitHub ID>/Unix-Git-Exercise
```

### Clone Your Repository on the HPC-Class Cluster

Now log on to the HPC-class cluster (replace `<ISU NetID>` with your ISU NetID):

```
ssh <ISU NetID>@hpc-class.its.iastate.edu
```

Once you have logged on to the cluster, clone your forked repository to your home directory (replace `<your GitHub ID>` with your GitHub ID):

```
git clone https://github.com/<your GitHub ID>/Unix-Git-Exercise
```

Now change to the `Unix-Git-Exercise` directory and follow the Unix exercise steps in the next section.

```
cd Unix-Git-Exercise
```

## Unix Exercise

## Git Exercise Part 2

Now that you have completed all of the Unix tasks and you are more familiar with the Unix environment, push your changes and new files to your version of the exercise repository.

First you will have to stage all of your changes by _add_ing them:

```
git add .
```

Now that the files are staged, commit them to your local repository and include a commit message (note that you do not have to use the same commit message `completed the unix exercise` and you can choose something else that you feel is descriptive and informative, just be sure to keep the `""`):

```
git commit -m "completed the unix exercise"
```

With the changes committed to your local repository, you can now push them to your remote host on GitHub:

```
git push
```

Git! Git! Hooray!