---
description: Feel free to use local system setup or else use sandbox.
layout:
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: false
  pagination:
    visible: true
---

# 💻 Hands-on-Labs

{% hint style="info" %}
Microsoft Sandbox Env&#x20;

[https://learn.microsoft.com/en-us/training/modules/intro-to-git/2-exercise-configure-git](https://learn.microsoft.com/en-us/training/modules/intro-to-git/2-exercise-configure-git)
{% endhint %}

{% code title="To check Git installed version " %}
```bash
git --version 

or 

git -v 
```
{% endcode %}

{% code title="Set your user name " %}
```bash
git config --global user.name "<USER_NAME>"
```
{% endcode %}

{% code title="set your email " %}
```bash
git config --global user.email "<USER_EMAIL>"
```
{% endcode %}

```bash
git config --list
```

```bash
git --help 
```

```bash
git status
```

```bash
git add 
```

```bash
git commit 
```

<details>

<summary>MS Learn Path </summary>

[https://learn.microsoft.com/en-us/training/paths/intro-to-vc-git/](https://learn.microsoft.com/en-us/training/paths/intro-to-vc-git/)

</details>

<details>

<summary><mark style="color:purple;"><strong>New Repository</strong></mark></summary>

{% code lineNumbers="true" %}
```bash
git init 
git branch -M main 
git remote add origin "<your url of repository>"
git add .
git commit -m "commit message here"
git push -u origin main 
```
{% endcode %}

</details>

<details>

<summary><mark style="color:purple;"><strong>Existing Repository</strong></mark> </summary>

{% code lineNumbers="true" %}
```bash
git remote add origin <your repository url>
git branch -M main 
git push -u origin main 
// to rebase run below command 
git pull --rebase origin main 
```
{% endcode %}

</details>

