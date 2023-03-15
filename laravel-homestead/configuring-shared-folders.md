# Configuring Shared Folders

Steps to Configuring Shared Folders in Laravel Homestead:

1. Run `init.bat` command from the Homestead directory to create the <mark style="color:red;">Homestead.yaml</mark> configuration file.

```bash
init.bat
```

<figure><img src="../.gitbook/assets/image (5) (2).png" alt=""><figcaption><p>Run <code>init.bat</code> command from the Homestead directory.</p></figcaption></figure>

2. Run `code .` command from the Homestead directory to open the repository in VS Code.

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

6. Update the <mark style="color:blue;">`sites:`</mark> configuration, by adding your project name.

```yaml

sites:
    - map: acware.test
      to: /home/vagrant/code/{projectname}/public 
      
```

In this example, we named the project mylaravelapp which will be discussed in detail in [Creating a Laravel project in Homestead. ](creating-a-laravel-project-in-homestead..md)

<figure><img src="../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

6. Your Homestead.yaml configuration will look like this:

```yaml
---
ip: "192.168.56.56"
memory: 2048
cpus: 2
provider: virtualbox

authorize: ~/.ssh/id_rsa.pub

keys:
    - ~/.ssh/id_rsa

folders:
    - map: /code
      to: /home/vagrant/code
      type: "nfs"

sites:
    - map: acware.test
      to: /home/vagrant/code/mylaravelapp/public 
    

databases:
    - acw

features:
    - mysql: true
    - mariadb: false
    - postgresql: false
    - ohmyzsh: false
    - webdriver: false

services:
    - enabled:
          - "mysql"
#    - disabled:
#        - "postgresql@11-main"

#ports:
#    - send: 33060 # MySQL/MariaDB
#      to: 3306
#    - send: 4040
#      to: 4040
#    - send: 54320 # PostgreSQL
#      to: 5432
#    - send: 8025 # Mailhog
#      to: 8025
#    - send: 9600
#      to: 9600
#    - send: 27017
#      to: 27017

```

6. Save the changes to the `Homestead.yaml` file and exit.
7. You need to install the vagrant-winnfsd plugin for <mark style="color:blue;">`type`</mark>`:`` `<mark style="color:orange;">`"nfs"`</mark> configuration by running the following command in your terminal:

```powershell
vagrant plugin install vagrant-winnfsd
```

<figure><img src="../.gitbook/assets/image (35).png" alt=""><figcaption></figcaption></figure>

8. This required restarting the computer after the installation.



That's it! You have successfully configured shared folders in Laravel Homestead on a Windows machine.

In the next topic, we will generate SSH Keys. SSH keys are a pair of cryptographic keys (a public key and a private key) that can be used to authenticate with remote servers or services, without the need for a password.

