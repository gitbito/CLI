# Bito CLI
Bito CLI (Command Line Interface) provides a command line interface to the Bito AI chat functionality. Over time, CLI will add more functions and new command options to support complex automation and workflows.

The CLI is in alpha.  We're excited to have you try it out.  Please send us your feedback at founders@bito.co or support@bito.co, we'd love to hear about bugs, feature requests, or any ideas you have!

#### Prerequisites

Terminal
* Bash (for Mac and Linux)
* CMD (for Windows)

## Using Bito CLI
- **Execute Chat:** Run ```bito``` command on command prompt to get started. Now type anything you want help with such as `awk command to print first and last column`.

    **Note:** Bito CLI supports multiline input so you can give long form prompts. To complete and submit the prompt, press `Ctrl+D`. Enter/return key adds a new line to the input.
- **Exit Bito CLI:** To quit/exit from Bito CLI, type ```quit``` and press ```Ctrl+D``` .
- **Terminate:** Press ```Ctrl+C``` to Bito CLI..
## Installing/downloading Bito CLI

**Download And Install Using Curl (Mac/Linux)** Recommended

```sudo curl https://alpha.bito.co/downloads/cli/install.sh -fsSL | bash``` (curl will always download the latest version)

**MSI Package (for Windows)** Recommended

1. Install the Bito CLI using this [installer](https://github.com/gitbito/CLI/raw/main/version-1.0/BitoCLI.msi).
2. On Windows 11 you might get notification related to publisher verification. Click on "Show more" or "More info" and click on "Run anyway" (we are working on fixing this as soon as possbile).
3. Once the installation is complete, start a new command prompt and run ```bito``` to get started.

**Manual Binary Download**
1. Download Bito CLI binary specific to your OS platform from [here](https://github.com/gitbito/CLI/tree/main/version-1.0) (Please download the latest version for all new updates).

## MacOS specific note:
After downloading the CLI for Mac you might face issues related to verification for which you will have to manually do the steps from [here](https://support.apple.com/en-in/guide/mac-help/mh40616/mac) (we are working on fixing it as soon as possible).

## Manual Install (In case you downloaded binaries directly)
### On Mac/Linux
1. Start the terminal and go to location where bito CLI was downloaded and move the downloaded file (in the command below use bito-* filename you have downloaded) to filename bito
    ``` mv bito-<os>-<arch> bito ```
2. Make the file executable using following command
   ```chmod +x ./bito```
3. Copy the bito CLI binary to /usr/local/bin using following command
    ```sudo cp ./bito /usr/local/bin```
4. Set PATH variable so that bito CLI is always accessible.
    ```PATH=$PATH:/usr/local/bin```
### On Windows
1. For using bito CLI, always move to the directory containing bito CLI prior to running it.
2. Set PATH variable so that bito CLI is always accessible.
    * Follow the instructions as per this [link](https://share.bito.co/static/share?aid=02f4506f-1208-4d97-bb1d-96f3b4a1a017)
    * Edit the "Path" variable and add new path of the location where bito CLI is installed on your machine.

## Running Bito CLI
### For Mac/Linux
1. If you have followed steps for intall then run
    ```bito```
2. In case you did not follow the steps for install, just go to directory where bito CLI is downloaded and run ```./bito``` or run ```./<path-to-bito>/bito``` where path-to-bito should be replaced with relative or complete path to access bito CLI
### For Windows
1. In case you have followed recommended steps for install then open CMD/Terminal and run
    ```bito```
2. In case you did not follow the recommended steps for install, go to the folder where bito CLI was downloaded in terminal/CMD and run ```bito```

### Other CLI options
#### help
- On MAC/Linux: run ```./bito --help``` or ```./bito config --help```
- On Windows: run ```bito --help``` or ```bito config --help```     
## License ##

Copyright (C) 2021, Bito Inc - All Rights Reserved
