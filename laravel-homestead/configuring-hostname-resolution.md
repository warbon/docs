# Configuring Hostname Resolution

In order to access the websites running on Homestead, you need to add the IP address and site names to your computer's host file. This file is used by your operating system to map domain names to IP addresses. In this guide, we will walk through the steps to add the IP address and site names from Homestead.yaml to the Windows host file.

Steps to Configuring Host file in Windows environment:

1. Open Homestead repository in VS Code and select Homestead.yaml file.

<figure><img src="../.gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>

2. We will add the IP address and site name from Homestead.yaml to the Windows host file.

<figure><img src="../.gitbook/assets/image (9) (3).png" alt=""><figcaption></figcaption></figure>

3. Run command terminal as Administrator.

<figure><img src="../.gitbook/assets/image (13).png" alt=""><figcaption></figcaption></figure>

4. Navigate to the Windows host file: In the Command Prompt, navigate to the directory where the Windows host file is located by typing the following command:

```bash
cd C:\Windows\System32\drivers\etc
```

<figure><img src="../.gitbook/assets/image (1) (1).png" alt=""><figcaption></figcaption></figure>

5. Open the Windows host file with Notepad: Type the following command to open the Windows host file in Notepad:

```powershell
notepad hosts
```

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption><p>Type the following command to open the Windows host file in Notepad</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>

6. Copy the IP address: Open the Homestead.yaml file in a text editor and copy the IP address for your Homestead virtual machine.

<figure><img src="../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>

7. Add the IP address and site names to the Windows host file: In the Notepad window, add a new line at the bottom of the file and paste the IP address you copied earlier. Then, add the site names you want to map to that IP address. For example, if you have a site named "homestead.test" in your Homestead.yaml file, add this line:

```
192.168.56.56 homestead.test
```

<figure><img src="../.gitbook/assets/image (2) (1).png" alt=""><figcaption></figcaption></figure>

8. Save the changes and exit Notepad: Save the changes you made to the Windows host file and exit Notepad.

That's it! You have successfully added the IP address and site name to Windows host file. In the next topic, we will launch the Laravel Homestead box using the Vagrant command and create a Laravel project to test the hostname resolution.
