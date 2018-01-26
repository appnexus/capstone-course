# Git Tutorial

## Git, defined

> [Git](https://git-scm.com/) is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.
> \- _git-scm.com_

In more practical terms, git is a tool for working on software projects and lets you manage your work and the work of your partners more effectively over the life of your project.

## Concepts and Terms

* **Repository**: a project in git; like an application, a software library, or a course syllabus. Also referred to as a _repo_.
* **Branch**: A timeline of work in your repo. A repo consists of a _master_ branch and any number of branches off of that. Branches can be used to develop code in isolation of other branches. Since branches are recursive, you can branch off a branch (and then branch off of that branch, etc. etc.).
* **Commit**: an atomic amount of work that lives on a branch. Typically these are a collection of _diffs_, which are a list of the files or lines that have been added or subtracted from a file; for example, this correction of a list of items:
```
--- a/FAVORITE_THINGS.md
+++ b/FAVORITE_THINGS.md
A list of my favorite musical notes:
* DO
* RE
- * FA
+ * MI
```
* **Merge**: Combining two branches together. Let's say branch _A_ has a file called `Foo.java` and branch _B_ has a file called `Bar.java`. Merging branch _B_ into _A_ would result in branch _A_ having both `Foo.java` and `Bar.java`
* **Conflict**: When two branches cannot be merged without a correction. Typically, this requires you to identify which lines in a diff should go in the target branch. For example, if two people write different code for a function in separate branches, the person doing the merge would need to decide which lines to keep and which to get rid of:
```
--- a/example.js
+++ b/example.js
function print() {
    <<<<<<< HEAD:branch-a
    console.log('hello world!')
    =======
    console.log('goodbye world!')
    >>>>>>> 8f8588aa64:branch-b
}
```
* **Pull Request**: A formal way of declaring that you want to merge two branches, usually requiring the approval of your partners and/or some review. Pull requests are not a built-in feature of git, but different _implementations_ of git allow you to set up rules that are appropriate for your repo.

## Implementations of git

Git is "distributed" because your repos exist on your computer _and_ in the cloud, requiring you to sync repos between your local and your remote. One such provider of git is [Github](github.com), which will be used in this course. Other popular git include [Bitbucket](https://bitbucket.org/) and [GitLab](https://gitlab.com), and some organizations host their own git environments for securty or privacy's sake.

## Links to resources

### [Git Interactive Tutorial](https://try.github.io/levels/1/challenges/1)

### [Git Documentation](https://git-scm.com/documentation)

### [GitHub Patchwork](https://patchwork.github.io/curriculum/#resources)

### [Github Hello World](https://guides.github.com/activities/hello-world/)

### [Git Workflows Compared](https://www.atlassian.com/git/tutorials/comparing-workflows)