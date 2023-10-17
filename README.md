# Bito CLI
Bito CLI (Command Line Interface) provides a command line interface to the Bito AI chat functionality. Over time, CLI will add more functions and new command options to support complex automation and workflows.

This is a very early Alpha version. We would love to get your feedback on the new features or improvements.  Please write us at founders@bito.ai or support@bito.ai. 

#### Prerequisites
Terminal
* Bash (for Mac and Linux)
* CMD (for Windows)

## Using Bito CLI
- **Execute Chat:** Run ```bito``` command on command prompt to get started. Ask anything you want help with such as `awk command to print first and last column`.

    **Note:** Bito CLI supports long prompts through multiline input. To complete and submit the prompt, press `Ctrl+D`. Enter/Return key adds a new line to the input.
- **Exit Bito CLI:** To quit/exit from Bito CLI, type ```quit``` and press ```Ctrl+D``` .
- **Terminate:** Press ```Ctrl+C``` to Bito CLI.

### Getting Started
Check out the video below to get started with Bito CLI

https://user-images.githubusercontent.com/61789690/236821693-11705a17-e2a8-4f7c-8921-a47e75c81794.mp4

## Installing Bito CLI (Recommended)
We recommend you use the following methods to install Bito CLI.

### MAC and Linux

```sudo curl https://alpha.bito.ai/downloads/cli/install.sh -fsSL | bash``` (curl will always download the latest version)

#### Archlinux 

Arch and  Arch based distro users can install it from [AUR](https://aur.archlinux.org/packages/bito-cli)

``` yay -S bito-cli``` or ```paru -S bito-cli```


**Note for the Mac Users:** You might face issue related to verification for which you will have to manually do the steps from [here](https://support.apple.com/en-in/guide/mac-help/mh40616/mac) (we are working on fixing it as soon as possible).

### Windows

1. Install the Bito CLI through MSI using this [installer](https://github.com/gitbito/CLI/raw/main/version-3.5/Bito CLI.exe).
2. On Windows 11 you might get notification related to publisher verification. Click on "Show more" or "More info" and click on "Run anyway" (we are working on fixing this as soon as possbile).
3. Once the installation is complete, start a new command prompt and run ```bito``` to get started.

## Uninstalling Bito CLI

### MAC and Linux

```sudo curl https://alpha.bito.ai/downloads/cli/uninstall.sh -fsSL | bash``` (this will completely uninstall Bito CLI and all of its components)

### Windows

For Windows you can uninstall Bito CLI just like you do for any other software uninstall from control panel. You can still refer the link provided [here](https://sharestage.bito.co/static/share?aid=91940c09-0813-495d-9ea8-a89f1db19fdc).


## Installing with Manual Binary Download (Not Recommended)
While it's not recommended, you can download the Bito CLI binary from our repository, and install is manually. The binary is available for Linux and Mac OS, x86 and ARM architecture. 

### Mac & Linux

1. Download Bito CLI binary specific to your OS platform from [here](https://github.com/gitbito/CLI/tree/main/version-3.5) (Please download the latest version for all new updates).
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
- On MAC/Linux: 
run ```bito --help``` or ```bito config --help```

- On Windows: 
run ```bito --help``` or ```bito config --help```

#### Bito CLI MyPrompt (Automation using Bito CLI)
##### On MAC/Linux: 

- run ```bito -v``` or ```bito --version``` to print the version number of Bito CLI installed currently.

- run ```bito –p writedocprompt.txt -f mycode.js``` for non-interactive mode in Bito (where writedocprompt.txt will contain your prompt text such as "Explain the code below in brief" and mycode.js will contain the actual code on which the action is to be performed).

- run ```bito –p writedocprompt.txt``` to read the content at standard input in Bito (where writedocprompt.txt will contain your prompt text such as "Explain the code below in brief" and input provided will have the actual content on which the action is to be performed).

- run ```cat file.txt | bito``` to directly cat a file and pipe it to bito and get instant result for your query.

- run ```cat inventory.sql | bito -p testdataprompt.txt > testdata.sql``` to redirect your output directly to a file (where -p can be used along with cat to perform prompt related action on the given content).

- run ```cat inventory.sql | bito -c runcontext.txt -p testdataprompt.txt > testdata.sql``` to store context/conversation history in non-interactive mode in file `runcontext.txt` to use for next set of commands in case prior context is needed. If `runcontext.txt` is not present it will be created. Please provide a new file or an existing context file created by bito using `-c` option. ***With `-c` option now context is supported in non-interactive mode***

- run ```echo "give me code for bubble sort in python" | bito``` to instantly get response for your queries using Bito CLI.

##### On Windows: 
- run ```bito -v``` or ```bito --version``` to print the version number of Bito CLI installed currently.

- run ```bito –p writedocprompt.txt -f mycode.js``` for non-interactive mode in Bito (where writedocprompt.txt will contain your prompt text such as "Explain the code below in brief" and mycode.js will contain the actual code on which the action is to be performed).

- run ```bito –p writedocprompt.txt``` to read the content at standard input in Bito (where writedocprompt.txt will contain your prompt text such as "Explain the code below in brief" and input provided will have the actual content on which the action is to be performed).

- run ```type file.txt | bito``` to take input from file in windows and pipe it to bito and get instant result for your query.

- run ```type inventory.sql | bito -p testdataprompt.txt > testdata.sql``` to redirect your output directly to a file (where -p can be used along with type to perform prompt related action on the given content).

- run ```type inventory.sql | bito -c runcontext.txt -p testdataprompt.txt > testdata.sql``` to store context/conversation history in non-interactive mode in file `runcontext.txt` to use for next set of commands in case prior context is needed. If `runcontext.txt` is not present it will be created. Please provide a new file or an existing context file created by bito using `-c` option. ***With `-c` option now context is supported in non-interactive mode***

- run ```echo "give me code for bubble sort in python" | bito``` to instantly get response for your queries using Bito CLI.

##### Using Macro:

Use ``{{%input%}}`` macro in the prompt file to refer to the contents of the file provided via -f option

Example: To check if a file contains JS code or not, you can create a prompt file checkifjscode.txt with following prompt:
```
Context is provided below within contextstart and contextend
contextstart
{{%input%}}
contextend
Check if content provided in context is JS code.
```

#### Examples: 
Here are two examples for you to see My Prompt in action:

1. How to Create Git Commit Messages and Markdown Documentation with Ease using Bito CLI My Prompt:

[![Video](https://markdown-videos.vercel.app/youtube/q42hqwT-jsg)](https://www.youtube.com/watch?v=q42hqwT-jsg)

2. How to generate test data using Bito CLI My Prompt:

[![Video](https://markdown-videos.vercel.app/youtube/GYa0p511NUQ)](https://www.youtube.com/watch?v=GYa0p511NUQ)

### Bito CLI Configuration
#### bito config [flags]

- run ```bito config -l``` or ```bito config --list``` to list all config variables and values.

- run ```bito config -e``` or ```bito config --edit``` to open the config file in default editor.

#### Sample Configuration

bito:<br/>
&emsp;access_key: ""<br/>
&emsp;email: first.last@mycompany.com<br/>
&emsp;preferred_ai_model: ADVANCED<br/>
settings:<br/>
&emsp;auto_update: true<br/>
&emsp;max_context_entries: 20<br/>

##### Preferred AI Model Type
By default AI Model Type is set to ```ADVANCED``` and it can be overridden by running ```bito -m <BASIC/ADVANCED>```
Model type is used for AI query in the current session. Model type can be set to BASIC/ADVANCED, which is case insensitive.

##### Access Key
Access Key can be created at Bito Web UI and used in Bito CLI.

To create an access key, do the following:
- Login into your account at: https://alpha.bito.ai
- Once logged in open: https://alpha.bito.ai/home/settings/advanced
- Click on the "Create new key" button under section "Bito Access Key" to create a new key and copy it.
- Make sure to protect your key and do not check it in, into any code to avoid accidental leakage.
- In case you think your key is compromised, you can delete the existing key and create new key anytime.

Access Key is an alternate authentication mechanism to Email & OTP based aunthentication.


Access Key can be persisted in Bito CLI by running ```bito config -e```
Such persisted Access Key can be over-ridden by running ```bito -k <access-key>``` or ```bito --key <access-key>``` for the transient session.

## FAQs

### Enabling unicode For Windows 10 and below:
1. Unicode characters (using other languages) might not be readily supported on command prompt if you are on Windows 10 or below. You can run command ```chcp 936``` in cmd prior to using bito to support unicode characters in Windows 10 or below (To undo the settings done here you can follow this [link](https://share.bito.co/static/share?aid=8e535e57-d57f-4e03-a692-cf81a98fa6d2)).
2. IF you are on Windows 11 then you shouldn't encounter any such issues.

### Using Homebrew for Bito CLI:
1. Before using homebrew, please make sure that you uninstall any previously installed versions of Bito CLI using the uninstall script provided [here](https://github.com/gitbito/CLI#uninstalling-bito-cli).
2. Once above is done then you can use following commands to install Bito CLI using homebrew:
    - First tap the CLI repo using ```brew tap gitbito/bitocli```, this should be a one time action and not required every time.
    - Now you can install Bito CLI using following command:
        - ```brew install bito-cli``` - this should install Bito CLI based upon your machine architecture.
    - To update Bito CLI to the latest version, use following commands:
        - Please make sure you always do ```brew update``` before upgrading to avoid any errors.
        - ```brew update``` - this will update all the required packages before upgrading.
        - ```brew upgrade bito-cli``` - once above is done, this will update Bito CLI to the latest version.
    - To uninstall Bito CLI you can either use the uninstall command from [here](https://github.com/gitbito/CLI#uninstalling-bito-cli) or use following commands:
        - ```brew uninstall bito-cli``` - this should uninstall Bito CLI completely from your system.

## License ##

Copyright (C) 2021, Bito Inc - All Rights Reserved
