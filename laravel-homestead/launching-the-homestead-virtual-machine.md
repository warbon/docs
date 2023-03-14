# Launching the Homestead Virtual Machine

Now, let's proceed to launch the Vagrant box with Homestead.yaml file:

1. To launch the Homestead virtual machine for the first time or if you have  made any changes to the Homestead.yaml file. Run the command,`vagrant up`` `<mark style="color:red;">`--provision`</mark>. And if you have not made any changes to the Homestead.yaml file. Run command `vagrant up`.&#x20;

```powershell
// Run command if you made changes to Homestead.yaml file
vagrant up --provision
```

```
// Run command if no changes made to Homestead.yaml file
vagrant up --provision
```

2. Open command terminal and change directory to homestead directory. Always run vagrant command inside the homestead directory.

```
vagrant up --provision
```

<figure><img src="../.gitbook/assets/image (11).png" alt=""><figcaption><p>Always run vagrant command inside the homestead directory</p></figcaption></figure>

3. During the first launch, Vagrant will download the necessary resources, which may take a while depending on the speed of your internet connection.

<figure><img src="../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>

4. To access the Vagrant box via SSH, run the following command:

```bash
vagrant ssh
```

This will open a SSH connection to the Vagrant box, allowing you to run commands and interact with the environment.

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

5. Open Oracle VM VirtualBox Manager and you will see the `homestead` virtual machine running.

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

That's it! You have successfully launched the Vagrant box with Laravel Homestead using either the `vagrant up` or `vagrant up --provision` command, depending on whether or not you needed to re-provision the box.

In the next topic, let's try to create a Laravel project in Homestead virtual machine and to test the hostname resolution.
