# Cloning Laravel  Homestead Repository

Steps to Clone Laravel Homestead using Git on Windows:\


1. Create a directory/folder where you clone the Homestead repository. In my below example, I created `vm` a directory/folder.

<figure><img src="../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>

2. Open Git Bash or the command terminal and navigate to the directory where you want to install Homestead. Run the following command to clone the Homestead repository.

```bash
git clone https://github.com/laravel/homestead.git Homestead
```

<figure><img src="../.gitbook/assets/image (33).png" alt=""><figcaption><p>Run the following command to clone the Homestead repository.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption><p>Homestead repository successfully cloned.</p></figcaption></figure>

3. After cloning, Run the following command to change Homestead directory and to checkout the latest stable release of Homestead

```bash
cd Homestead
 
git checkout release

git branch
```

<figure><img src="../.gitbook/assets/image (27).png" alt=""><figcaption><p>Checkout the latest stable release of Homestead.</p></figcaption></figure>



That's it! You've successfully cloned Laravel Homestead on your Windows machine.

In the next topic, we will configure folder mapping to share your Laravel project folder between your host and guest machines.

