.. title:: A Comprehensive Guide to Reaver

Introduction
============

Reaver is an open-source command-line tool designed for cracking WPS (Wi-Fi Protected Setup) enabled wireless routers' PINs and recovering the WPA/WPA2 pre-shared keys. It is commonly used by security professionals and penetration testers to assess the security of Wi-Fi networks that have WPS enabled. In this guide, we will explore Reaver in detail, covering its features, installation, basic usage, and examples.

Features
========

Reaver offers several features, including:

1. **WPS PIN Cracking**: Reaver specializes in cracking WPS PINs, which are used to authenticate devices to a Wi-Fi network. Once the PIN is cracked, the WPA/WPA2 pre-shared key can be obtained.

2. **Automatic Mode**: Reaver can run in an automatic mode where it continuously attempts to crack the WPS PIN without requiring manual intervention.

3. **Customization**: Users can customize attack parameters, such as the target router's BSSID (MAC address), interface to use, and more.

4. **Rate Limiting**: Reaver includes rate limiting functionality to avoid lockout or detection by the target router.

Installation
============

To use Reaver, you need to install it on your system. Here are the general steps for installation:

1. **Download and Install Reaver**:

   - Reaver is available for Linux distributions and can typically be installed using the package manager specific to your distribution.

   - For example, on Debian-based systems like Ubuntu, you can install Reaver using the following command:

     ```bash
     sudo apt-get install reaver
     ```

   - On other distributions, you may need to download the source code from the official Reaver GitHub repository and compile it manually.

Basic Usage
===========

Reaver has a straightforward command-line syntax. Here is the basic command to use Reaver:

```plaintext
reaver -i <interface> -b <BSSID> -c <channel> -vv
```

- `-i <interface>`: Specify the wireless network interface to use for the attack.

- `-b <BSSID>`: Provide the BSSID (MAC address) of the target router.

- `-c <channel>`: Specify the channel on which the target router operates.

- `-vv`: Enable verbose output for detailed progress and information.

Examples
========

Example 1: Running Reaver in Automatic Mode
--------------------------------------------

To run Reaver in automatic mode to crack the WPS PIN of a target router with the BSSID `00:11:22:33:44:55` on channel `6`, use the following command:

```bash
reaver -i wlan0 -b 00:11:22:33:44:55 -c 6 -vv
```

Reaver will attempt to crack the WPS PIN automatically and display progress and results.

Example 2: Customizing Reaver Parameters
----------------------------------------

You can customize Reaver parameters as needed. For instance, to set a delay between PIN attempts to avoid rate limiting and use a different wireless interface (`wlan1`), you can use the following command:

```bash
reaver -i wlan1 -b 00:11:22:33:44:55 -c 6 -d 10 -vv
```

- `-d 10`: Set a delay of 10 seconds between PIN attempts.

Conclusion
==========

Reaver is a valuable tool for assessing the security of Wi-Fi networks that have WPS enabled. When using Reaver for penetration testing or security assessments, it's essential to have proper authorization to perform the tests and ensure compliance with legal and ethical standards.

This guide has provided an overview of Reaver, including installation, basic usage, and practical examples. Explore its capabilities to assess the security of WPS-enabled Wi-Fi networks and take appropriate measures to enhance network security.