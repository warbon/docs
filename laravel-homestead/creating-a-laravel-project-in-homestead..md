# Creating a Laravel project in Homestead.

In this topic we will create a basic laravel project to test our newly configured Laravel Homestead development environment.

To start launch the Homestead Virtual Machine which was discussed in detail in our previous topic [Launching the Homestead Virtual Machine](launching-the-homestead-virtual-machine.md).

Once the Homestead virtual machine is up and running, you can connect to it using SSH.

1. Open Windows Terminal, and navigate to the `Homestead` directory.

```bash
cd /vm/Homestead
```

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

2. In the terminal or command prompt, run the following command:

```bash
vagrant ssh
```

This command will connect you to the Homestead virtual machine.

<figure><img src="../.gitbook/assets/image (13).png" alt=""><figcaption></figcaption></figure>

3. Run the following command to navigate to <mark style="color:blue;">`code`</mark> directory:

```bash
cd code
```

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

4. Then, run the following command to create a new Laravel project:

```bash
composer create-project --prefer-dist laravel/laravel mylaravelapp
```

The project name `mylaravelapp` is the project name we set in our previous topic [Configuring Shared Folders.](configuring-shared-folders.md)

<figure><img src="../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

5. Please wait, this will install the dependencies for the new project.

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

Below shows that you have successfully a new laravel project.

<figure><img src="../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

Run the following command to navigate to the project directory:

```bash
cd mylaravelapp
```

<figure><img src="../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

6. You can also directly check the project in the code directory we created in the previous topic [Configuring Shared Folders](configuring-shared-folders.md).

<figure><img src="../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

7. The application is now accessible to the hostname we configured in the [Configuring Hostname Resolution](configuring-hostname-resolution.md) topic.&#x20;

{% embed url="http://homestead.test/" %}

<figure><img src="../.gitbook/assets/image (2) (1).png" alt=""><figcaption></figcaption></figure>

8. Your project will now open to your default browser.

<figure><img src="../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

8. You can now open your project in the VS Code and start coding.

<figure><img src="../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

That's it! You have successfully created a Laravel project in Homestead and launched it on your local machine. You can now start developing your Laravel application using the Homestead virtual environment.

You can check to [Laravel](https://laravel.com/) site for the detail of the documentation.

In the next topic, we will create a Laravel API project and test the API on [Postman](https://www.postman.com/).
