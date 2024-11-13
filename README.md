**Local Python Code Protector Script Documentation**

[![License](https://img.shields.io/badge/license-Custom-blue.svg)](LICENSE.md)
[![Python Version](https://img.shields.io/badge/python-3.6%2B-blue)](https://www.python.org/downloads/)
[![Code Protection](https://img.shields.io/badge/code-protection-green.svg)](README.md#main-functions-of-the-script)
[![Secure Code](https://img.shields.io/badge/secure-code-green.svg)](README.md#introduction)
[![Python Security](https://img.shields.io/badge/python-security-blue.svg)](README.md#recommendations-and-best-practices)
[![Code Obfuscation](https://img.shields.io/badge/code-obfuscation-blue.svg)](README.md#main-functions-of-the-script)
[![Secure Transfer](https://img.shields.io/badge/secure-transfer-blue.svg)](README.md#introduction)
[![Encryption](https://img.shields.io/badge/encryption-enabled-brightgreen.svg)](README.md#main-functions-of-the-script)

*Version: 1.2\
Author: Alpha Beta Network Research Team\
© 2024 αβ.net (alphabetanet.com) - Alpha Beta Network. All Rights
Reserved.*

------------------------------------------------------------------------

**Table of Contents**

- [1. Introduction](#1-introduction)
- [2. Installation](#2-installation)
  - [2.1 Installing Required Packages](#21-installing-required-packages)
- [3. Main Functions of the Script](#3-main-functions-of-the-script)
  - [3.1 Obfuscating Python Source Files](#31-obfuscating-python-source-files)
  - [3.2 Obfuscating Compiled Python Files](#32-obfuscating-compiled-python-files)
- [4. Detailed Description of Each Function](#4-detailed-description-of-each-function)
  - [4.1 Obfuscating Python Source Files](#41-obfuscating-python-source-files)
  - [4.2 Obfuscating Compiled Python Files](#42-obfuscating-compiled-python-files)
- [5. Additional Features](#5-additional-features)
  - [5.1 Restricting Code Execution to Specific Devices](#51-restricting-code-execution-to-specific-devices)
  - [5.2 Setting an Expiration Date](#52-setting-an-expiration-date)
  - [5.3 Adding Custom Messages](#53-adding-custom-messages)
- [6. Usage Examples](#6-usage-examples)
  - [6.1 Basic Obfuscation of a Source File](#61-basic-obfuscation-of-a-source-file)
  - [6.2 Obfuscation with Device Restrictions](#62-obfuscation-with-device-restrictions)
  - [6.3 Obfuscation with Expiration Date](#63-obfuscation-with-expiration-date)
  - [6.4 Obfuscation with All Features](#64-obfuscation-with-all-features)
- [7. Recommendations and Best Practices](#7-recommendations-and-best-practices)
- [Appendix A: Installation of Required Packages](#appendix-a-installation-of-required-packages)
- [Appendix B: Generating Hardware IDs](#appendix-b-generating-hardware-ids)
- [Appendix C: Contact Information](#appendix-c-contact-information)

------------------------------------------------------------------------

**Table of Contents**

-   1\. Introduction

-   2\. Installation

-   3\. Main Functions of the Script

    -   3.1 Obfuscating Python Source Files

    -   3.2 Obfuscating Compiled Python Files

-   4\. Detailed Description of Each Function

    -   4.1 Obfuscating Python Source Files

    -   4.2 Obfuscating Compiled Python Files

-   5\. Additional Features

    -   5.1 Restricting Code Execution to Specific Devices

    -   5.2 Setting an Expiration Date

    -   5.3 Adding Custom Messages

-   6\. Usage Examples

    -   6.1 Basic Obfuscation of a Source File

    -   6.2 Obfuscation with Device Restrictions

    -   6.3 Obfuscation with Expiration Date

    -   6.4 Obfuscation with All Features

-   7\. Recommendations and Best Practices

-   Appendix A: Installation of Required Packages

-   Appendix B: Generating Hardware IDs

-   Appendix C: Contact Information

------------------------------------------------------------------------

# 1. Introduction

The **Local Python Code Protector Script** is a command-line tool
designed to provide **source code protection** and **secure code
sharing** for Python scripts. It allows developers to obfuscate their
Python code, making it more difficult for others to understand or
reverse-engineer. This script supports both Python source files (.py)
and compiled Python files (.pyc), offering flexible options for code
obfuscation and encryption.

Key features of the script include:

-   **Code Obfuscation and Encryption**: Implements multi-level
    protection with dynamic encryption and obfuscation techniques.

-   **Device-Specific Restrictions**: Allows restricting code execution
    to specific devices based on hardware IDs.

-   **Expiration Date Settings**: Enables setting an expiration date
    after which the code will not run.

-   **Cross-Platform Compatibility**: Works on Windows, macOS,
    Linux/Unix, and other operating systems where Python 3.6+ is
    installed.

-   **No Internet Connection Required**: The protected code runs locally
    without needing an internet connection.

This tool is ideal for developers who need to protect their Python code
when sharing it with clients, colleagues, or deploying it on servers,
ensuring **Python code security best practices** are upheld.

------------------------------------------------------------------------

# 2. Installation

Before using the Local Python Code Protector Script, ensure that you
have **Python 3.6+** installed on your system.

**2.1 Installing Required Packages**

The script requires the following Python packages:

-   requests

-   psutil

-   cryptography

-   decompyle3

-   xdis

-   astor

You can install them using pip:

```bash

pip install requests psutil cryptography decompyle3 xdis astor
```
Ensure that you are using the correct version of pip associated with
your Python 3 installation. If you are using a virtual environment,
activate it before installing the packages.

------------------------------------------------------------------------

# 3. Main Functions of the Script

The Local Python Code Protector Script provides the following main
functionalities:

## 3.1 Obfuscating Python Source Files

Obfuscate and protect Python source files (.py) by applying multi-level
encryption and obfuscation techniques.

## 3.2 Obfuscating Compiled Python Files

Protect previously compiled Python files (.pyc) using a unique
recompilation technology that enhances their security.

------------------------------------------------------------------------

# 4. Detailed Description of Each Function

## 4.1 Obfuscating Python Source Files

The script can obfuscate Python source files, making them harder to read
and reverse-engineer.

**Command Syntax**

```bash

python local_python_code_protector.py -f FILE_PATH [OPTIONS]
```
**Description of Parameters**

-   -f FILE_PATH or \--file FILE_PATH: **(Required)** Specifies the path
    to the Python source file (.py) to protect.

-   -d DEVICES or \--device DEVICES: *(Optional)* A comma-separated list
    of hardware IDs (HWIDs) to restrict the code execution to specific
    devices.

-   -e DATE or \--expiration DATE: *(Optional)* Sets an expiration date
    in YYYY-MM-DD format, after which the code will not run.

-   -m MESSAGE or \--message MESSAGE: *(Optional)* A custom message to
    display when the protected code is executed.

## 4.2 Obfuscating Compiled Python Files

The script can obfuscate compiled Python files (.pyc) by converting them
back to a safe code representation and re-protecting them.

**Command Syntax**

```bash

python local_python_code_protector.py -f FILE_PATH [OPTIONS]
```
**Note:** The parameters are the same as for source files.

------------------------------------------------------------------------

# 5. Additional Features

## 5.1 Restricting Code Execution to Specific Devices

You can restrict the execution of the protected code to specific devices
by specifying their hardware IDs (HWIDs). Only devices with the listed
HWIDs will be able to run the code.

**Parameter**

-   -d DEVICES or \--device DEVICES: A comma-separated list of HWIDs.

**Example**

```bash

python local_python_code_protector.py -f my_script.py -d 123456789012345678,987654321098765432
```
## 5.2 Setting an Expiration Date

Set an expiration date for the protected code. After this date, the code
will refuse to run.

**Parameter**

-   -e DATE or \--expiration DATE: The expiration date
    in YYYY-MM-DD format.

**Example**

```bash

python local_python_code_protector.py -f my_script.py -e 2024-01-01
```
## 5.3 Adding Custom Messages

Add a custom message that will be displayed when the protected code is
executed. This could be a disclaimer or any pertinent information.

**Parameter**

-   -m MESSAGE or \--message MESSAGE: The custom message text.

**Example**

```bash

python local_python_code_protector.py -f my_script.py -m "This is a licensed instance #123456789012345678. Unauthorized use, reproduction, or distribution is prohibited."
```
------------------------------------------------------------------------

# 6. Usage Examples

## 6.1 Basic Obfuscation of a Source File

Obfuscate a Python source file without any additional restrictions.

**Command**

```bash

python local_python_code_protector.py -f my_script.py
```
**Output**

-   The protected file will be saved in the Local_Protected directory as
    a compiled .pyc file.

## 6.2 Obfuscation with Device Restrictions

Restrict the execution of the protected code to specific devices.

**Command**

```bash

python local_python_code_protector.py -f my_script.py -d 123456789012345678,987654321098765432
```
**Notes**

-   Replace the numbers with the actual HWIDs of the devices.

-   Only the devices with the specified HWIDs can execute the protected
    code.

## 6.3 Obfuscation with Expiration Date

Set an expiration date for the protected code.

**Command**

```bash

python local_python_code_protector.py -f my_script.py -e 2024-01-01
```
**Notes**

-   After January 1, 2024, the code will not run.

## 6.4 Obfuscation with All Features

Combine device restrictions, expiration date, and a custom message.

**Command**

```bash

python local_python_code_protector.py -f my_script.py -d 123456789012345678 -e 2024-01-01 -m "License valid until 2024-01-01."
```
**Notes**

-   The code will only run on the device with
    HWID 123456789012345678 and before January 1, 2024.

-   Upon execution, the message \"License valid until 2024-01-01.\" will
    be displayed.

------------------------------------------------------------------------

# 7. Recommendations and Best Practices

-   **Add Multiple Protection Layers**: To enhance security, you can
    obfuscate the already protected code again using the script.

-   **Use Latest Python Versions**: If possible, use the latest Python
    versions for which decompilers are not readily available.

-   **Utilize Virtual Environments**: Create virtual environments for
    different Python versions to generate protected versions compatible
    with various Python installations.

-   **Combine with Cloud Protection**: For more robust protection,
    consider using cloud-based solutions
    like secure_python_code_manager.py.

------------------------------------------------------------------------

# Appendix A: Installation of Required Packages

The local_python_code_protector.py script requires the following Python
packages:

-   **requests**

-   **psutil**

-   **cryptography**

-   **decompyle3**

-   **xdis**

-   **astor**

**Installing Packages with pip**

You can install these packages using the following command:

```bash

pip install requests psutil cryptography decompyle3 xdis astor
```
Ensure that you are using the correct version of pip associated with
your Python 3 installation. If you are working within a virtual
environment, activate it before installing the packages.

------------------------------------------------------------------------

# Appendix B: Generating Hardware IDs

To restrict code execution to specific devices, you need to obtain the
hardware IDs (HWIDs) of those devices. Use
the system_hardware_id_generator.py script to generate the HWID.

**Usage:**

1.  Run the script on the target device:

```bash

python system_hardware_id_generator.py
```
2.  The script will display the HWID:

```bash

Your Hardware ID (HWID) is: 123456789012345678
```
3.  Use this HWID with the -d or \--device parameter when obfuscating
    your code.

------------------------------------------------------------------------

# Appendix C: Contact Information

If you experience issues or have questions not covered in this
documentation, please contact the Alpha Beta Network Research Team.

-   **Website**: https://alphabetanet.com \| https://αβ.net

-   **Official Telegram Channel**: https://t.me/alphabetanetcom

------------------------------------------------------------------------

© 2024 αβ.net (alphabetanet.com) - **Alpha Beta Network**. All Rights
Reserved.
