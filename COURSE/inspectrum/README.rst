.. title:: A Comprehensive Guide to Inspectrum

Introduction
============

Inspectrum is an open-source tool used for analyzing and visualizing digital signals, particularly those from Software-Defined Radio (SDR) receivers. It is a valuable tool for examining radio frequency (RF) and other digital signals, making it useful for tasks such as signal decoding, modulation analysis, and reverse engineering. In this guide, we will explore Inspectrum in detail, covering its features, installation, basic usage, and examples.

Features
========

Inspectrum offers several features, including:

1. **Signal Visualization**: Inspectrum provides a graphical interface for visualizing digital signals, enabling users to view the amplitude and frequency characteristics of captured signals.

2. **Signal Analysis**: Users can analyze and demodulate various types of digital signals, including amplitude-shift keying (ASK), frequency-shift keying (FSK), and phase-shift keying (PSK).

3. **Export and Import**: Inspectrum allows users to export captured signals in various formats, such as CSV or complex baseband, and import signals for analysis.

4. **Cursor Measurement**: It provides tools for measuring signal characteristics using cursors, allowing users to determine signal properties such as frequency, symbol rate, and phase.

Installation
============

To use Inspectrum, you need to install it on your system. Here are the general steps for installation:

1. **Installation via Package Manager**:

   Inspectrum may be available in the repositories of some Linux distributions. You can use your distribution's package manager to install it. For example, on Debian-based systems like Ubuntu, you can use the following command:

   ```bash
   sudo apt-get install inspectrum
   ```

2. **Building from Source**:

   Alternatively, you can build Inspectrum from source by cloning the official GitHub repository (https://github.com/miek/inspectrum) and following the build instructions provided in the repository's README file.

Basic Usage
===========

Inspectrum has a user-friendly graphical interface. Here are the basic steps to use Inspectrum:

1. **Launch Inspectrum**:

   After installation, launch Inspectrum from your system's applications menu or by executing `inspectrum` in the terminal.

2. **Load a Signal**:

   Open a captured signal file by selecting "File" > "Open" from the menu. Supported file formats include I/Q samples, complex baseband, and more.

3. **Visualize and Analyze**:

   Once the signal is loaded, you can use the tools provided by Inspectrum to visualize the signal, set cursors for measurements, and analyze its characteristics.

Examples
========

Example 1: Analyzing an FSK Signal
-----------------------------------

Suppose you have captured an FSK (Frequency-Shift Keying) signal using an SDR receiver. You can use Inspectrum to analyze the signal's frequency shifts and decode the digital information.

1. Load the captured signal into Inspectrum.

2. Use cursors to measure the frequency difference between signal shifts, which corresponds to the FSK modulation.

3. Analyze the signal's bit pattern and decode the digital data based on the frequency shifts.

Example 2: Exporting Signal Data
---------------------------------

You can export signal data for further analysis or processing in other tools. To export signal data from Inspectrum:

1. Load the signal.

2. Select "File" > "Export" from the menu.

3. Choose the desired export format (e.g., CSV) and specify export options.

4. Save the exported data to a file.

Conclusion
==========

Inspectrum is a valuable tool for analyzing and visualizing digital signals, particularly those captured using SDR receivers. It is useful for decoding and understanding various modulation schemes and digital signal formats.

This guide has provided an overview of Inspectrum, including installation, basic usage, and practical examples. Explore its capabilities to analyze and work with digital signals effectively.