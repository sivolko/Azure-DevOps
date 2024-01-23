---
layout:
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: false
  pagination:
    visible: true
---

# 🌟 GIT & GITHUB

Git is a distributed version control system developed by Linus Torvald

GitHub is a cloud platform that uses Git as its core technology. GitHub simplifies the process of collaborating on projects and provides a website, more command-line tools, and overall flow that developers and users can use to work together. GitHub act s as the remote repository.

<mark style="color:purple;">**GitHub Key Features:**</mark>

* Issues
* Discussions
* Pull requests
* Notifications
* Labels
* Actions
* Forks
* Projects

<img src="../../.gitbook/assets/file.excalidraw (5).svg" alt="" class="gitbook-drawing">

### Git Terminology&#x20;

<details>

<summary><mark style="color:purple;"><strong>Working Tree</strong></mark></summary>

The set of nested directories and files that contain the project that's being worked on

</details>

<details>

<summary><mark style="color:purple;"><strong>Repository (Repo)</strong></mark></summary>

The directory, located at the top level of a working tree, where Git keeps all the history and metadata for a project. Repositories are almost always referred to as _repos_. A _bare repository_ is one that isn't part of a working tree; it's used for sharing or backup. A bare repo is usually a directory with a name that ends in _.git_—for example, _project.git_.

</details>

<details>

<summary><mark style="color:purple;">Hash</mark></summary>

A number produced by a hash function that represents the contents of a file or another object as a fixed number of digits. Git uses hashes that are 160 bits long. One advantage to using hashes is that Git can tell whether a file has changed by hashing its contents and comparing the result to the previous hash. If the file time-and-date stamp is changed, but the file hash isn’t changed, Git knows the file contents aren’t changed

</details>

<details>

<summary><mark style="color:purple;"><strong>Object</strong></mark></summary>

A Git repo contains four types of _objects,_ each uniquely identified by an SHA-1 hash. A _blob_ object contains an ordinary file. A _tree_ object represents a directory; it contains names, hashes, and permissions. A _commit_ object represents a specific version of the working tree. A _tag_ is a name attached to a commit

</details>

<details>

<summary><mark style="color:purple;"><strong>Commit</strong></mark></summary>

When used as a verb, _commit_ means to make a commit object. This action takes its name from commits to a database. It means you are committing the changes you have made so that others can eventually see them, too.

</details>

<details>

<summary><mark style="color:purple;"><strong>Branch</strong></mark></summary>

A branch is a named series of linked commits. The most recent commit on a branch is called the _head_. The default branch, which is created when you initialize a repository, is called `main`, often named `master` in Git. The head of the current branch is named `HEAD`. Branches are an incredibly useful feature of Git because they allow developers to work independently (or together) in branches and later merge their changes into the default branch.

</details>

<details>

<summary><mark style="color:purple;"><strong>Remote</strong></mark></summary>

A remote is a named reference to another Git repository. When you create a repo, Git creates a remote named `origin` that is the default remote for push and pull operations.

</details>
