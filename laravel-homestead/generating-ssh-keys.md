# Generating SSH Keys

SSH (Secure Shell) is a secure network protocol used to remotely access and manage network devices securely. SSH keys are a pair of cryptographic keys (a public key and a private key) that can be used to authenticate with remote servers or services, without the need for a password. Homestead is a development environment that allows developers to create virtual machines for web development. The homestead.yaml file is a configuration file for Homestead, which contains settings for virtual machines and their corresponding software configurations.

Here are the steps to generate SSH keys in Windows terminal and add it to the homestead.yaml file:

1. Open Windows terminal, and type the following command to generate the SSH key pair:

```bash
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

Here, "[your\_email@example.com](mailto:your\_email@example.com)" is the email address associated with your SSH key.

2. Save the SSH keys. The terminal will prompt you to enter a file name to save the keys. You can leave the default file name by pressing enter, or you can enter a custom name. Next, the terminal will prompt you to enter a passphrase to encrypt the private key. You can enter a passphrase or leave it blank for no passphrase.

<figure><img src="../.gitbook/assets/image (9) (4).png" alt=""><figcaption></figcaption></figure>

3. Add SSH keys to the homestead.yaml file Open the homestead.yaml file, which is usually located in the Homestead directory. And homestead added it by default.

<figure><img src="../.gitbook/assets/image (1) (4).png" alt=""><figcaption></figcaption></figure>

That's it! You have now generated SSH keys in Windows terminal and added it to the homestead.yaml file.

In the next topic, we will add the IP address and the domain to the host file to our Windows environment.
