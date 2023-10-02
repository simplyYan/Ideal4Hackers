.. title:: A Comprehensive Guide to Medusa

Introduction
============

Medusa is an open-source command-line password cracking tool designed for conducting brute force attacks and dictionary attacks against various network protocols and services. It is a versatile and powerful tool used by security professionals, ethical hackers, and penetration testers to assess the strength of passwords and identify weak authentication mechanisms. In this guide, we will explore Medusa in detail, covering its features, installation, basic usage, and examples.

Features
========

Medusa offers a wide range of features, including:

1. **Protocol Support**: Medusa supports multiple network protocols and services, such as SSH, FTP, Telnet, HTTP, RDP, SMB, and more.

2. **Parallel and Distributed Attack**: It can perform parallel and distributed attacks, enabling faster and more efficient password cracking.

3. **Flexible Syntax**: Medusa provides a flexible command-line syntax that allows users to customize attack parameters, including target host, port, username, password list, and attack type.

4. **Brute Force and Dictionary Attacks**: Medusa supports both brute force attacks and dictionary-based attacks, making it adaptable for different scenarios.

5. **Session Management**: It allows for session resumption, ensuring that progress is not lost in case of a connection failure.

Installation
============

To use Medusa, you need to install it on your system. Here are the general steps for installation:

1. **Install Dependencies**:

   Depending on your operating system, you may need to install dependencies like OpenSSL and libssh2. Use the package manager specific to your system to install these dependencies.

2. **Download and Compile Medusa**:

   You can download the latest version of Medusa from the official website (http://foofus.net/goons/jmk/medusa/medusa.html) or clone the GitHub repository:

   ```bash
   git clone https://github.com/jmk-foofus/medusa.git
   ```

3. **Compile Medusa**:

   Navigate to the Medusa directory and compile it using the following commands:

   ```bash
   cd medusa
   ./configure
   make
   sudo make install
   ```

Basic Usage
===========

Medusa has a flexible and straightforward command-line syntax. Here is the basic command structure:

```plaintext
medusa -h <target> -U <user-list> -P <password-list> -M <protocol> -m <attack-type> -v 6
```

- `-h <target>`: The target host or IP address.
- `-U <user-list>`: The path to a file containing a list of usernames to test.
- `-P <password-list>`: The path to a file containing a list of passwords to test.
- `-M <protocol>`: The protocol or service to attack (e.g., ssh, ftp, http).
- `-m <attack-type>`: The attack type (e.g., brute, dictionary).
- `-v 6`: Set the verbosity level to 6 (for detailed output).

Examples
========

Example 1: Performing an SSH Brute Force Attack
------------------------------------------------

To perform a brute force attack against an SSH server:

```bash
medusa -h target_ip -U users.txt -P passwords.txt -M ssh -m HYDRA -v 6
```

- `target_ip`: Replace with the IP address or hostname of the SSH server.
- `users.txt`: Replace with the path to a file containing a list of usernames.
- `passwords.txt`: Replace with the path to a file containing a list of passwords.
- `ssh`: Specify the SSH protocol.
- `HYDRA`: Specify the brute force attack type.
- `-v 6`: Set the verbosity level to 6 for detailed output.

Medusa will attempt to log in to the SSH server using the provided username and password combinations.

Example 2: Performing an FTP Dictionary Attack
------------------------------------------------

To perform a dictionary attack against an FTP server:

```bash
medusa -h target_ip -U users.txt -P passwords.txt -M ftp -m DICT -v 6
```

- `target_ip`: Replace with the IP address or hostname of the FTP server.
- `users.txt`: Replace with the path to a file containing a list of usernames.
- `passwords.txt`: Replace with the path to a file containing a list of passwords.
- `ftp`: Specify the FTP protocol.
- `DICT`: Specify the dictionary attack type.
- `-v 6`: Set the verbosity level to 6 for detailed output.

Medusa will attempt to log in to the FTP server using username and password combinations from the dictionary.

Conclusion
==========

Medusa is a powerful and versatile password-cracking tool used for assessing the security of network services and protocols. When using Medusa, always ensure that you have proper authorization to perform password cracking, as unauthorized use may have legal and ethical consequences.

This guide has provided an overview of Medusa, including installation, basic usage, and practical examples. Continue