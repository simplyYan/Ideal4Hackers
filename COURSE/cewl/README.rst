.. title:: A Comprehensive Guide to CeWL (Custom Word List Generator)

Introduction
============

CeWL, which stands for "Custom Word List Generator," is an open-source tool used to generate custom wordlists or dictionaries for password cracking, phishing, and security assessments. It is designed to crawl websites, extract text content, and create wordlists based on the words and phrases found within a target website or web application. In this guide, we will explore CeWL in detail, covering its features, installation, basic usage, and examples.

Features
========

CeWL offers several features, including:

1. **Website Crawling**: CeWL can crawl a specified website or web application, following links and gathering text content from web pages.

2. **Customizable Depth**: Users can set the depth of the crawl, specifying how many levels of links CeWL should follow.

3. **Wordlist Generation**: It generates wordlists based on the text content extracted from the crawled pages, including words, phrases, and character combinations.

4. **Customizable Output**: Users can customize the wordlist output format, including the minimum and maximum word length and the inclusion or exclusion of numbers, symbols, or special characters.

Installation
============

To use CeWL, you need to install it on your system. Here are the general steps for installation:

1. **Ruby Installation**:

   CeWL is written in Ruby, so ensure that you have Ruby installed on your system. You can download Ruby from the official website (https://www.ruby-lang.org/en/documentation/installation/) or use a package manager specific to your operating system.

2. **CeWL Installation**:

   You can install CeWL using RubyGems, a package manager for Ruby:

   ```bash
   gem install cewl
   ```

Basic Usage
===========

CeWL is simple to use and comes with a straightforward command structure. Here is the basic command to use CeWL:

```plaintext
cewl <options> <target_url> -w <output_wordlist_file>
```

- `<options>`: Specify any desired options or flags.
- `<target_url>`: Provide the URL of the website or web application to crawl.
- `-w <output_wordlist_file>`: Specify the output wordlist file to which the generated words will be saved.

Examples
========

Example 1: Generating a Wordlist from a Website
------------------------------------------------

To generate a wordlist from a website, use the following command:

```bash
cewl http://example.com -w my_wordlist.txt
```

- `http://example.com`: Replace with the URL of the website you want to crawl.
- `my_wordlist.txt`: Replace with the desired output wordlist file name.

CeWL will crawl the website and generate a wordlist based on the text content found.

Example 2: Customizing Wordlist Output
----------------------------------------

You can customize the wordlist output by specifying options such as minimum and maximum word length, inclusion or exclusion of numbers, and more. For example:

```bash
cewl http://example.com -w custom_wordlist.txt -m 4 -M 12 -d 1 -o
```

- `-m 4`: Set the minimum word length to 4 characters.
- `-M 12`: Set the maximum word length to 12 characters.
- `-d 1`: Limit the wordlist to alphanumeric characters only.
- `-o`: Include words with special characters.

CeWL will create a custom wordlist according to your specified options.

Conclusion
==========

CeWL is a valuable tool for generating custom wordlists for password cracking, phishing, and security assessments. When using CeWL, always ensure that you have proper authorization to crawl and extract content from websites, as unauthorized use may have legal and ethical consequences.

This guide has provided an overview of CeWL, including installation, basic usage, and practical examples. Explore its capabilities to create wordlists tailored to your specific needs.