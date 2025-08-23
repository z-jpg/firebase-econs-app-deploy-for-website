<div align="center"><h2>Notice: We are working full time work on <a href="https://github.com/coreybutler/nvm-windows/wiki/Runtime">Runtime</a>, the successor to NVM for Windows.</h2>Complete <a href="https://t.co/oGqQCM9FPx">this form</a> to provide your thoughts and sign up for progress updates.<br/><br/>Updates will also be posted on the <A href="https://linkedin.com/company/authorsoftware">Author Software LinkedIn Page</a>.</div>
<br/><br/>
<h1 align="center">NVM for Windows</h1>

<div align="center">
  The <a href="https://docs.microsoft.com/en-us/windows/nodejs/setup-on-windows">Microsoft</a>/<a href="https://docs.npmjs.com/cli/v9/configuring-npm/install#windows-node-version-managers">npm</a>/<a href="https://cloud.google.com/nodejs/docs/setup#installing_nvm">Google</a> recommended Node.js version manager for <em>Windows</em>.<br/>

<details>
<summary><b>This is not the same thing as nvm!</b> (expand for details)</summary>

_The original [nvm](https://github.com/nvm-sh/nvm) is a completely separate project for Mac/Linux only._ This project uses an entirely different philosophy and is not just a clone of nvm. Details are listed in [Why another version manager?](#bulb-why-another-version-manager) and [what&#39;s the big difference?](#bulb-whats-the-big-difference).
</details>

[![Download Now](https://img.shields.io/badge/-Download%20Now!-%2322A6F2)](https://github.com/coreybutler/nvm-windows/releases) [![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/coreybutler/nvm-windows?label=Latest%20Release&style=social&x=1)]((https://github.com/coreybutler/nvm-windows/releases)) ![GitHub Release Date](https://img.shields.io/github/release-date/coreybutler/nvm-windows?label=Released&style=social) ![GitHub all releases](https://img.shields.io/github/downloads/coreybutler/nvm-windows/total?label=Downloads&style=social) [![Discuss](https://img.shields.io/badge/-Discuss-blue)](https://github.com/coreybutler/nvm-windows/discussions) [![Twitter URL](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Ftwitter.com%2Fintent%2Ftweet%3Fhashtags%3Dnodejs%26original_referer%3Dhttp%253A%252F%252F127.0.0.1%253A91%252F%26text%3DCheck%2520out%2520NVM%2520for%2520Windows%21%26tw_p%3Dtweetbutton%26url%3Dhttp%253A%252F%252Fgithub.com%252Fcoreybutler%252Fnvm-windows%26via%3Dgoldglovecb)](https://twitter.com/intent/tweet?hashtags=nodejs&original_referer=http%3A%2F%2F127.0.0.1%3A91%2F&text=Check%20out%20NVM%20for%20Windows!&tw_p=tweetbutton&url=http%3A%2F%2Fgithub.com%2Fcoreybutler%2Fnvm-windows&via=goldglovecb)
</div>

<h5 align="center">Sponsors</h5>

<div align="center">
  <table cellpadding="5" cellspacing="0" border="0" align="center">
    <tr>
      <td><a href="https://linkedin.com/company/authorsoftware"><img src="https://github.com/coreybutler/staticassets/blob/master/sponsors/logo_author_software_flat.png" width="200px"/></a></td>
      <td width="33%" align="center"><a href="https://ecorventures.com"><img src="https://avatars.githubusercontent.com/u/8259581?s=200&v=4" height="30px"/></a></td>
      <td width="33%" align="center"><a href="https://github.com/microsoft"><img src="https://user-images.githubusercontent.com/770982/195955265-5c3dca78-7140-4ec6-b05a-f308518643ee.png" height="30px"/></a></td>
    </tr>
    <tr>
      <td colspan="4" align="center">
        <a href="https://github.com/sponsors/coreybutler"><img src="https://img.shields.io/github/sponsors/coreybutler?label=Individual%20Sponsors&logo=github&style=social"/></a>
        &nbsp;<a href="https://github.com/sponsors/coreybutler"><img src="https://img.shields.io/badge/-Become%20a%20Sponsor-yellow"/></a>
      </td>
    </tr>
    <tr>
      <td colspan="4" align="center">
        <img src="https://github.blog/wp-content/uploads/2020/09/github-stars-logo_Color.png" width="50"/><br/>
        <b>Can't sponsor?</b><br/>Consider <a href="https://stars.github.com/nominate/" target="_blank">nominating @coreybutler for a Github star</a>.
      </td>
    </tr>
  </table>
</div>
<br/>

<div align="center"><b>Running into issues?</b> See the <a href="https://github.com/coreybutler/nvm-windows/wiki/Common-Issues">common issues wiki</a>.</div>

<br/>
<table style="background-color:red;padding:6px;border-radius:3px;">
  <tr><td>
    <h3>Seeking Feedback:</h3>
    We're working on <a href="https://github.com/coreybutler/nvm-windows/wiki/Runtime">Runtime (rt)</a>, the successor to NVM For Windows. Please contribute by taking a minute to complete <a href="https://t.co/oGqQCM9FPx">this form</a>. Thank you!
    <h3></h3>
  </td></tr>
</table>

## Overview

Manage multiple installations of node.js on a Windows computer.

**tl;dr** Similar (not identical) to [nvm](https://github.com/creationix/nvm), but for Windows. Has an installer. [Download Now](https://github.com/coreybutler/nvm-windows/releases)!

This has always been a node version manager, not an io.js manager, so there is no back-support for io.js. Node 4+ is supported. Remember when running `nvm install` or `nvm use`, Windows usually requires administrative rights (to create symlinks). To install the latest version of Node.js, run `nvm install latest`. To install the latest stable version, run `nvm install lts`.

![NVM for Windows](https://github.com/coreybutler/staticassets/raw/master/images/nvm-1.1.8-screenshot.jpg)

There are situations where the ability to switch between different versions of Node.js can be very useful. For example, if you want to test a module you're developing with the latest bleeding edge version without uninstalling the stable version of node, this utility can help.

![Switch between stable and unstable versions.](https://github.com/coreybutler/staticassets/raw/master/images/nvm-usage-highlighted.jpg)

### Installation & Upgrades

#### :star: :star: Uninstall any pre-existing Node installations!! :star: :star:

The simplest (recommended) way to get NVM for Windows running properly is to uninstall any prior Node installation _before_ installing NVM for Windows. It avoids all of the pitfalls listed below. However; you may not wish to nuke your Node installation if you've highly customized it. NVM for Windows _can_ assume management of an existing installation, but there are nuances to this (dependent entirely on the permissions of the user running the installation). If you have an administrative account, it's relatively safe to install NVM for Windows before uninstalling the original Node version. If you are working in a closed environment, such as a corporate Active Directory environment where installations/uninstallations are controlled by group policy, you should really consider removing the original version of Node before installing NVM4W.

_Permission Problems_
For security reasons, Windows will not allow an application from one vendor to "uninstall" an application from a different vendor. The official NVM4W installer will attempt assume management of an existing installation of Node., but it cannot actually uninstall the original Node.js version. To work around this, NVM for Windows installer attempts to copy the original Node.js installation files to the NVM root. This includes global npm modules and configurations. Once this process is complete, the original Node.js installation can be uninstalled without losing data.

_PATH Installation Problems_
If you attempt to configure the `NVM_SYMLINK` to use an existing directory (like `C:\Program Files\nodejs`), it will fail because a symlink cannot overwrite a physical directory. This is not a problem if you choose a different symlink path (such as `C:\nvm\node`).

_PATH Conflicts_
If you do not uninstall the original version, running `nvm use` may appear to do nothing at all. Running `node -v` will always show the original installation version. This is due to a [`PATH` conflict](https://github.com/coreybutler/nvm-windows/wiki/Common-Issues#why-do-i-need-to-uninstall-nodejs-before-installing-nvm-for-windows) that presents when the same application is installed multiple times. In NVM4W 1.1.11+, run `nvm debug` to determine if you have a `PATH` conflict.

For simpliciy, we recommend uninstalling any existing versions of Node.js before using NVM for Windows. Delete any existing Node.js installation directories (e.g., `%ProgramFiles%\nodejs`) that might remain. NVM's generated symlink will not overwrite an existing (even empty) installation directory.

:eyes: **Backup any global `npmrc` config** :eyes:
(e.g. `%AppData%\npm\etc\npmrc`)

Alternatively, copy the settings to the user config `%UserProfile%\.npmrc`. Delete the existing npm install location (e.g. `%AppData%\npm`) to prevent global module conflicts.

#### Install nvm-windows

Use the [latest installer](https://github.com/coreybutler/nvm/releases) (comes with an uninstaller). Alternatively, follow the  [manual installation](https://github.com/coreybutler/nvm-windows/wiki#manual-installation) guide.

_If NVM4W doesn't appear to work immediately after installation, restart the terminal/powershell (not the whole computer)._

![NVM for Windows Installer](https://github.com/coreybutler/staticassets/raw/master/images/nvm-installer.jpg)

#### Reinstall any global utilities

After install, reinstalling global utilities (e.g. yarn) will have to be done for each installed version of node:

```
nvm use 14.0.0
npm install -g yarn
nvm use 12.0.1
npm install -g yarn
```

### Upgrading nvm-windows

:bulb: _As of v1.1.8, there is an upgrade utility that will automate the upgrade process._

**To upgrade nvm-windows**, run the new installer. It will safely overwrite the files it needs to update without touching your node.js installations. Make sure you use the same installation and symlink folder. If you originally installed to the default locations, you just need to click "next" on each window until it finishes.

### Usage

**nvm-windows runs in an Admin shell**. You'll need to start `powershell` or Command Prompt as Administrator to use nvm-windows

NVM for Windows is a command line tool. Simply type `nvm` in the console for help. The basic commands are:

- **`nvm arch [32|64]`**: Show if node is running in 32 or 64 bit mode. Specify 32 or 64 to override the default architecture.
- **`nvm debug`**: Check the NVM4W process for known problems.
- **`nvm current`**: Display active version.
- **`nvm install <version> [arch]`**:  The version can be a specific version, "latest" for the latest current version, or "lts" for the most recent LTS version. Optionally specify whether to install the 32 or 64 bit version (defaults to system arch). Set [arch] to "all" to install 32 AND 64 bit versions. Add `--insecure` to the end of this command to bypass SSL validation of the remote download server.
- **`nvm list [available]`**: List the node.js installations. Type `available` at the end to show a list of versions available for download.
- **`nvm on`**: Enable node.js version management.
- **`nvm off`**: Disable node.js version management (does not uninstall anything).
- **`nvm proxy [url]`**: Set a proxy to use for downloads. Leave `[url]` blank to see the current proxy. Set `[url]` to "none" to remove the proxy.
- **`nvm uninstall <version>`**: Uninstall a specific version.
- **`nvm use <version> [arch]`**: Switch to use the specified version. Optionally use `latest`, `lts`, or `newest`. `newest` is the latest _installed_ version. Optionally specify 32/64bit architecture. `nvm use <arch>` will continue using the selected version, but switch to 32/64 bit mode. For information about using `use` in a specific directory (or using `.nvmrc`), please refer to [issue #16](https://github.com/coreybutler/nvm-windows/issues/16).
- **`nvm root <path>`**: Set the directory where nvm should store different versions of node.js. If `<path>` is not set, the current root will be displayed.
- **`nvm version`**: Displays the current running version of NVM for Windows.
- **`nvm node_mirror <node_mirror_url>`**: Set the node mirror.People in China can use *https://npmmirror.com/mirrors/node/*
- **`nvm npm_mirror <npm_mirror_url>`**: Set the npm mirror.People in China can use *https://npmmirror.com/mirrors/npm/*

### :warning: Gotcha!

Please note that any global npm modules you may have installed are **not** shared between the various versions of node.js you have installed. Additionally, some npm modules may not be supported in the version of node you're using, so be aware of your environment as you work.

### :name_badge: Antivirus

Users have reported some problems using antivirus, specifically McAfee. It appears the antivirus software is manipulating access to the VBScript engine. See [issue #133](https://github.com/coreybutler/nvm-windows/issues/133) for details and resolution.

**v1.1.8 is not code signed**, but all other versions are signed by [Ecor Ventures LLC](https://ecorventures.com)/[Author.io](https://author.io). This should help prevent false positives with most antivirus software.

> v1.1.8+ was not code signed due to an expired certificate (see the [release notes](https://github.com/coreybutler/nvm-windows/releases/tag/1.1.8) for reasons). **v1.1.9 _is_ code signed** thanks to [ajyong](https://github.com/ajyong), who sponsored the new certificate.

### Using Yarn

**tldr;** `npm i -g yarn`

See the [wiki](https://github.com/coreybutler/nvm-windows/wiki/Common-Issues#how-do-i-use-yarn-with-nvm-windows) for details.

### Build from source

- Install go from http://golang.org
- Download source / Git Clone the repo
- Change GOARCH to amd64 in build.bat if you feel like building a 64-bit executable
- Fire up a Windows command prompt and change directory to project dir
- Execute `go get github.com/blang/semver`
- Execute `go get github.com/olekukonko/tablewriter`
- Execute `build.bat`
- Check the `dist`directory for generated setup program.

---

## :bulb: Why another version manager?

There are several version managers for node.js. Tools like [nvm](https://github.com/creationix/nvm) and [n](https://github.com/tj/n)
only run on Mac OSX and Linux. Windows users are left in the cold? No. [nvmw](https://github.com/hakobera/nvmw) and [nodist](https://github.com/marcelklehr/nodist)
are both designed for Windows. So, why another version manager for Windows?

The architecture of most node version managers for Windows rely on `.bat` files, which do some clever tricks to set or mimic environment variables. Some of them use node itself (once it's downloaded), which is admirable, but prone to problems. Right around node 0.10.30, the installation structure changed a little, causing some of these to just stop working with anything new.

Additionally, some users struggle to install these modules since it requires a little more knowledge of node's installation structure. I believe if it were easier for people to switch between versions, people might take the time to test their code on back and future versions... which is just good practice.

## :bulb: What's the big difference?

First and foremost, this version of nvm has no dependency on node. It's written in [Go](https://golang.org/), which is a much more structured approach than hacking around a limited `.bat` file. It does not rely on having an existing node installation. Go offers the ability to create a Mac/Linux version on the same code base. In fact, this is already underway.

The control mechanism is also quite different. There are two general ways to support multiple node installations with hot switching capabilities. The first is to modify the system `PATH` any time you switch versions, or bypass it by using a `.bat` file to mimic the node executable and redirect accordingly. This always seemed a little hackish to me, and there are some quirks as a result of this implementation.

The second option is to use a symlink. This concept requires putting the symlink in the system `PATH`, then updating its target to the node installation directory you want to use. This is a straightforward approach, and seems to be what people recommend.... until they realize just how much of a pain symlinks are on Windows. This is why it hasn't happened before.

In order to create/modify a symlink, you must be running as an admin, and you must get around Windows UAC (that annoying prompt). Luckily, this is a challenge I already solved with some helper scripts in [node-windows](https://github.com/coreybutler/node-windows). As a result, NVM for Windows maintains a single symlink that is put in the system `PATH` during installation only. Switching to different versions of node is a matter of switching the symlink target. As a result, this utility does **not** require you to run `nvm use x.x.x` every time you open a console window. When you _do_ run `nvm use x.x.x`, the active version of node is automatically updated across all open console windows. It also persists between system reboots, so you only need to use nvm when you want to make a change.

NVM for Windows comes with an installer, courtesy of a byproduct of my work on [Fenix Web Server](https://preview.fenixwebserver.com).

Overall, this project brings together some ideas, a few battle-hardened pieces of other modules, and support for newer versions of node.

NVM for Windows recognizes the "latest" versions using a [list](https://nodejs.org/download/release/index.json) provided by the Node project. Version 1.1.1+ use this list. Before this list existed, I was scraping releases and serving it as a standalone [data feed](https://github.com/coreybutler/nodedistro). This list was used in versions 1.1.0 and prior, but is now deprecated.

## Motivation

I needed it, plain and simple. Additionally, it's apparent that [support for multiple versions](https://github.com/nodejs/node-v0.x-archive/issues/8075) is not coming to node core. It was also an excuse to play with Go.

## Why Go? Why not Node?

I chose Go because it is cross-platform, felt like less overhead than Java, has been around longer than most people think. Plus, I wanted to experiment with it. I've been asked why I didn't write it with Node. Trying to write a tool with the tool you're trying to install doesn't make sense to me. As a result, my project requirements for this were simple... something that's not Node. Node will continue to evolve and change. If you need a reminder of that, remember io.js, Ayo, all the breaking changes between 4.x.x and 6.x.x, and the shift to ES Modules in 12+. Change is inevitable in the world of software. JavaScript is extremely dynamic.

## :pray: Thanks

Thanks to everyone who has submitted issues on and off Github, made suggestions, and generally helped make this a better project. Special thanks to

- [@vkbansal](https://github.com/vkbansal), who provided significant early feedback throughout the early releases.
- [@rainabba](https://github.com/rainabba) and [@sullivanpt](https://github.com/sullivanpt) for getting Node v4 support integrated.
- [@s-h-a-d-o-w](https://github.com/s-h-a-d-o-w) who resolved the longstanding space escaping issue in path names ([#355](https://github.com/coreybutler/nvm-windows/pull/355)).
- [ajyong](https://github.com/ajyong) who sponsored the code signing certificate in late 2021.

<br/>

![Contributors](https://contrib.rocks/image?repo=coreybutler/nvm-windows)

AI Overview
To deploy a web application to Firebase Hosting, the following steps outline the process for installing the necessary tools and initiating the deployment:
1. Install the Firebase CLI:
The Firebase Command Line Interface (CLI) is essential for interacting with Firebase services, including Hosting. If Node.js and npm are not already installed, they must be installed first.
Code

npm install -g firebase-tools
2. Initialize Your Project:
Navigate to the root directory of your local project in the terminal and initialize Firebase Hosting for your project.
Code

firebase init hosting
During the initialization process, the CLI will prompt for the following:
Select a Firebase project:
Choose the Firebase project to which you want to connect your local directory. This becomes the default project.
Specify a public root directory:
This directory will contain all your publicly served static files (e.g., index.html, CSS, JavaScript, images). The default is public. If the directory doesn't exist, Firebase will create it.
3. Deploy Your Application:
Once the project is initialized and the firebase.json configuration file is set up, you can deploy your application to Firebase Hosting.
Code

firebase deploy --only hosting
This command builds and deploys the contents of your public directory to Firebase Hosting. You can then access your deployed application via the URL provided in the terminal output.
AI Overview
The latest version of the Google API Client Library for Python (google-api-python-client) can be installed using pip, preferably within a virtual environment.
Installation Steps:
Create a Virtual Environment (Recommended):

AI Overview
To use the latest version of the Google API Client Library for Python (google-api-python-client) within a virtual environment, follow these steps: Create a Virtual Environment.
It is recommended to use venv (built-in with Python 3) or virtualenv to create an isolated environment for your project.
Code

    python -m venv my_project_env
Activate the Virtual Environment.
Activate the newly created virtual environment. The command varies slightly depending on your operating system. Linux/macOS.
Code

        source my_project_env/bin/activate
Windows (Command Prompt).
Code

        my_project_env\Scripts\activate.bat
Windows (PowerShell).
Code

        my_project_env\Scripts\Activate.ps1
Install the Google API Client Library.
Once the virtual environment is active, install the google-api-python-client using pip. This will install the latest available version by default.
Code

    pip install --upgrade google-api-python-client
The --upgrade flag ensures that if an older version is already present, it will be updated to the latest.
After these steps, the google-api-python-client and its dependencies will be installed within my_project_env, isolated from your system's global Python packages. You can then proceed to use the library in your Python scripts within this activated environment.
Mac/Linux:
Code

        python3 -m venv <your-env>
        source <your-env>/bin/activate
Windows.
Code

        py -m venv <your-env>
        .\<your-env>\Scripts\activate
Replace <your-env> with your desired virtual environment name. Install the Library.
Once your virtual environment is activated, install the library using pip:
Code

    pip install --upgrade google-api-python-client
The --upgrade flag ensures you get the latest available version.
Supported Python Versions:
The google-api-python-client library officially supports Python versions 3.7 and later. Using older, unsupported Python versions may lead to unexpected behavior or authentication issues.

AI Overview
The google-api-python-client is a Python library for interacting with various Google APIs. While it can be used to interact with Firebase-related APIs, the standard and recommended way to deploy a Firebase application is by using the Firebase Command Line Interface (CLI).
Installation of Firebase CLI:
•	Install Node.js and npm: Ensure Node.js and npm (Node Package Manager) are installed on your system, as the Firebase CLI is an npm package.
•	Install Firebase CLI: Open your terminal or command prompt and run the following command:
Code
    npm install -g firebase-tools
This command installs the Firebase CLI globally on your machine.
Deployment of Firebase App:
•	Authenticate Firebase CLI: After installation, authenticate the CLI with your Google account by running:
Code
    firebase login
•	Initialize Firebase Project (if not already done): Navigate to your project's root directory and run:
Code
    firebase init
Follow the prompts to select Firebase features and link your project to a Firebase project in the Google Cloud Console.
•	Deploy your application: To deploy your Firebase application (e.g., Firebase Hosting content, Cloud Functions), execute the following command from your project's root directory:
Code
    firebase deploy
This command deploys all configured Firebase services within your project.
Note: While the google-api-python-client can be used for more programmatic interaction with Firebase APIs (e.g., for custom deployment scripts or automation beyond the CLI's capabilities), the Firebase CLI provides a streamlined and efficient method for most Firebase app deployments.

AI Overview
The google-api-python-client is a Python library for interacting with various Google APIs. While it can be used to interact with Firebase-related APIs, the standard and recommended way to deploy a Firebase application is by using the Firebase Command Line Interface (CLI).
Installation of Firebase CLI:
•	Install Node.js and npm: Ensure Node.js and npm (Node Package Manager) are installed on your system, as the Firebase CLI is an npm package.
•	Install Firebase CLI: Open your terminal or command prompt and run the following command:
Code
    npm install -g firebase-tools
This command installs the Firebase CLI globally on your machine.
Deployment of Firebase App:
•	Authenticate Firebase CLI: After installation, authenticate the CLI with your Google account by running:
Code
    firebase login
•	Initialize Firebase Project (if not already done): Navigate to your project's root directory and run:
Code
    firebase init
Follow the prompts to select Firebase features and link your project to a Firebase project in the Google Cloud Console.
•	Deploy your application: To deploy your Firebase application (e.g., Firebase Hosting content, Cloud Functions), execute the following command from your project's root directory:
Code
    firebase deploy
This command deploys all configured Firebase services within your project.
Note: While the google-api-python-client can be used for more programmatic interaction with Firebase APIs (e.g., for custom deployment scripts or automation beyond the CLI's capabilities), the Firebase CLI provides a streamlined and efficient method for most Firebase app deployments.


# firebaseconsappcodewebsite
Google Cloud Python Client
==========================

Python idiomatic clients for `Google Cloud Platform`_ services.

.. _Google Cloud Platform: https://cloud.google.com/


Stability levels
*******************

The `development status classifier`_ on PyPI indicates the current stability
of a package.

.. _development status classifier: https://pypi.org/classifiers/

General Availability
--------------------

**GA** (general availability) indicates that the client library for a
particular service is stable, and that the code surface will not change in
backwards-incompatible ways unless either absolutely necessary (e.g. because
of critical security issues) or with an extensive deprecation period.
Issues and requests against GA libraries are addressed with the highest
priority.

GA libraries have development status classifier ``Development Status :: 5 - Production/Stable``.

.. note::

    Sub-components of GA libraries explicitly marked as beta in the
    import path (e.g. ``google.cloud.language_v1beta2``) should be considered
    to be beta.

Beta Support
------------

**Beta** indicates that the client library for a particular service is
mostly stable and is being prepared for release. Issues and requests
against beta libraries are addressed with a higher priority.

Beta libraries have development status classifier ``Development Status :: 4 - Beta``.

Alpha Support
-------------

**Alpha** indicates that the client library for a particular service is
still a work-in-progress and is more likely to get backwards-incompatible
updates. See `versioning`_ for more details.


Alpha libraries have development status classifier ``Development Status :: 3 - Alpha``.

If you need support for other Google APIs, check out the
`Google APIs Python Client library`_.

.. _Google APIs Python Client library: https://github.com/google/google-api-python-client


Libraries
*********

.. This table is generated, see synth.py for details.

.. API_TABLE_START

.. list-table::
   :header-rows: 1

   * - Client
     - Release Level
     - Version
     - API Issues
     - File an API Issue
     - Client Library Issues
   * - `A python wrapper of the C library 'CRC32C' <https://github.com/googleapis/python-crc32c>`_
     - stable
     - |PyPI-google-crc32c|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/python-crc32c/issues>`_
   * - `AI Platform <https://github.com/googleapis/python-aiplatform>`_
     - stable
     - |PyPI-google-cloud-aiplatform|
     - `API Issues <https://issuetracker.google.com/savedsearches/559744>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187220>`_
     - `Client Library Issues <https://github.com/googleapis/python-aiplatform/issues>`_
   * - `AI Platform Notebooks <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-notebooks>`_
     - stable
     - |PyPI-google-cloud-notebooks|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `API Gateway <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-api-gateway>`_
     - stable
     - |PyPI-google-cloud-api-gateway|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `APIs Common Protos <https://github.com/googleapis/google-cloud-python/tree/main/packages/googleapis-common-protos>`_
     - stable
     - |PyPI-googleapis-common-protos|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Access Approval <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-access-approval>`_
     - stable
     - |PyPI-google-cloud-access-approval|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Apigee Connect <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-apigee-connect>`_
     - stable
     - |PyPI-google-cloud-apigee-connect|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `App Engine Admin <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-appengine-admin>`_
     - stable
     - |PyPI-google-cloud-appengine-admin|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `App Engine Logging Protos <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-appengine-logging>`_
     - stable
     - |PyPI-google-cloud-appengine-logging|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Artifact Registry <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-artifact-registry>`_
     - stable
     - |PyPI-google-cloud-artifact-registry|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Asset Inventory <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-asset>`_
     - stable
     - |PyPI-google-cloud-asset|
     - `API Issues <https://issuetracker.google.com/savedsearches/559757>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187210>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Assured Workloads for Government <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-assured-workloads>`_
     - stable
     - |PyPI-google-cloud-assured-workloads|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `AutoML <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-automl>`_
     - stable
     - |PyPI-google-cloud-automl|
     - `API Issues <https://issuetracker.google.com/savedsearches/559744>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187220>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Bare Metal Solution <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-bare-metal-solution>`_
     - stable
     - |PyPI-google-cloud-bare-metal-solution|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `BigQuery <https://github.com/googleapis/python-bigquery>`_
     - stable
     - |PyPI-google-cloud-bigquery|
     - `API Issues <https://issuetracker.google.com/savedsearches/559654>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187149>`_
     - `Client Library Issues <https://github.com/googleapis/python-bigquery/issues>`_
   * - `BigQuery Connection <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-bigquery-connection>`_
     - stable
     - |PyPI-google-cloud-bigquery-connection|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `BigQuery Data Transfer <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-bigquery-datatransfer>`_
     - stable
     - |PyPI-google-cloud-bigquery-datatransfer|
     - `API Issues <https://issuetracker.google.com/savedsearches/559654>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187149>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `BigQuery Logging Protos <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-bigquery-logging>`_
     - stable
     - |PyPI-google-cloud-bigquery-logging|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `BigQuery Reservation <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-bigquery-reservation>`_
     - stable
     - |PyPI-google-cloud-bigquery-reservation|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `BigQuery Storage <https://github.com/googleapis/python-bigquery-storage>`_
     - stable
     - |PyPI-google-cloud-bigquery-storage|
     - `API Issues <https://issuetracker.google.com/savedsearches/559654>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187149>`_
     - `Client Library Issues <https://github.com/googleapis/python-bigquery-storage/issues>`_
   * - `BigQuery connector for Jupyter and IPython <https://github.com/googleapis/python-bigquery-magics>`_
     - stable
     - |PyPI-bigquery-magics|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/python-bigquery-magics/issues>`_
   * - `Bigtable <https://github.com/googleapis/python-bigtable>`_
     - stable
     - |PyPI-google-cloud-bigtable|
     - `API Issues <https://issuetracker.google.com/savedsearches/559777>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187206>`_
     - `Client Library Issues <https://github.com/googleapis/python-bigtable/issues>`_
   * - `Billing <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-billing>`_
     - stable
     - |PyPI-google-cloud-billing|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Billing Budget <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-billing-budgets>`_
     - stable
     - |PyPI-google-cloud-billing-budgets|
     - `API Issues <https://issuetracker.google.com/savedsearches/559770>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187201>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Binary Authorization <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-binary-authorization>`_
     - stable
     - |PyPI-google-cloud-binary-authorization|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Build <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-build>`_
     - stable
     - |PyPI-google-cloud-build|
     - `API Issues <https://issuetracker.google.com/savedsearches/5226584>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=190802>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Certificate Manager <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-certificate-manager>`_
     - stable
     - |PyPI-google-cloud-certificate-manager|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Channel Services <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-channel>`_
     - stable
     - |PyPI-google-cloud-channel|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Common <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-common>`_
     - stable
     - |PyPI-google-cloud-common|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Composer <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-orchestration-airflow>`_
     - stable
     - |PyPI-google-cloud-orchestration-airflow|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Compute Engine <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-compute>`_
     - stable
     - |PyPI-google-cloud-compute|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:187134>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187134&template=0>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Contact Center AI Insights <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-contact-center-insights>`_
     - stable
     - |PyPI-google-cloud-contact-center-insights|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Container Analysis <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-containeranalysis>`_
     - stable
     - |PyPI-google-cloud-containeranalysis|
     - `API Issues <https://issuetracker.google.com/savedsearches/559777>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187206>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Data Catalog <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-datacatalog>`_
     - stable
     - |PyPI-google-cloud-datacatalog|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Data Fusion <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-data-fusion>`_
     - stable
     - |PyPI-google-cloud-data-fusion|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Data Loss Prevention <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-dlp>`_
     - stable
     - |PyPI-google-cloud-dlp|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Database Migration Service <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-dms>`_
     - stable
     - |PyPI-google-cloud-dms|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Dataplex <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-dataplex>`_
     - stable
     - |PyPI-google-cloud-dataplex|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Dataproc <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-dataproc>`_
     - stable
     - |PyPI-google-cloud-dataproc|
     - `API Issues <https://issuetracker.google.com/savedsearches/559745>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187133>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Dataproc Metastore <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-dataproc-metastore>`_
     - stable
     - |PyPI-google-cloud-dataproc-metastore|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Datastore <https://github.com/googleapis/python-datastore>`_
     - stable
     - |PyPI-google-cloud-datastore|
     - `API Issues <https://issuetracker.google.com/savedsearches/559768>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187197>`_
     - `Client Library Issues <https://github.com/googleapis/python-datastore/issues>`_
   * - `Datastream <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-datastream>`_
     - stable
     - |PyPI-google-cloud-datastream|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Deploy <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-deploy>`_
     - stable
     - |PyPI-google-cloud-deploy|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Dialogflow <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-dialogflow>`_
     - stable
     - |PyPI-google-cloud-dialogflow|
     - `API Issues <https://issuetracker.google.com/savedsearches/5300385>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=501190>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Dialogflow CX <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-dialogflow-cx>`_
     - stable
     - |PyPI-google-cloud-dialogflow-cx|
     - `API Issues <https://issuetracker.google.com/savedsearches/5300385>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=501190>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Document AI <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-documentai>`_
     - stable
     - |PyPI-google-cloud-documentai|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Domains <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-domains>`_
     - stable
     - |PyPI-google-cloud-domains|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Essential Contacts <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-essential-contacts>`_
     - stable
     - |PyPI-google-cloud-essential-contacts|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Eventarc <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-eventarc>`_
     - stable
     - |PyPI-google-cloud-eventarc|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Filestore <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-filestore>`_
     - stable
     - |PyPI-google-cloud-filestore|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Firestore <https://github.com/googleapis/python-firestore>`_
     - stable
     - |PyPI-google-cloud-firestore|
     - `API Issues <https://issuetracker.google.com/savedsearches/5337669>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=530136>`_
     - `Client Library Issues <https://github.com/googleapis/python-firestore/issues>`_
   * - `Functions <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-functions>`_
     - stable
     - |PyPI-google-cloud-functions|
     - `API Issues <https://issuetracker.google.com/savedsearches/559729>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187195>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `GKE Hub <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-gke-hub>`_
     - stable
     - |PyPI-google-cloud-gke-hub|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Grafeas <https://github.com/googleapis/google-cloud-python/tree/main/packages/grafeas>`_
     - stable
     - |PyPI-grafeas|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `IAM Logging Protos <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-iam-logging>`_
     - stable
     - |PyPI-google-cloud-iam-logging|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `IAM Policy Troubleshooter API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-policy-troubleshooter>`_
     - stable
     - |PyPI-google-cloud-policy-troubleshooter|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `IDS <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-ids>`_
     - stable
     - |PyPI-google-cloud-ids|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Identity and Access Management <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-iam>`_
     - stable
     - |PyPI-google-cloud-iam|
     - `API Issues <https://issuetracker.google.com/savedsearches/559761>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187161>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Identity and Access Management <https://github.com/googleapis/google-cloud-python/tree/main/packages/grpc-google-iam-v1>`_
     - stable
     - |PyPI-grpc-google-iam-v1|
     - `API Issues <https://issuetracker.google.com/savedsearches/559761>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187161>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Identity-Aware Proxy <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-iap>`_
     - stable
     - |PyPI-google-cloud-iap|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Key Management Service <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-kms>`_
     - stable
     - |PyPI-google-cloud-kms|
     - `API Issues <https://issuetracker.google.com/savedsearches/5264932>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=190860>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Kubernetes Engine <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-container>`_
     - stable
     - |PyPI-google-cloud-container|
     - `API Issues <https://issuetracker.google.com/savedsearches/559746>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187077>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Live Stream <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-video-live-stream>`_
     - stable
     - |PyPI-google-cloud-video-live-stream|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Logging <https://github.com/googleapis/python-logging>`_
     - stable
     - |PyPI-google-cloud-logging|
     - `API Issues <https://issuetracker.google.com/savedsearches/559764>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187203>`_
     - `Client Library Issues <https://github.com/googleapis/python-logging/issues>`_
   * - `Managed Service for Microsoft Active Directory <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-managed-identities>`_
     - stable
     - |PyPI-google-cloud-managed-identities|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Memorystore for Memcached <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-memcache>`_
     - stable
     - |PyPI-google-cloud-memcache|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Metrics Scopes <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-monitoring-metrics-scopes>`_
     - stable
     - |PyPI-google-cloud-monitoring-metrics-scopes|
     - `API Issues <https://issuetracker.google.com/savedsearches/559785>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187228>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Monitoring Dashboards <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-monitoring-dashboards>`_
     - stable
     - |PyPI-google-cloud-monitoring-dashboards|
     - `API Issues <https://issuetracker.google.com/savedsearches/559785>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187228>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `NDB Client Library for Datastore <https://github.com/googleapis/python-ndb>`_
     - stable
     - |PyPI-google-cloud-ndb|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/python-ndb/issues>`_
   * - `Natural Language <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-language>`_
     - stable
     - |PyPI-google-cloud-language|
     - `API Issues <https://issuetracker.google.com/savedsearches/559753>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187079>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Network Connectivity Center <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-network-connectivity>`_
     - stable
     - |PyPI-google-cloud-network-connectivity|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Network Management <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-network-management>`_
     - stable
     - |PyPI-google-cloud-network-management|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `OS Config <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-os-config>`_
     - stable
     - |PyPI-google-cloud-os-config|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `OS Login <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-os-login>`_
     - stable
     - |PyPI-google-cloud-os-login|
     - `API Issues <https://issuetracker.google.com/savedsearches/559755>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187134>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Optimization <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-optimization>`_
     - stable
     - |PyPI-google-cloud-optimization|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Organization Policy <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-org-policy>`_
     - stable
     - |PyPI-google-cloud-org-policy|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Pandas Data Types for SQL systems (BigQuery, Spanner) <https://github.com/googleapis/python-db-dtypes-pandas>`_
     - stable
     - |PyPI-db-dtypes|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/python-db-dtypes-pandas/issues>`_
   * - `Private Certificate Authority <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-private-ca>`_
     - stable
     - |PyPI-google-cloud-private-ca|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Pub/Sub <https://github.com/googleapis/python-pubsub>`_
     - stable
     - |PyPI-google-cloud-pubsub|
     - `API Issues <https://issuetracker.google.com/savedsearches/559741>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187173>`_
     - `Client Library Issues <https://github.com/googleapis/python-pubsub/issues>`_
   * - `Pub/Sub Lite <https://github.com/googleapis/python-pubsublite>`_
     - stable
     - |PyPI-google-cloud-pubsublite|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/python-pubsublite/issues>`_
   * - `Recommender <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-recommender>`_
     - stable
     - |PyPI-google-cloud-recommender|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Redis <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-redis>`_
     - stable
     - |PyPI-google-cloud-redis|
     - `API Issues <https://issuetracker.google.com/savedsearches/5169231>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=404472>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Resource Manager <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-resource-manager>`_
     - stable
     - |PyPI-google-cloud-resource-manager|
     - `API Issues <https://issuetracker.google.com/savedsearches/559757>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187210>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Retail <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-retail>`_
     - stable
     - |PyPI-google-cloud-retail|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Scheduler <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-scheduler>`_
     - stable
     - |PyPI-google-cloud-scheduler|
     - `API Issues <https://issuetracker.google.com/savedsearches/5411429>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=589898>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Secret Manager <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-secret-manager>`_
     - stable
     - |PyPI-google-cloud-secret-manager|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Security Command Center <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-securitycenter>`_
     - stable
     - |PyPI-google-cloud-securitycenter|
     - `API Issues <https://issuetracker.google.com/savedsearches/559748>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187215>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Security Scanner <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-websecurityscanner>`_
     - stable
     - |PyPI-google-cloud-websecurityscanner|
     - `API Issues <https://issuetracker.google.com/savedsearches/559748>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187215>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Service Control <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-service-control>`_
     - stable
     - |PyPI-google-cloud-service-control|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Service Directory <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-service-directory>`_
     - stable
     - |PyPI-google-cloud-service-directory|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Service Management <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-service-management>`_
     - stable
     - |PyPI-google-cloud-service-management|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Service Usage <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-service-usage>`_
     - stable
     - |PyPI-google-cloud-service-usage|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Shell <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-shell>`_
     - stable
     - |PyPI-google-cloud-shell|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Source Context <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-source-context>`_
     - stable
     - |PyPI-google-cloud-source-context|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Spanner <https://github.com/googleapis/python-spanner>`_
     - stable
     - |PyPI-google-cloud-spanner|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:190851>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=190851>`_
     - `Client Library Issues <https://github.com/googleapis/python-spanner/issues>`_
   * - `Spanner Django <https://github.com/googleapis/python-spanner-django>`_
     - stable
     - |PyPI-django-google-spanner|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:190851>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=190851>`_
     - `Client Library Issues <https://github.com/googleapis/python-spanner-django/issues>`_
   * - `Speech <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-speech>`_
     - stable
     - |PyPI-google-cloud-speech|
     - `API Issues <https://issuetracker.google.com/savedsearches/559758>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187181>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Stackdriver Monitoring <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-monitoring>`_
     - stable
     - |PyPI-google-cloud-monitoring|
     - `API Issues <https://issuetracker.google.com/savedsearches/559785>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187228>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Storage <https://github.com/googleapis/python-storage>`_
     - stable
     - |PyPI-google-cloud-storage|
     - `API Issues <https://issuetracker.google.com/savedsearches/559782>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187243>`_
     - `Client Library Issues <https://github.com/googleapis/python-storage/issues>`_
   * - `Storage Control API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-storage-control>`_
     - stable
     - |PyPI-google-cloud-storage-control|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:187243>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187243&template=1162869>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Storage Transfer Service <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-storage-transfer>`_
     - stable
     - |PyPI-google-cloud-storage-transfer|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `TPU <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-tpu>`_
     - stable
     - |PyPI-google-cloud-tpu|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Talent Solution <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-talent>`_
     - stable
     - |PyPI-google-cloud-talent|
     - `API Issues <https://issuetracker.google.com/savedsearches/559664>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187187>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Tasks <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-tasks>`_
     - stable
     - |PyPI-google-cloud-tasks|
     - `API Issues <https://issuetracker.google.com/savedsearches/5433985>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=608118>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Text-to-Speech <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-texttospeech>`_
     - stable
     - |PyPI-google-cloud-texttospeech|
     - `API Issues <https://issuetracker.google.com/savedsearches/5235428>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=451645>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Trace <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-trace>`_
     - stable
     - |PyPI-google-cloud-trace|
     - `API Issues <https://issuetracker.google.com/savedsearches/559776>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187216>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Transcoder <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-video-transcoder>`_
     - stable
     - |PyPI-google-cloud-video-transcoder|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Translation <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-translate>`_
     - stable
     - |PyPI-google-cloud-translate|
     - `API Issues <https://issuetracker.google.com/savedsearches/559749>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187144>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `VM Migration <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-vm-migration>`_
     - stable
     - |PyPI-google-cloud-vm-migration|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Video Intelligence <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-videointelligence>`_
     - stable
     - |PyPI-google-cloud-videointelligence|
     - `API Issues <https://issuetracker.google.com/savedsearches/5084810>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=190865>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Virtual Private Cloud <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-vpc-access>`_
     - stable
     - |PyPI-google-cloud-vpc-access|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Vision <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-vision>`_
     - stable
     - |PyPI-google-cloud-vision|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Web Risk <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-webrisk>`_
     - stable
     - |PyPI-google-cloud-webrisk|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Workflows <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-workflows>`_
     - stable
     - |PyPI-google-cloud-workflows|
     - `API Issues <https://issuetracker.google.com/savedsearches/559729>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187195>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `reCAPTCHA Enterprise <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-recaptcha-enterprise>`_
     - stable
     - |PyPI-google-cloud-recaptcha-enterprise|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `A unified Python API in BigQuery <https://github.com/googleapis/python-bigquery-dataframes>`_
     - preview
     - |PyPI-bigframes|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/python-bigquery-dataframes/issues>`_
   * - `API Hub API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-apihub>`_
     - preview
     - |PyPI-google-cloud-apihub|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:1447560>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=1447560>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `API Keys <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-api-keys>`_
     - preview
     - |PyPI-google-cloud-api-keys|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Access Context Manager <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-access-context-manager>`_
     - preview
     - |PyPI-google-cloud-access-context-manager|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Ad Manager <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-ads-admanager>`_
     - preview
     - |PyPI-google-ads-admanager|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:1265187>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=1265187&template=1787490>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Address Validation API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-maps-addressvalidation>`_
     - preview
     - |PyPI-google-maps-addressvalidation|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Advisory Notifications <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-advisorynotifications>`_
     - preview
     - |PyPI-google-cloud-advisorynotifications|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `AlloyDB <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-alloydb>`_
     - preview
     - |PyPI-google-cloud-alloydb|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `AlloyDB connectors <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-alloydb-connectors>`_
     - preview
     - |PyPI-google-cloud-alloydb-connectors|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:1194526>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=1194526&template=1689942>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Analytics Admin <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-analytics-admin>`_
     - preview
     - |PyPI-google-analytics-admin|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:187400>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187400>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Analytics Data <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-analytics-data>`_
     - preview
     - |PyPI-google-analytics-data|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:187400>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187400>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Anthos Multicloud <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-gke-multicloud>`_
     - preview
     - |PyPI-google-cloud-gke-multicloud|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Anti Money Laundering AI API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-financialservices>`_
     - preview
     - |PyPI-google-cloud-financialservices|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Apigee Registry API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-apigee-registry>`_
     - preview
     - |PyPI-google-cloud-apigee-registry|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `App Hub API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-apphub>`_
     - preview
     - |PyPI-google-cloud-apphub|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:1509913>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=1509913>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Apps Card Protos <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-apps-card>`_
     - preview
     - |PyPI-google-apps-card|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Apps Script Type Protos <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-apps-script-type>`_
     - preview
     - |PyPI-google-apps-script-type|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Area 120 Tables <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-area120-tables>`_
     - preview
     - |PyPI-google-area120-tables|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Audit Log API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-audit-log>`_
     - preview
     - |PyPI-google-cloud-audit-log|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Backup and DR Service API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-backupdr>`_
     - preview
     - |PyPI-google-cloud-backupdr|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:966572>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=966572>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Backup for GKE <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-gke-backup>`_
     - preview
     - |PyPI-google-cloud-gke-backup|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Batch <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-batch>`_
     - preview
     - |PyPI-google-cloud-batch|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `BeyondCorp AppConnections <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-beyondcorp-appconnections>`_
     - preview
     - |PyPI-google-cloud-beyondcorp-appconnections|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `BeyondCorp AppConnectors <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-beyondcorp-appconnectors>`_
     - preview
     - |PyPI-google-cloud-beyondcorp-appconnectors|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `BeyondCorp AppGateways <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-beyondcorp-appgateways>`_
     - preview
     - |PyPI-google-cloud-beyondcorp-appgateways|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `BeyondCorp ClientConnectorServices <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-beyondcorp-clientconnectorservices>`_
     - preview
     - |PyPI-google-cloud-beyondcorp-clientconnectorservices|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `BeyondCorp ClientGateways <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-beyondcorp-clientgateways>`_
     - preview
     - |PyPI-google-cloud-beyondcorp-clientgateways|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `BigLake API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-bigquery-biglake>`_
     - preview
     - |PyPI-google-cloud-bigquery-biglake|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:187149>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187149&template=1019829>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `BigQuery Analytics Hub <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-bigquery-analyticshub>`_
     - preview
     - |PyPI-google-cloud-bigquery-analyticshub|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `BigQuery Analytics Hub <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-bigquery-data-exchange>`_
     - preview
     - |PyPI-google-cloud-bigquery-data-exchange|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `BigQuery Data Policy <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-bigquery-datapolicies>`_
     - preview
     - |PyPI-google-cloud-bigquery-datapolicies|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `BigQuery Migration <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-bigquery-migration>`_
     - preview
     - |PyPI-google-cloud-bigquery-migration|
     - `API Issues <https://issuetracker.google.com/savedsearches/559654>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187149>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `BigQuery connector for pandas <https://github.com/googleapis/python-bigquery-pandas>`_
     - preview
     - |PyPI-pandas-gbq|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/python-bigquery-pandas/issues>`_
   * - `CSS API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-css>`_
     - preview
     - |PyPI-google-shopping-css|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:826068>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=826068&template=1564577>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Chat API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-apps-chat>`_
     - preview
     - |PyPI-google-apps-chat|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Chronicle API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-chronicle>`_
     - preview
     - |PyPI-google-cloud-chronicle|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:1387895>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=1387895>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Commerce Consumer Procurement API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-commerce-consumer-procurement>`_
     - preview
     - |PyPI-google-cloud-commerce-consumer-procurement|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:1396141>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=1396141>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Confidential Computing API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-confidentialcomputing>`_
     - preview
     - |PyPI-google-cloud-confidentialcomputing|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:1166820>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=1166820>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Controls Partner API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-cloudcontrolspartner>`_
     - preview
     - |PyPI-google-cloud-cloudcontrolspartner|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `DNS <https://github.com/googleapis/python-dns>`_
     - preview
     - |PyPI-google-cloud-dns|
     - `API Issues <https://issuetracker.google.com/savedsearches/559772>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187241>`_
     - `Client Library Issues <https://github.com/googleapis/python-dns/issues>`_
   * - `Data Labeling <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-datalabeling>`_
     - preview
     - |PyPI-google-cloud-datalabeling|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Data Lineage API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-datacatalog-lineage>`_
     - preview
     - |PyPI-google-cloud-datacatalog-lineage|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Data QnA <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-data-qna>`_
     - preview
     - |PyPI-google-cloud-data-qna|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Dataflow <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-dataflow-client>`_
     - preview
     - |PyPI-google-cloud-dataflow-client|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Dataform <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-dataform>`_
     - preview
     - |PyPI-google-cloud-dataform|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Developer Connect API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-developerconnect>`_
     - preview
     - |PyPI-google-cloud-developerconnect|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:1446966>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=1446966&template=1822025>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Device Streaming API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-devicestreaming>`_
     - preview
     - |PyPI-google-cloud-devicestreaming|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:1767292>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=1767292&template=2112325>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Discovery Engine API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-discoveryengine>`_
     - preview
     - |PyPI-google-cloud-discoveryengine|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Distributed Edge Container <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-edgecontainer>`_
     - preview
     - |PyPI-google-cloud-edgecontainer|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Distributed Edge Network API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-edgenetwork>`_
     - preview
     - |PyPI-google-cloud-edgenetwork|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:187192>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187192&template=1162689>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Document AI Toolbox <https://github.com/googleapis/python-documentai-toolbox>`_
     - preview
     - |PyPI-google-cloud-documentai-toolbox|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/python-documentai-toolbox/issues>`_
   * - `Document AI Warehouse <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-contentwarehouse>`_
     - preview
     - |PyPI-google-cloud-contentwarehouse|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Enterprise Knowledge Graph <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-enterpriseknowledgegraph>`_
     - preview
     - |PyPI-google-cloud-enterpriseknowledgegraph|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Error Reporting <https://github.com/googleapis/python-error-reporting>`_
     - preview
     - |PyPI-google-cloud-error-reporting|
     - `API Issues <https://issuetracker.google.com/savedsearches/559780>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187271>`_
     - `Client Library Issues <https://github.com/googleapis/python-error-reporting/issues>`_
   * - `Eventarc Publishing <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-eventarc-publishing>`_
     - preview
     - |PyPI-google-cloud-eventarc-publishing|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `GDC Hardware Management API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-gdchardwaremanagement>`_
     - preview
     - |PyPI-google-cloud-gdchardwaremanagement|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:1563150>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=1563150>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `GKE Connect Gateway <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-gke-connect-gateway>`_
     - preview
     - |PyPI-google-cloud-gke-connect-gateway|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Generative Language API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-ai-generativelanguage>`_
     - preview
     - |PyPI-google-ai-generativelanguage|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Geo Type Protos <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-geo-type>`_
     - preview
     - |PyPI-google-geo-type|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Infrastructure Manager API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-config>`_
     - preview
     - |PyPI-google-cloud-config|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:536700>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=536700>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `KMS Inventory API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-kms-inventory>`_
     - preview
     - |PyPI-google-cloud-kms-inventory|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:190860>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=190860&template=819701>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Last Mile Fleet Solution Delivery API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-maps-fleetengine-delivery>`_
     - preview
     - |PyPI-google-maps-fleetengine-delivery|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Life Sciences <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-life-sciences>`_
     - preview
     - |PyPI-google-cloud-life-sciences|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Local Rides and Deliveries API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-maps-fleetengine>`_
     - preview
     - |PyPI-google-maps-fleetengine|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Managed Lustre API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-lustre>`_
     - preview
     - |PyPI-google-cloud-lustre|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:1625664>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=1625664>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Managed Service for Apache Kafka <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-managedkafka>`_
     - preview
     - |PyPI-google-cloud-managedkafka|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:1376234>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=1376234>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Maps Platform Datasets API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-maps-mapsplatformdatasets>`_
     - preview
     - |PyPI-google-maps-mapsplatformdatasets|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Maps Routing <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-maps-routing>`_
     - preview
     - |PyPI-google-maps-routing|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Marketing Platform Admin API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-ads-marketingplatform-admin>`_
     - preview
     - |PyPI-google-ads-marketingplatform-admin|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Media Translation <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-media-translation>`_
     - preview
     - |PyPI-google-cloud-media-translation|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Meet API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-apps-meet>`_
     - preview
     - |PyPI-google-apps-meet|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:1216362>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=1216362&template=1766418>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Memorystore <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-memorystore>`_
     - preview
     - |PyPI-google-cloud-memorystore|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Memorystore for Redis API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-redis-cluster>`_
     - preview
     - |PyPI-google-cloud-redis-cluster|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:1288776>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=1288776&template=1161103>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Merchant API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-merchant-accounts>`_
     - preview
     - |PyPI-google-shopping-merchant-accounts|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Merchant API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-merchant-conversions>`_
     - preview
     - |PyPI-google-shopping-merchant-conversions|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Merchant API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-merchant-datasources>`_
     - preview
     - |PyPI-google-shopping-merchant-datasources|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Merchant API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-merchant-lfp>`_
     - preview
     - |PyPI-google-shopping-merchant-lfp|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Merchant API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-merchant-notifications>`_
     - preview
     - |PyPI-google-shopping-merchant-notifications|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Merchant API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-merchant-ordertracking>`_
     - preview
     - |PyPI-google-shopping-merchant-ordertracking|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:171084>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=171084&template=555201>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Merchant API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-merchant-products>`_
     - preview
     - |PyPI-google-shopping-merchant-products|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Merchant API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-merchant-promotions>`_
     - preview
     - |PyPI-google-shopping-merchant-promotions|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Merchant Inventories API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-merchant-inventories>`_
     - preview
     - |PyPI-google-shopping-merchant-inventories|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:171084>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=171084&template=555201>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Merchant Reports API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-merchant-reports>`_
     - preview
     - |PyPI-google-shopping-merchant-reports|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:171084>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=171084&template=555201>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Merchant Reviews API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-merchant-reviews>`_
     - preview
     - |PyPI-google-shopping-merchant-reviews|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Migration Center API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-migrationcenter>`_
     - preview
     - |PyPI-google-cloud-migrationcenter|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Model Armor API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-modelarmor>`_
     - preview
     - |PyPI-google-cloud-modelarmor|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:1514910>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=1514910&template=0>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `NetApp API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-netapp>`_
     - preview
     - |PyPI-google-cloud-netapp|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:1144971>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=1144971>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Network Security <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-network-security>`_
     - preview
     - |PyPI-google-cloud-network-security|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Network Services <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-network-services>`_
     - preview
     - |PyPI-google-cloud-network-services|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Oracle Database@API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-oracledatabase>`_
     - preview
     - |PyPI-google-cloud-oracledatabase|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:1492565>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=1492565>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Parallelstore API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-parallelstore>`_
     - preview
     - |PyPI-google-cloud-parallelstore|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Parameter Manager API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-parametermanager>`_
     - preview
     - |PyPI-google-cloud-parametermanager|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:1442085>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=1442085&template=2002674>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Phishing Protection <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-phishing-protection>`_
     - preview
     - |PyPI-google-cloud-phishing-protection|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Places API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-maps-places>`_
     - preview
     - |PyPI-google-maps-places|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Places Insights API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-maps-areainsights>`_
     - preview
     - |PyPI-google-maps-areainsights|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:1624013>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=1624013&template=2026178>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Policy Simulator API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-policysimulator>`_
     - preview
     - |PyPI-google-cloud-policysimulator|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Policy Troubleshooter API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-policytroubleshooter-iam>`_
     - preview
     - |PyPI-google-cloud-policytroubleshooter-iam|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:690790>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=690790&template=1814512>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Private Catalog <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-private-catalog>`_
     - preview
     - |PyPI-google-cloud-private-catalog|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Privileged Access Manager API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-privilegedaccessmanager>`_
     - preview
     - |PyPI-google-cloud-privilegedaccessmanager|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Public Certificate Authority <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-public-ca>`_
     - preview
     - |PyPI-google-cloud-public-ca|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Quotas API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-quotas>`_
     - preview
     - |PyPI-google-cloud-quotas|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:445904>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=445904>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Rapid Migration Assessment API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-rapidmigrationassessment>`_
     - preview
     - |PyPI-google-cloud-rapidmigrationassessment|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Recommendations AI <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-recommendations-ai>`_
     - preview
     - |PyPI-google-cloud-recommendations-ai|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Route Optimization API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-maps-routeoptimization>`_
     - preview
     - |PyPI-google-maps-routeoptimization|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:1546507>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=1546507>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Run <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-run>`_
     - preview
     - |PyPI-google-cloud-run|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Runtime Configurator <https://github.com/googleapis/python-runtimeconfig>`_
     - preview
     - |PyPI-google-cloud-runtimeconfig|
     - `API Issues <https://issuetracker.google.com/savedsearches/559663>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187078>`_
     - `Client Library Issues <https://github.com/googleapis/python-runtimeconfig/issues>`_
   * - `SQLAlchemy dialect for BigQuery <https://github.com/googleapis/python-bigquery-sqlalchemy>`_
     - preview
     - |PyPI-sqlalchemy-bigquery|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/python-bigquery-sqlalchemy/issues>`_
   * - `Secure Source Manager API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-securesourcemanager>`_
     - preview
     - |PyPI-google-cloud-securesourcemanager|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Security Center Management API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-securitycentermanagement>`_
     - preview
     - |PyPI-google-cloud-securitycentermanagement|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Service Health API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-servicehealth>`_
     - preview
     - |PyPI-google-cloud-servicehealth|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:1466723>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=1466723&template=1161103>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Shopping Merchant Quota <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-merchant-quota>`_
     - preview
     - |PyPI-google-shopping-merchant-quota|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:171084>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=171084&template=555201>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Shopping Type Protos <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-type>`_
     - preview
     - |PyPI-google-shopping-type|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Solar API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-maps-solar>`_
     - preview
     - |PyPI-google-maps-solar|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:1356349>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=1356349>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Storage Batch Operations API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-storagebatchoperations>`_
     - preview
     - |PyPI-google-cloud-storagebatchoperations|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:815827>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=815827&template=1395449>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Storage Insights API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-storageinsights>`_
     - preview
     - |PyPI-google-cloud-storageinsights|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:1156610>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=1156610>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Support API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-support>`_
     - preview
     - |PyPI-google-cloud-support|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Telco Automation API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-telcoautomation>`_
     - preview
     - |PyPI-google-cloud-telcoautomation|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:190865>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=190865&template=1161103>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `VMware Engine <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-vmwareengine>`_
     - preview
     - |PyPI-google-cloud-vmwareengine|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Video Stitcher <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-video-stitcher>`_
     - preview
     - |PyPI-google-cloud-video-stitcher|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Vision AI API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-visionai>`_
     - preview
     - |PyPI-google-cloud-visionai|
     - `API Issues <https://issuetracker.google.com/issues?q=componentid:187174>`_
     - `File an API Issue <https://issuetracker.google.com/issues/new?component=187174&template=1161261>`_
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Workspace Add-ons API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-gsuiteaddons>`_
     - preview
     - |PyPI-google-cloud-gsuiteaddons|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Workspace Events API <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-apps-events-subscriptions>`_
     - preview
     - |PyPI-google-apps-events-subscriptions|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_
   * - `Workstations <https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-workstations>`_
     - preview
     - |PyPI-google-cloud-workstations|
     -
     -
     - `Client Library Issues <https://github.com/googleapis/google-cloud-python/issues>`_

.. |PyPI-google-crc32c| image:: https://img.shields.io/pypi/v/google-crc32c.svg
     :target: https://pypi.org/project/google-crc32c
.. |PyPI-google-cloud-aiplatform| image:: https://img.shields.io/pypi/v/google-cloud-aiplatform.svg
     :target: https://pypi.org/project/google-cloud-aiplatform
.. |PyPI-google-cloud-notebooks| image:: https://img.shields.io/pypi/v/google-cloud-notebooks.svg
     :target: https://pypi.org/project/google-cloud-notebooks
.. |PyPI-google-cloud-api-gateway| image:: https://img.shields.io/pypi/v/google-cloud-api-gateway.svg
     :target: https://pypi.org/project/google-cloud-api-gateway
.. |PyPI-googleapis-common-protos| image:: https://img.shields.io/pypi/v/googleapis-common-protos.svg
     :target: https://pypi.org/project/googleapis-common-protos
.. |PyPI-google-cloud-access-approval| image:: https://img.shields.io/pypi/v/google-cloud-access-approval.svg
     :target: https://pypi.org/project/google-cloud-access-approval
.. |PyPI-google-cloud-apigee-connect| image:: https://img.shields.io/pypi/v/google-cloud-apigee-connect.svg
     :target: https://pypi.org/project/google-cloud-apigee-connect
.. |PyPI-google-cloud-appengine-admin| image:: https://img.shields.io/pypi/v/google-cloud-appengine-admin.svg
     :target: https://pypi.org/project/google-cloud-appengine-admin
.. |PyPI-google-cloud-appengine-logging| image:: https://img.shields.io/pypi/v/google-cloud-appengine-logging.svg
     :target: https://pypi.org/project/google-cloud-appengine-logging
.. |PyPI-google-cloud-artifact-registry| image:: https://img.shields.io/pypi/v/google-cloud-artifact-registry.svg
     :target: https://pypi.org/project/google-cloud-artifact-registry
.. |PyPI-google-cloud-asset| image:: https://img.shields.io/pypi/v/google-cloud-asset.svg
     :target: https://pypi.org/project/google-cloud-asset
.. |PyPI-google-cloud-assured-workloads| image:: https://img.shields.io/pypi/v/google-cloud-assured-workloads.svg
     :target: https://pypi.org/project/google-cloud-assured-workloads
.. |PyPI-google-cloud-automl| image:: https://img.shields.io/pypi/v/google-cloud-automl.svg
     :target: https://pypi.org/project/google-cloud-automl
.. |PyPI-google-cloud-bare-metal-solution| image:: https://img.shields.io/pypi/v/google-cloud-bare-metal-solution.svg
     :target: https://pypi.org/project/google-cloud-bare-metal-solution
.. |PyPI-google-cloud-bigquery| image:: https://img.shields.io/pypi/v/google-cloud-bigquery.svg
     :target: https://pypi.org/project/google-cloud-bigquery
.. |PyPI-google-cloud-bigquery-connection| image:: https://img.shields.io/pypi/v/google-cloud-bigquery-connection.svg
     :target: https://pypi.org/project/google-cloud-bigquery-connection
.. |PyPI-google-cloud-bigquery-datatransfer| image:: https://img.shields.io/pypi/v/google-cloud-bigquery-datatransfer.svg
     :target: https://pypi.org/project/google-cloud-bigquery-datatransfer
.. |PyPI-google-cloud-bigquery-logging| image:: https://img.shields.io/pypi/v/google-cloud-bigquery-logging.svg
     :target: https://pypi.org/project/google-cloud-bigquery-logging
.. |PyPI-google-cloud-bigquery-reservation| image:: https://img.shields.io/pypi/v/google-cloud-bigquery-reservation.svg
     :target: https://pypi.org/project/google-cloud-bigquery-reservation
.. |PyPI-google-cloud-bigquery-storage| image:: https://img.shields.io/pypi/v/google-cloud-bigquery-storage.svg
     :target: https://pypi.org/project/google-cloud-bigquery-storage
.. |PyPI-bigquery-magics| image:: https://img.shields.io/pypi/v/bigquery-magics.svg
     :target: https://pypi.org/project/bigquery-magics
.. |PyPI-google-cloud-bigtable| image:: https://img.shields.io/pypi/v/google-cloud-bigtable.svg
     :target: https://pypi.org/project/google-cloud-bigtable
.. |PyPI-google-cloud-billing| image:: https://img.shields.io/pypi/v/google-cloud-billing.svg
     :target: https://pypi.org/project/google-cloud-billing
.. |PyPI-google-cloud-billing-budgets| image:: https://img.shields.io/pypi/v/google-cloud-billing-budgets.svg
     :target: https://pypi.org/project/google-cloud-billing-budgets
.. |PyPI-google-cloud-binary-authorization| image:: https://img.shields.io/pypi/v/google-cloud-binary-authorization.svg
     :target: https://pypi.org/project/google-cloud-binary-authorization
.. |PyPI-google-cloud-build| image:: https://img.shields.io/pypi/v/google-cloud-build.svg
     :target: https://pypi.org/project/google-cloud-build
.. |PyPI-google-cloud-certificate-manager| image:: https://img.shields.io/pypi/v/google-cloud-certificate-manager.svg
     :target: https://pypi.org/project/google-cloud-certificate-manager
.. |PyPI-google-cloud-channel| image:: https://img.shields.io/pypi/v/google-cloud-channel.svg
     :target: https://pypi.org/project/google-cloud-channel
.. |PyPI-google-cloud-common| image:: https://img.shields.io/pypi/v/google-cloud-common.svg
     :target: https://pypi.org/project/google-cloud-common
.. |PyPI-google-cloud-orchestration-airflow| image:: https://img.shields.io/pypi/v/google-cloud-orchestration-airflow.svg
     :target: https://pypi.org/project/google-cloud-orchestration-airflow
.. |PyPI-google-cloud-compute| image:: https://img.shields.io/pypi/v/google-cloud-compute.svg
     :target: https://pypi.org/project/google-cloud-compute
.. |PyPI-google-cloud-contact-center-insights| image:: https://img.shields.io/pypi/v/google-cloud-contact-center-insights.svg
     :target: https://pypi.org/project/google-cloud-contact-center-insights
.. |PyPI-google-cloud-containeranalysis| image:: https://img.shields.io/pypi/v/google-cloud-containeranalysis.svg
     :target: https://pypi.org/project/google-cloud-containeranalysis
.. |PyPI-google-cloud-datacatalog| image:: https://img.shields.io/pypi/v/google-cloud-datacatalog.svg
     :target: https://pypi.org/project/google-cloud-datacatalog
.. |PyPI-google-cloud-data-fusion| image:: https://img.shields.io/pypi/v/google-cloud-data-fusion.svg
     :target: https://pypi.org/project/google-cloud-data-fusion
.. |PyPI-google-cloud-dlp| image:: https://img.shields.io/pypi/v/google-cloud-dlp.svg
     :target: https://pypi.org/project/google-cloud-dlp
.. |PyPI-google-cloud-dms| image:: https://img.shields.io/pypi/v/google-cloud-dms.svg
     :target: https://pypi.org/project/google-cloud-dms
.. |PyPI-google-cloud-dataplex| image:: https://img.shields.io/pypi/v/google-cloud-dataplex.svg
     :target: https://pypi.org/project/google-cloud-dataplex
.. |PyPI-google-cloud-dataproc| image:: https://img.shields.io/pypi/v/google-cloud-dataproc.svg
     :target: https://pypi.org/project/google-cloud-dataproc
.. |PyPI-google-cloud-dataproc-metastore| image:: https://img.shields.io/pypi/v/google-cloud-dataproc-metastore.svg
     :target: https://pypi.org/project/google-cloud-dataproc-metastore
.. |PyPI-google-cloud-datastore| image:: https://img.shields.io/pypi/v/google-cloud-datastore.svg
     :target: https://pypi.org/project/google-cloud-datastore
.. |PyPI-google-cloud-datastream| image:: https://img.shields.io/pypi/v/google-cloud-datastream.svg
     :target: https://pypi.org/project/google-cloud-datastream
.. |PyPI-google-cloud-deploy| image:: https://img.shields.io/pypi/v/google-cloud-deploy.svg
     :target: https://pypi.org/project/google-cloud-deploy
.. |PyPI-google-cloud-dialogflow| image:: https://img.shields.io/pypi/v/google-cloud-dialogflow.svg
     :target: https://pypi.org/project/google-cloud-dialogflow
.. |PyPI-google-cloud-dialogflow-cx| image:: https://img.shields.io/pypi/v/google-cloud-dialogflow-cx.svg
     :target: https://pypi.org/project/google-cloud-dialogflow-cx
.. |PyPI-google-cloud-documentai| image:: https://img.shields.io/pypi/v/google-cloud-documentai.svg
     :target: https://pypi.org/project/google-cloud-documentai
.. |PyPI-google-cloud-domains| image:: https://img.shields.io/pypi/v/google-cloud-domains.svg
     :target: https://pypi.org/project/google-cloud-domains
.. |PyPI-google-cloud-essential-contacts| image:: https://img.shields.io/pypi/v/google-cloud-essential-contacts.svg
     :target: https://pypi.org/project/google-cloud-essential-contacts
.. |PyPI-google-cloud-eventarc| image:: https://img.shields.io/pypi/v/google-cloud-eventarc.svg
     :target: https://pypi.org/project/google-cloud-eventarc
.. |PyPI-google-cloud-filestore| image:: https://img.shields.io/pypi/v/google-cloud-filestore.svg
     :target: https://pypi.org/project/google-cloud-filestore
.. |PyPI-google-cloud-firestore| image:: https://img.shields.io/pypi/v/google-cloud-firestore.svg
     :target: https://pypi.org/project/google-cloud-firestore
.. |PyPI-google-cloud-functions| image:: https://img.shields.io/pypi/v/google-cloud-functions.svg
     :target: https://pypi.org/project/google-cloud-functions
.. |PyPI-google-cloud-gke-hub| image:: https://img.shields.io/pypi/v/google-cloud-gke-hub.svg
     :target: https://pypi.org/project/google-cloud-gke-hub
.. |PyPI-grafeas| image:: https://img.shields.io/pypi/v/grafeas.svg
     :target: https://pypi.org/project/grafeas
.. |PyPI-google-cloud-iam-logging| image:: https://img.shields.io/pypi/v/google-cloud-iam-logging.svg
     :target: https://pypi.org/project/google-cloud-iam-logging
.. |PyPI-google-cloud-policy-troubleshooter| image:: https://img.shields.io/pypi/v/google-cloud-policy-troubleshooter.svg
     :target: https://pypi.org/project/google-cloud-policy-troubleshooter
.. |PyPI-google-cloud-ids| image:: https://img.shields.io/pypi/v/google-cloud-ids.svg
     :target: https://pypi.org/project/google-cloud-ids
.. |PyPI-google-cloud-iam| image:: https://img.shields.io/pypi/v/google-cloud-iam.svg
     :target: https://pypi.org/project/google-cloud-iam
.. |PyPI-grpc-google-iam-v1| image:: https://img.shields.io/pypi/v/grpc-google-iam-v1.svg
     :target: https://pypi.org/project/grpc-google-iam-v1
.. |PyPI-google-cloud-iap| image:: https://img.shields.io/pypi/v/google-cloud-iap.svg
     :target: https://pypi.org/project/google-cloud-iap
.. |PyPI-google-cloud-kms| image:: https://img.shields.io/pypi/v/google-cloud-kms.svg
     :target: https://pypi.org/project/google-cloud-kms
.. |PyPI-google-cloud-container| image:: https://img.shields.io/pypi/v/google-cloud-container.svg
     :target: https://pypi.org/project/google-cloud-container
.. |PyPI-google-cloud-video-live-stream| image:: https://img.shields.io/pypi/v/google-cloud-video-live-stream.svg
     :target: https://pypi.org/project/google-cloud-video-live-stream
.. |PyPI-google-cloud-logging| image:: https://img.shields.io/pypi/v/google-cloud-logging.svg
     :target: https://pypi.org/project/google-cloud-logging
.. |PyPI-google-cloud-managed-identities| image:: https://img.shields.io/pypi/v/google-cloud-managed-identities.svg
     :target: https://pypi.org/project/google-cloud-managed-identities
.. |PyPI-google-cloud-memcache| image:: https://img.shields.io/pypi/v/google-cloud-memcache.svg
     :target: https://pypi.org/project/google-cloud-memcache
.. |PyPI-google-cloud-monitoring-metrics-scopes| image:: https://img.shields.io/pypi/v/google-cloud-monitoring-metrics-scopes.svg
     :target: https://pypi.org/project/google-cloud-monitoring-metrics-scopes
.. |PyPI-google-cloud-monitoring-dashboards| image:: https://img.shields.io/pypi/v/google-cloud-monitoring-dashboards.svg
     :target: https://pypi.org/project/google-cloud-monitoring-dashboards
.. |PyPI-google-cloud-ndb| image:: https://img.shields.io/pypi/v/google-cloud-ndb.svg
     :target: https://pypi.org/project/google-cloud-ndb
.. |PyPI-google-cloud-language| image:: https://img.shields.io/pypi/v/google-cloud-language.svg
     :target: https://pypi.org/project/google-cloud-language
.. |PyPI-google-cloud-network-connectivity| image:: https://img.shields.io/pypi/v/google-cloud-network-connectivity.svg
     :target: https://pypi.org/project/google-cloud-network-connectivity
.. |PyPI-google-cloud-network-management| image:: https://img.shields.io/pypi/v/google-cloud-network-management.svg
     :target: https://pypi.org/project/google-cloud-network-management
.. |PyPI-google-cloud-os-config| image:: https://img.shields.io/pypi/v/google-cloud-os-config.svg
     :target: https://pypi.org/project/google-cloud-os-config
.. |PyPI-google-cloud-os-login| image:: https://img.shields.io/pypi/v/google-cloud-os-login.svg
     :target: https://pypi.org/project/google-cloud-os-login
.. |PyPI-google-cloud-optimization| image:: https://img.shields.io/pypi/v/google-cloud-optimization.svg
     :target: https://pypi.org/project/google-cloud-optimization
.. |PyPI-google-cloud-org-policy| image:: https://img.shields.io/pypi/v/google-cloud-org-policy.svg
     :target: https://pypi.org/project/google-cloud-org-policy
.. |PyPI-db-dtypes| image:: https://img.shields.io/pypi/v/db-dtypes.svg
     :target: https://pypi.org/project/db-dtypes
.. |PyPI-google-cloud-private-ca| image:: https://img.shields.io/pypi/v/google-cloud-private-ca.svg
     :target: https://pypi.org/project/google-cloud-private-ca
.. |PyPI-google-cloud-pubsub| image:: https://img.shields.io/pypi/v/google-cloud-pubsub.svg
     :target: https://pypi.org/project/google-cloud-pubsub
.. |PyPI-google-cloud-pubsublite| image:: https://img.shields.io/pypi/v/google-cloud-pubsublite.svg
     :target: https://pypi.org/project/google-cloud-pubsublite
.. |PyPI-google-cloud-recommender| image:: https://img.shields.io/pypi/v/google-cloud-recommender.svg
     :target: https://pypi.org/project/google-cloud-recommender
.. |PyPI-google-cloud-redis| image:: https://img.shields.io/pypi/v/google-cloud-redis.svg
     :target: https://pypi.org/project/google-cloud-redis
.. |PyPI-google-cloud-resource-manager| image:: https://img.shields.io/pypi/v/google-cloud-resource-manager.svg
     :target: https://pypi.org/project/google-cloud-resource-manager
.. |PyPI-google-cloud-retail| image:: https://img.shields.io/pypi/v/google-cloud-retail.svg
     :target: https://pypi.org/project/google-cloud-retail
.. |PyPI-google-cloud-scheduler| image:: https://img.shields.io/pypi/v/google-cloud-scheduler.svg
     :target: https://pypi.org/project/google-cloud-scheduler
.. |PyPI-google-cloud-secret-manager| image:: https://img.shields.io/pypi/v/google-cloud-secret-manager.svg
     :target: https://pypi.org/project/google-cloud-secret-manager
.. |PyPI-google-cloud-securitycenter| image:: https://img.shields.io/pypi/v/google-cloud-securitycenter.svg
     :target: https://pypi.org/project/google-cloud-securitycenter
.. |PyPI-google-cloud-websecurityscanner| image:: https://img.shields.io/pypi/v/google-cloud-websecurityscanner.svg
     :target: https://pypi.org/project/google-cloud-websecurityscanner
.. |PyPI-google-cloud-service-control| image:: https://img.shields.io/pypi/v/google-cloud-service-control.svg
     :target: https://pypi.org/project/google-cloud-service-control
.. |PyPI-google-cloud-service-directory| image:: https://img.shields.io/pypi/v/google-cloud-service-directory.svg
     :target: https://pypi.org/project/google-cloud-service-directory
.. |PyPI-google-cloud-service-management| image:: https://img.shields.io/pypi/v/google-cloud-service-management.svg
     :target: https://pypi.org/project/google-cloud-service-management
.. |PyPI-google-cloud-service-usage| image:: https://img.shields.io/pypi/v/google-cloud-service-usage.svg
     :target: https://pypi.org/project/google-cloud-service-usage
.. |PyPI-google-cloud-shell| image:: https://img.shields.io/pypi/v/google-cloud-shell.svg
     :target: https://pypi.org/project/google-cloud-shell
.. |PyPI-google-cloud-source-context| image:: https://img.shields.io/pypi/v/google-cloud-source-context.svg
     :target: https://pypi.org/project/google-cloud-source-context
.. |PyPI-google-cloud-spanner| image:: https://img.shields.io/pypi/v/google-cloud-spanner.svg
     :target: https://pypi.org/project/google-cloud-spanner
.. |PyPI-django-google-spanner| image:: https://img.shields.io/pypi/v/django-google-spanner.svg
     :target: https://pypi.org/project/django-google-spanner
.. |PyPI-google-cloud-speech| image:: https://img.shields.io/pypi/v/google-cloud-speech.svg
     :target: https://pypi.org/project/google-cloud-speech
.. |PyPI-google-cloud-monitoring| image:: https://img.shields.io/pypi/v/google-cloud-monitoring.svg
     :target: https://pypi.org/project/google-cloud-monitoring
.. |PyPI-google-cloud-storage| image:: https://img.shields.io/pypi/v/google-cloud-storage.svg
     :target: https://pypi.org/project/google-cloud-storage
.. |PyPI-google-cloud-storage-control| image:: https://img.shields.io/pypi/v/google-cloud-storage-control.svg
     :target: https://pypi.org/project/google-cloud-storage-control
.. |PyPI-google-cloud-storage-transfer| image:: https://img.shields.io/pypi/v/google-cloud-storage-transfer.svg
     :target: https://pypi.org/project/google-cloud-storage-transfer
.. |PyPI-google-cloud-tpu| image:: https://img.shields.io/pypi/v/google-cloud-tpu.svg
     :target: https://pypi.org/project/google-cloud-tpu
.. |PyPI-google-cloud-talent| image:: https://img.shields.io/pypi/v/google-cloud-talent.svg
     :target: https://pypi.org/project/google-cloud-talent
.. |PyPI-google-cloud-tasks| image:: https://img.shields.io/pypi/v/google-cloud-tasks.svg
     :target: https://pypi.org/project/google-cloud-tasks
.. |PyPI-google-cloud-texttospeech| image:: https://img.shields.io/pypi/v/google-cloud-texttospeech.svg
     :target: https://pypi.org/project/google-cloud-texttospeech
.. |PyPI-google-cloud-trace| image:: https://img.shields.io/pypi/v/google-cloud-trace.svg
     :target: https://pypi.org/project/google-cloud-trace
.. |PyPI-google-cloud-video-transcoder| image:: https://img.shields.io/pypi/v/google-cloud-video-transcoder.svg
     :target: https://pypi.org/project/google-cloud-video-transcoder
.. |PyPI-google-cloud-translate| image:: https://img.shields.io/pypi/v/google-cloud-translate.svg
     :target: https://pypi.org/project/google-cloud-translate
.. |PyPI-google-cloud-vm-migration| image:: https://img.shields.io/pypi/v/google-cloud-vm-migration.svg
     :target: https://pypi.org/project/google-cloud-vm-migration
.. |PyPI-google-cloud-videointelligence| image:: https://img.shields.io/pypi/v/google-cloud-videointelligence.svg
     :target: https://pypi.org/project/google-cloud-videointelligence
.. |PyPI-google-cloud-vpc-access| image:: https://img.shields.io/pypi/v/google-cloud-vpc-access.svg
     :target: https://pypi.org/project/google-cloud-vpc-access
.. |PyPI-google-cloud-vision| image:: https://img.shields.io/pypi/v/google-cloud-vision.svg
     :target: https://pypi.org/project/google-cloud-vision
.. |PyPI-google-cloud-webrisk| image:: https://img.shields.io/pypi/v/google-cloud-webrisk.svg
     :target: https://pypi.org/project/google-cloud-webrisk
.. |PyPI-google-cloud-workflows| image:: https://img.shields.io/pypi/v/google-cloud-workflows.svg
     :target: https://pypi.org/project/google-cloud-workflows
.. |PyPI-google-cloud-recaptcha-enterprise| image:: https://img.shields.io/pypi/v/google-cloud-recaptcha-enterprise.svg
     :target: https://pypi.org/project/google-cloud-recaptcha-enterprise
.. |PyPI-bigframes| image:: https://img.shields.io/pypi/v/bigframes.svg
     :target: https://pypi.org/project/bigframes
.. |PyPI-google-cloud-apihub| image:: https://img.shields.io/pypi/v/google-cloud-apihub.svg
     :target: https://pypi.org/project/google-cloud-apihub
.. |PyPI-google-cloud-api-keys| image:: https://img.shields.io/pypi/v/google-cloud-api-keys.svg
     :target: https://pypi.org/project/google-cloud-api-keys
.. |PyPI-google-cloud-access-context-manager| image:: https://img.shields.io/pypi/v/google-cloud-access-context-manager.svg
     :target: https://pypi.org/project/google-cloud-access-context-manager
.. |PyPI-google-ads-admanager| image:: https://img.shields.io/pypi/v/google-ads-admanager.svg
     :target: https://pypi.org/project/google-ads-admanager
.. |PyPI-google-maps-addressvalidation| image:: https://img.shields.io/pypi/v/google-maps-addressvalidation.svg
     :target: https://pypi.org/project/google-maps-addressvalidation
.. |PyPI-google-cloud-advisorynotifications| image:: https://img.shields.io/pypi/v/google-cloud-advisorynotifications.svg
     :target: https://pypi.org/project/google-cloud-advisorynotifications
.. |PyPI-google-cloud-alloydb| image:: https://img.shields.io/pypi/v/google-cloud-alloydb.svg
     :target: https://pypi.org/project/google-cloud-alloydb
.. |PyPI-google-cloud-alloydb-connectors| image:: https://img.shields.io/pypi/v/google-cloud-alloydb-connectors.svg
     :target: https://pypi.org/project/google-cloud-alloydb-connectors
.. |PyPI-google-analytics-admin| image:: https://img.shields.io/pypi/v/google-analytics-admin.svg
     :target: https://pypi.org/project/google-analytics-admin
.. |PyPI-google-analytics-data| image:: https://img.shields.io/pypi/v/google-analytics-data.svg
     :target: https://pypi.org/project/google-analytics-data
.. |PyPI-google-cloud-gke-multicloud| image:: https://img.shields.io/pypi/v/google-cloud-gke-multicloud.svg
     :target: https://pypi.org/project/google-cloud-gke-multicloud
.. |PyPI-google-cloud-financialservices| image:: https://img.shields.io/pypi/v/google-cloud-financialservices.svg
     :target: https://pypi.org/project/google-cloud-financialservices
.. |PyPI-google-cloud-apigee-registry| image:: https://img.shields.io/pypi/v/google-cloud-apigee-registry.svg
     :target: https://pypi.org/project/google-cloud-apigee-registry
.. |PyPI-google-cloud-apphub| image:: https://img.shields.io/pypi/v/google-cloud-apphub.svg
     :target: https://pypi.org/project/google-cloud-apphub
.. |PyPI-google-apps-card| image:: https://img.shields.io/pypi/v/google-apps-card.svg
     :target: https://pypi.org/project/google-apps-card
.. |PyPI-google-apps-script-type| image:: https://img.shields.io/pypi/v/google-apps-script-type.svg
     :target: https://pypi.org/project/google-apps-script-type
.. |PyPI-google-area120-tables| image:: https://img.shields.io/pypi/v/google-area120-tables.svg
     :target: https://pypi.org/project/google-area120-tables
.. |PyPI-google-cloud-audit-log| image:: https://img.shields.io/pypi/v/google-cloud-audit-log.svg
     :target: https://pypi.org/project/google-cloud-audit-log
.. |PyPI-google-cloud-backupdr| image:: https://img.shields.io/pypi/v/google-cloud-backupdr.svg
     :target: https://pypi.org/project/google-cloud-backupdr
.. |PyPI-google-cloud-gke-backup| image:: https://img.shields.io/pypi/v/google-cloud-gke-backup.svg
     :target: https://pypi.org/project/google-cloud-gke-backup
.. |PyPI-google-cloud-batch| image:: https://img.shields.io/pypi/v/google-cloud-batch.svg
     :target: https://pypi.org/project/google-cloud-batch
.. |PyPI-google-cloud-beyondcorp-appconnections| image:: https://img.shields.io/pypi/v/google-cloud-beyondcorp-appconnections.svg
     :target: https://pypi.org/project/google-cloud-beyondcorp-appconnections
.. |PyPI-google-cloud-beyondcorp-appconnectors| image:: https://img.shields.io/pypi/v/google-cloud-beyondcorp-appconnectors.svg
     :target: https://pypi.org/project/google-cloud-beyondcorp-appconnectors
.. |PyPI-google-cloud-beyondcorp-appgateways| image:: https://img.shields.io/pypi/v/google-cloud-beyondcorp-appgateways.svg
     :target: https://pypi.org/project/google-cloud-beyondcorp-appgateways
.. |PyPI-google-cloud-beyondcorp-clientconnectorservices| image:: https://img.shields.io/pypi/v/google-cloud-beyondcorp-clientconnectorservices.svg
     :target: https://pypi.org/project/google-cloud-beyondcorp-clientconnectorservices
.. |PyPI-google-cloud-beyondcorp-clientgateways| image:: https://img.shields.io/pypi/v/google-cloud-beyondcorp-clientgateways.svg
     :target: https://pypi.org/project/google-cloud-beyondcorp-clientgateways
.. |PyPI-google-cloud-bigquery-biglake| image:: https://img.shields.io/pypi/v/google-cloud-bigquery-biglake.svg
     :target: https://pypi.org/project/google-cloud-bigquery-biglake
.. |PyPI-google-cloud-bigquery-analyticshub| image:: https://img.shields.io/pypi/v/google-cloud-bigquery-analyticshub.svg
     :target: https://pypi.org/project/google-cloud-bigquery-analyticshub
.. |PyPI-google-cloud-bigquery-data-exchange| image:: https://img.shields.io/pypi/v/google-cloud-bigquery-data-exchange.svg
     :target: https://pypi.org/project/google-cloud-bigquery-data-exchange
.. |PyPI-google-cloud-bigquery-datapolicies| image:: https://img.shields.io/pypi/v/google-cloud-bigquery-datapolicies.svg
     :target: https://pypi.org/project/google-cloud-bigquery-datapolicies
.. |PyPI-google-cloud-bigquery-migration| image:: https://img.shields.io/pypi/v/google-cloud-bigquery-migration.svg
     :target: https://pypi.org/project/google-cloud-bigquery-migration
.. |PyPI-pandas-gbq| image:: https://img.shields.io/pypi/v/pandas-gbq.svg
     :target: https://pypi.org/project/pandas-gbq
.. |PyPI-google-shopping-css| image:: https://img.shields.io/pypi/v/google-shopping-css.svg
     :target: https://pypi.org/project/google-shopping-css
.. |PyPI-google-apps-chat| image:: https://img.shields.io/pypi/v/google-apps-chat.svg
     :target: https://pypi.org/project/google-apps-chat
.. |PyPI-google-cloud-chronicle| image:: https://img.shields.io/pypi/v/google-cloud-chronicle.svg
     :target: https://pypi.org/project/google-cloud-chronicle
.. |PyPI-google-cloud-commerce-consumer-procurement| image:: https://img.shields.io/pypi/v/google-cloud-commerce-consumer-procurement.svg
     :target: https://pypi.org/project/google-cloud-commerce-consumer-procurement
.. |PyPI-google-cloud-confidentialcomputing| image:: https://img.shields.io/pypi/v/google-cloud-confidentialcomputing.svg
     :target: https://pypi.org/project/google-cloud-confidentialcomputing
.. |PyPI-google-cloud-cloudcontrolspartner| image:: https://img.shields.io/pypi/v/google-cloud-cloudcontrolspartner.svg
     :target: https://pypi.org/project/google-cloud-cloudcontrolspartner
.. |PyPI-google-cloud-dns| image:: https://img.shields.io/pypi/v/google-cloud-dns.svg
     :target: https://pypi.org/project/google-cloud-dns
.. |PyPI-google-cloud-datalabeling| image:: https://img.shields.io/pypi/v/google-cloud-datalabeling.svg
     :target: https://pypi.org/project/google-cloud-datalabeling
.. |PyPI-google-cloud-datacatalog-lineage| image:: https://img.shields.io/pypi/v/google-cloud-datacatalog-lineage.svg
     :target: https://pypi.org/project/google-cloud-datacatalog-lineage
.. |PyPI-google-cloud-data-qna| image:: https://img.shields.io/pypi/v/google-cloud-data-qna.svg
     :target: https://pypi.org/project/google-cloud-data-qna
.. |PyPI-google-cloud-dataflow-client| image:: https://img.shields.io/pypi/v/google-cloud-dataflow-client.svg
     :target: https://pypi.org/project/google-cloud-dataflow-client
.. |PyPI-google-cloud-dataform| image:: https://img.shields.io/pypi/v/google-cloud-dataform.svg
     :target: https://pypi.org/project/google-cloud-dataform
.. |PyPI-google-cloud-developerconnect| image:: https://img.shields.io/pypi/v/google-cloud-developerconnect.svg
     :target: https://pypi.org/project/google-cloud-developerconnect
.. |PyPI-google-cloud-devicestreaming| image:: https://img.shields.io/pypi/v/google-cloud-devicestreaming.svg
     :target: https://pypi.org/project/google-cloud-devicestreaming
.. |PyPI-google-cloud-discoveryengine| image:: https://img.shields.io/pypi/v/google-cloud-discoveryengine.svg
     :target: https://pypi.org/project/google-cloud-discoveryengine
.. |PyPI-google-cloud-edgecontainer| image:: https://img.shields.io/pypi/v/google-cloud-edgecontainer.svg
     :target: https://pypi.org/project/google-cloud-edgecontainer
.. |PyPI-google-cloud-edgenetwork| image:: https://img.shields.io/pypi/v/google-cloud-edgenetwork.svg
     :target: https://pypi.org/project/google-cloud-edgenetwork
.. |PyPI-google-cloud-documentai-toolbox| image:: https://img.shields.io/pypi/v/google-cloud-documentai-toolbox.svg
     :target: https://pypi.org/project/google-cloud-documentai-toolbox
.. |PyPI-google-cloud-contentwarehouse| image:: https://img.shields.io/pypi/v/google-cloud-contentwarehouse.svg
     :target: https://pypi.org/project/google-cloud-contentwarehouse
.. |PyPI-google-cloud-enterpriseknowledgegraph| image:: https://img.shields.io/pypi/v/google-cloud-enterpriseknowledgegraph.svg
     :target: https://pypi.org/project/google-cloud-enterpriseknowledgegraph
.. |PyPI-google-cloud-error-reporting| image:: https://img.shields.io/pypi/v/google-cloud-error-reporting.svg
     :target: https://pypi.org/project/google-cloud-error-reporting
.. |PyPI-google-cloud-eventarc-publishing| image:: https://img.shields.io/pypi/v/google-cloud-eventarc-publishing.svg
     :target: https://pypi.org/project/google-cloud-eventarc-publishing
.. |PyPI-google-cloud-gdchardwaremanagement| image:: https://img.shields.io/pypi/v/google-cloud-gdchardwaremanagement.svg
     :target: https://pypi.org/project/google-cloud-gdchardwaremanagement
.. |PyPI-google-cloud-gke-connect-gateway| image:: https://img.shields.io/pypi/v/google-cloud-gke-connect-gateway.svg
     :target: https://pypi.org/project/google-cloud-gke-connect-gateway
.. |PyPI-google-ai-generativelanguage| image:: https://img.shields.io/pypi/v/google-ai-generativelanguage.svg
     :target: https://pypi.org/project/google-ai-generativelanguage
.. |PyPI-google-geo-type| image:: https://img.shields.io/pypi/v/google-geo-type.svg
     :target: https://pypi.org/project/google-geo-type
.. |PyPI-google-cloud-config| image:: https://img.shields.io/pypi/v/google-cloud-config.svg
     :target: https://pypi.org/project/google-cloud-config
.. |PyPI-google-cloud-kms-inventory| image:: https://img.shields.io/pypi/v/google-cloud-kms-inventory.svg
     :target: https://pypi.org/project/google-cloud-kms-inventory
.. |PyPI-google-maps-fleetengine-delivery| image:: https://img.shields.io/pypi/v/google-maps-fleetengine-delivery.svg
     :target: https://pypi.org/project/google-maps-fleetengine-delivery
.. |PyPI-google-cloud-life-sciences| image:: https://img.shields.io/pypi/v/google-cloud-life-sciences.svg
     :target: https://pypi.org/project/google-cloud-life-sciences
.. |PyPI-google-maps-fleetengine| image:: https://img.shields.io/pypi/v/google-maps-fleetengine.svg
     :target: https://pypi.org/project/google-maps-fleetengine
.. |PyPI-google-cloud-lustre| image:: https://img.shields.io/pypi/v/google-cloud-lustre.svg
     :target: https://pypi.org/project/google-cloud-lustre
.. |PyPI-google-cloud-managedkafka| image:: https://img.shields.io/pypi/v/google-cloud-managedkafka.svg
     :target: https://pypi.org/project/google-cloud-managedkafka
.. |PyPI-google-maps-mapsplatformdatasets| image:: https://img.shields.io/pypi/v/google-maps-mapsplatformdatasets.svg
     :target: https://pypi.org/project/google-maps-mapsplatformdatasets
.. |PyPI-google-maps-routing| image:: https://img.shields.io/pypi/v/google-maps-routing.svg
     :target: https://pypi.org/project/google-maps-routing
.. |PyPI-google-ads-marketingplatform-admin| image:: https://img.shields.io/pypi/v/google-ads-marketingplatform-admin.svg
     :target: https://pypi.org/project/google-ads-marketingplatform-admin
.. |PyPI-google-cloud-media-translation| image:: https://img.shields.io/pypi/v/google-cloud-media-translation.svg
     :target: https://pypi.org/project/google-cloud-media-translation
.. |PyPI-google-apps-meet| image:: https://img.shields.io/pypi/v/google-apps-meet.svg
     :target: https://pypi.org/project/google-apps-meet
.. |PyPI-google-cloud-memorystore| image:: https://img.shields.io/pypi/v/google-cloud-memorystore.svg
     :target: https://pypi.org/project/google-cloud-memorystore
.. |PyPI-google-cloud-redis-cluster| image:: https://img.shields.io/pypi/v/google-cloud-redis-cluster.svg
     :target: https://pypi.org/project/google-cloud-redis-cluster
.. |PyPI-google-shopping-merchant-accounts| image:: https://img.shields.io/pypi/v/google-shopping-merchant-accounts.svg
     :target: https://pypi.org/project/google-shopping-merchant-accounts
.. |PyPI-google-shopping-merchant-conversions| image:: https://img.shields.io/pypi/v/google-shopping-merchant-conversions.svg
     :target: https://pypi.org/project/google-shopping-merchant-conversions
.. |PyPI-google-shopping-merchant-datasources| image:: https://img.shields.io/pypi/v/google-shopping-merchant-datasources.svg
     :target: https://pypi.org/project/google-shopping-merchant-datasources
.. |PyPI-google-shopping-merchant-lfp| image:: https://img.shields.io/pypi/v/google-shopping-merchant-lfp.svg
     :target: https://pypi.org/project/google-shopping-merchant-lfp
.. |PyPI-google-shopping-merchant-notifications| image:: https://img.shields.io/pypi/v/google-shopping-merchant-notifications.svg
     :target: https://pypi.org/project/google-shopping-merchant-notifications
.. |PyPI-google-shopping-merchant-ordertracking| image:: https://img.shields.io/pypi/v/google-shopping-merchant-ordertracking.svg
     :target: https://pypi.org/project/google-shopping-merchant-ordertracking
.. |PyPI-google-shopping-merchant-products| image:: https://img.shields.io/pypi/v/google-shopping-merchant-products.svg
     :target: https://pypi.org/project/google-shopping-merchant-products
.. |PyPI-google-shopping-merchant-promotions| image:: https://img.shields.io/pypi/v/google-shopping-merchant-promotions.svg
     :target: https://pypi.org/project/google-shopping-merchant-promotions
.. |PyPI-google-shopping-merchant-inventories| image:: https://img.shields.io/pypi/v/google-shopping-merchant-inventories.svg
     :target: https://pypi.org/project/google-shopping-merchant-inventories
.. |PyPI-google-shopping-merchant-reports| image:: https://img.shields.io/pypi/v/google-shopping-merchant-reports.svg
     :target: https://pypi.org/project/google-shopping-merchant-reports
.. |PyPI-google-shopping-merchant-reviews| image:: https://img.shields.io/pypi/v/google-shopping-merchant-reviews.svg
     :target: https://pypi.org/project/google-shopping-merchant-reviews
.. |PyPI-google-cloud-migrationcenter| image:: https://img.shields.io/pypi/v/google-cloud-migrationcenter.svg
     :target: https://pypi.org/project/google-cloud-migrationcenter
.. |PyPI-google-cloud-modelarmor| image:: https://img.shields.io/pypi/v/google-cloud-modelarmor.svg
     :target: https://pypi.org/project/google-cloud-modelarmor
.. |PyPI-google-cloud-netapp| image:: https://img.shields.io/pypi/v/google-cloud-netapp.svg
     :target: https://pypi.org/project/google-cloud-netapp
.. |PyPI-google-cloud-network-security| image:: https://img.shields.io/pypi/v/google-cloud-network-security.svg
     :target: https://pypi.org/project/google-cloud-network-security
.. |PyPI-google-cloud-network-services| image:: https://img.shields.io/pypi/v/google-cloud-network-services.svg
     :target: https://pypi.org/project/google-cloud-network-services
.. |PyPI-google-cloud-oracledatabase| image:: https://img.shields.io/pypi/v/google-cloud-oracledatabase.svg
     :target: https://pypi.org/project/google-cloud-oracledatabase
.. |PyPI-google-cloud-parallelstore| image:: https://img.shields.io/pypi/v/google-cloud-parallelstore.svg
     :target: https://pypi.org/project/google-cloud-parallelstore
.. |PyPI-google-cloud-parametermanager| image:: https://img.shields.io/pypi/v/google-cloud-parametermanager.svg
     :target: https://pypi.org/project/google-cloud-parametermanager
.. |PyPI-google-cloud-phishing-protection| image:: https://img.shields.io/pypi/v/google-cloud-phishing-protection.svg
     :target: https://pypi.org/project/google-cloud-phishing-protection
.. |PyPI-google-maps-places| image:: https://img.shields.io/pypi/v/google-maps-places.svg
     :target: https://pypi.org/project/google-maps-places
.. |PyPI-google-maps-areainsights| image:: https://img.shields.io/pypi/v/google-maps-areainsights.svg
     :target: https://pypi.org/project/google-maps-areainsights
.. |PyPI-google-cloud-policysimulator| image:: https://img.shields.io/pypi/v/google-cloud-policysimulator.svg
     :target: https://pypi.org/project/google-cloud-policysimulator
.. |PyPI-google-cloud-policytroubleshooter-iam| image:: https://img.shields.io/pypi/v/google-cloud-policytroubleshooter-iam.svg
     :target: https://pypi.org/project/google-cloud-policytroubleshooter-iam
.. |PyPI-google-cloud-private-catalog| image:: https://img.shields.io/pypi/v/google-cloud-private-catalog.svg
     :target: https://pypi.org/project/google-cloud-private-catalog
.. |PyPI-google-cloud-privilegedaccessmanager| image:: https://img.shields.io/pypi/v/google-cloud-privilegedaccessmanager.svg
     :target: https://pypi.org/project/google-cloud-privilegedaccessmanager
.. |PyPI-google-cloud-public-ca| image:: https://img.shields.io/pypi/v/google-cloud-public-ca.svg
     :target: https://pypi.org/project/google-cloud-public-ca
.. |PyPI-google-cloud-quotas| image:: https://img.shields.io/pypi/v/google-cloud-quotas.svg
     :target: https://pypi.org/project/google-cloud-quotas
.. |PyPI-google-cloud-rapidmigrationassessment| image:: https://img.shields.io/pypi/v/google-cloud-rapidmigrationassessment.svg
     :target: https://pypi.org/project/google-cloud-rapidmigrationassessment
.. |PyPI-google-cloud-recommendations-ai| image:: https://img.shields.io/pypi/v/google-cloud-recommendations-ai.svg
     :target: https://pypi.org/project/google-cloud-recommendations-ai
.. |PyPI-google-maps-routeoptimization| image:: https://img.shields.io/pypi/v/google-maps-routeoptimization.svg
     :target: https://pypi.org/project/google-maps-routeoptimization
.. |PyPI-google-cloud-run| image:: https://img.shields.io/pypi/v/google-cloud-run.svg
     :target: https://pypi.org/project/google-cloud-run
.. |PyPI-google-cloud-runtimeconfig| image:: https://img.shields.io/pypi/v/google-cloud-runtimeconfig.svg
     :target: https://pypi.org/project/google-cloud-runtimeconfig
.. |PyPI-sqlalchemy-bigquery| image:: https://img.shields.io/pypi/v/sqlalchemy-bigquery.svg
     :target: https://pypi.org/project/sqlalchemy-bigquery
.. |PyPI-google-cloud-securesourcemanager| image:: https://img.shields.io/pypi/v/google-cloud-securesourcemanager.svg
     :target: https://pypi.org/project/google-cloud-securesourcemanager
.. |PyPI-google-cloud-securitycentermanagement| image:: https://img.shields.io/pypi/v/google-cloud-securitycentermanagement.svg
     :target: https://pypi.org/project/google-cloud-securitycentermanagement
.. |PyPI-google-cloud-servicehealth| image:: https://img.shields.io/pypi/v/google-cloud-servicehealth.svg
     :target: https://pypi.org/project/google-cloud-servicehealth
.. |PyPI-google-shopping-merchant-quota| image:: https://img.shields.io/pypi/v/google-shopping-merchant-quota.svg
     :target: https://pypi.org/project/google-shopping-merchant-quota
.. |PyPI-google-shopping-type| image:: https://img.shields.io/pypi/v/google-shopping-type.svg
     :target: https://pypi.org/project/google-shopping-type
.. |PyPI-google-maps-solar| image:: https://img.shields.io/pypi/v/google-maps-solar.svg
     :target: https://pypi.org/project/google-maps-solar
.. |PyPI-google-cloud-storagebatchoperations| image:: https://img.shields.io/pypi/v/google-cloud-storagebatchoperations.svg
     :target: https://pypi.org/project/google-cloud-storagebatchoperations
.. |PyPI-google-cloud-storageinsights| image:: https://img.shields.io/pypi/v/google-cloud-storageinsights.svg
     :target: https://pypi.org/project/google-cloud-storageinsights
.. |PyPI-google-cloud-support| image:: https://img.shields.io/pypi/v/google-cloud-support.svg
     :target: https://pypi.org/project/google-cloud-support
.. |PyPI-google-cloud-telcoautomation| image:: https://img.shields.io/pypi/v/google-cloud-telcoautomation.svg
     :target: https://pypi.org/project/google-cloud-telcoautomation
.. |PyPI-google-cloud-vmwareengine| image:: https://img.shields.io/pypi/v/google-cloud-vmwareengine.svg
     :target: https://pypi.org/project/google-cloud-vmwareengine
.. |PyPI-google-cloud-video-stitcher| image:: https://img.shields.io/pypi/v/google-cloud-video-stitcher.svg
     :target: https://pypi.org/project/google-cloud-video-stitcher
.. |PyPI-google-cloud-visionai| image:: https://img.shields.io/pypi/v/google-cloud-visionai.svg
     :target: https://pypi.org/project/google-cloud-visionai
.. |PyPI-google-cloud-gsuiteaddons| image:: https://img.shields.io/pypi/v/google-cloud-gsuiteaddons.svg
     :target: https://pypi.org/project/google-cloud-gsuiteaddons
.. |PyPI-google-apps-events-subscriptions| image:: https://img.shields.io/pypi/v/google-apps-events-subscriptions.svg
     :target: https://pypi.org/project/google-apps-events-subscriptions
.. |PyPI-google-cloud-workstations| image:: https://img.shields.io/pypi/v/google-cloud-workstations.svg
     :target: https://pypi.org/project/google-cloud-workstations

.. API_TABLE_END

.. |ga| image:: https://img.shields.io/badge/support-GA-gold.svg
   :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#general-availability

.. |beta| image:: https://img.shields.io/badge/support-beta-orange.svg
   :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#beta-support


.. |alpha| image:: https://img.shields.io/badge/support-alpha-orange.svg
   :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#alpha-support


Example Applications
********************

-  `getting-started-python`_ - A sample and `tutorial`_ that demonstrates how to build a complete web application using Cloud Datastore, Cloud Storage, and Cloud Pub/Sub and deploy it to Google App Engine or Google Compute Engine.
-  `python-docs-samples`_ - Python samples for Google Cloud Platform products.

.. _getting-started-python: https://github.com/GoogleCloudPlatform/getting-started-python
.. _tutorial: https://cloud.google.com/python
.. _python-docs-samples: https://github.com/GoogleCloudPlatform/python-docs-samples


Authentication
********************


With ``google-cloud-python`` we try to make authentication as painless as possible.
Check out the `Getting started with authentication`_ in our documentation to learn more.

.. _Getting started with authentication: https://cloud.google.com/docs/authentication/getting-started



License
********************


Apache 2.0 - See `the LICENSE`_ for more information.

.. _the LICENSE: https://github.com/googleapis/google-cloud-python/blob/main/LICENSE
