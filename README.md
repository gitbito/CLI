# Bito CLI
Bito CLI (Command Line Interface) provides a command line interface to the Bito AI chat functionality. Over time, CLI will add more functions and new command options to support complex automation and workflows.

This is a very early Alphas version. We would love to get your feedback on the new features or improvements.  Please write us at founders@bito.co or support@bito.co, 

#### Prerequisites
Terminal
* Bash (for Mac and Linux)
* CMD (for Windows)

## Using Bito CLI
- **Execute Chat:** Run ```bito``` command on command prompt to get started. Ask anything you want help with such as `awk command to print first and last column`.

    **Note:** Bito CLI supports long prompts through multiline input. To complete and submit the prompt, press `Ctrl+D`. Enter/Return key adds a new line to the input.
- **Exit Bito CLI:** To quit/exit from Bito CLI, type ```quit``` and press ```Ctrl+D``` .
- **Terminate:** Press ```Ctrl+C``` to Bito CLI..
## Installing Bito CLI (Recommended)
We recommend you use the following methods to install Bito CLI.

### MAC and Linux

```sudo curl https://alpha.bito.co/downloads/cli/install.sh -fsSL | bash``` (curl will always download the latest version)

**Note for the Mac Users:** You might face issue related to verification for which you will have to manually do the steps from [here](https://support.apple.com/en-in/guide/mac-help/mh40616/mac) (we are working on fixing it as soon as possible).

### Windows

1. Install the Bito CLI through MSI using this [installer](https://github.com/gitbito/CLI/raw/main/version-1.0/BitoCLI.msi).
2. On Windows 11 you might get notification related to publisher verification. Click on "Show more" or "More info" and click on "Run anyway" (we are working on fixing this as soon as possbile).
3. Once the installation is complete, start a new command prompt and run ```bito``` to get started.


## Installing with Manual Binary Download (Not Recommend)
While it's not recommended, you can download the Bito CLI binary from our repository, and install is manually. The binary is available for Linux and Mac OS, x86 and ARM architecture. 

### Mac & Linux

1. Download Bito CLI binary specific to your OS platform from [here](https://github.com/gitbito/CLI/tree/main/version-1.0) (Please download the latest version for all new updates).
2. Start the terminal, go to the location where your downloaded the binary, move the downloaded file (in the command below use bito-* filename you have downloaded) to filename bito
    ``` mv bito-<os>-<arch> bito ```
2. Make the file executable using following command
   ```chmod +x ./bito```
3. Copy the binary to /usr/local/bin using following command
    ```sudo cp ./bito /usr/local/bin```
4. Set PATH variable so that Bito CLI is always accessible.
    ```PATH=$PATH:/usr/local/bin```
5. Run Bito CLI with ```bito``` command. If PATH variable is not set, you will need to run command with the complete or relative path to the Bito executable binary. 
### Windows
1. For using bito CLI, always move to the directory containing bito CLI prior to running it.
2. Set PATH variable so that bito CLI is always accessible.
    * Follow the instructions as per this [link](https://share.bito.co/static/share?aid=02f4506f-1208-4d97-bb1d-96f3b4a1a017)
    * Edit the "Path" variable and add new path of the location where bito CLI is installed on your machine.


### Bito CLI Commands
#### help
- On MAC/Linux: run ```./bito --help``` or ```./bito config --help```
- On Windows: run ```bito --help``` or ```bito config --help```     
## License ##

Copyright (C) 2021, Bito Inc - All Rights Reserved
