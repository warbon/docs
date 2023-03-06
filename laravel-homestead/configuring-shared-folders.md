# Configuring Shared Folders

Steps to Configuring Shared Folders in Laravel Homestead:

1. Run `init.bat` command from the Homestead directory to create the <mark style="color:red;">Homestead.yaml</mark> configuration file.

```bash
init.bat
```

<figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption><p>Run <code>init.bat</code> command from the Homestead directory.</p></figcaption></figure>

2. Run `init.bat` command from the Homestead directory to open the repository in VS Code.

```powershell
C:\vm\Homestead>code .
```

3. Select Homestead.yaml file to display configuration.

<figure><img src="../.gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>

4. Update the <mark style="color:blue;">`folders:`</mark> configuration with the below configuration:

````yaml
```
folders:
    - map: /code
      to: /home/vagrant/code
      type: "nfs"
```
````

5. Create a directory/folder mapping to share your Laravel project/code between your host and Homestead guest machine. In this example, I mapped the `C:\code` folder to the `/home/vagrant/code` folder in the Homestead virtual machine.

<figure><img src="../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>

6. Save the changes to the `Homestead.yaml` file and exit.
7. You need to install the vagrant-winnfsd plugin for <mark style="color:blue;">`type`</mark>`:`` `<mark style="color:orange;">`"nfs"`</mark> configuration by running the following command in your terminal:

```powershell
vagrant plugin install vagrant-winnfsd
```

<figure><img src="../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

8. This required restarting the computer after the installation.



That's it! You have successfully configured shared folders in Laravel Homestead on a Windows machine.
