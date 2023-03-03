---
description: Installing Git version control system
---

# Git

Git is a version control system used for tracking changes in files and coordinating work on those files among multiple people. It allows users to make and save changes to files while keeping a history of all changes made, making it easy to track changes, roll back to earlier versions, and collaborate with others on a project. Git is widely used in software development and is typically used in conjunction with a hosting service, such as GitHub or GitLab.

### Installation

1. Download Git from the official website for your operating system. You can find the downloads at https://git-scm.com/downloads.

<figure><img src=".gitbook/assets/02.png" alt=""><figcaption></figcaption></figure>

2. Run the installer and follow the prompts to install Git. You can choose the default options for most settings, but you may want to customize the installation location or choose a different text editor if you prefer.
3. Once Git is installed, open a terminal or command prompt and type `git --version` to confirm that it is installed correctly. You should see the version number of Git printed in the terminal.

```shell
// git --version
git --version
git version 2.38.1.windows.1
```

4. Next, you'll want to configure Git with your name and email address. Type the following commands in the terminal, replacing "Your Name" and "[youremail@example.com](mailto:youremail@example.com)" with your own name and email address:

```bash
// git config
git config --global user.name "Your Name"
git config --global user.email youremail@example.com

```

5. That's it! You're now ready to start using Git. You can create a new repository with the `git init` command, or clone an existing repository with `git clone <repository URL>`. For more information on how to use Git, check out the official documentation at [https://git-scm.com/docs](https://git-scm.com/docs).
