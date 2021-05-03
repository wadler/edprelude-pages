# Inf1A-FP Haskell Installation

## 1. Installing Haskell
You may already have Haskell! That's excellent, you can skip right down to Step 2, installing EdPrelude. To check, open a terminal and type "`ghci --version`" to see if you have "`ghci`" already installed on your computer. If not, install by following the link below and picking the **correct version** for your OS (Windows, OS X for Mac, Linux). Choose the **minimal installation**.  
[https://www.haskell.org/downloads#minimal](https://www.haskell.org/downloads#minimal)  
After following those instructions, congratulations! You have Haskell.

## 2. Installing EdPrelude
With Haskell installed, you'll have a copy of Prelude, which is Haskell's standard library of useful functions. However, though Prelude is powerful, it is also complex. EdPrelude is an alternative version of Prelude, containing simple and straightforward definitions of the standard functions with a restricted set of available types. It also automatically derives a pretty-printer for data structures you specify, making it easier to read command-line output.

### Mac (OS X)/(UNIX) Instructions:
To install EdPrelude, follow the link below to get the zip file.  
[EdPrelude Download](https://github.com/wadler/edprelude/archive/refs/heads/main.zip)  
You should download a file named `e-prelude-master.zip`. Unzip this file, and navigate a terminal to the `e-prelude-master` folder (likely within your Downloads folder). At the terminal, within the folder, run the command below:  
`$ sudo ./install.sh` *(This command will require root access.)*  
If it succeeded without any errors, you should be done! As a test, run the following command from a new terminal:  
`$ edhci`  
It should open up an interactive REPL with EdPrelude loaded. As a further test, you can run the following command at the interactive prompt:  
`*EdPrelude> :type length`  
You should get back the following:  
`length :: [a] -> Integer`  
Demonstrating that you are using EdPrelude's definition of the length function compared to Prelude's.

### Uninstalling
If you ever want to uninstall EdPrelude, you can navigate to the same file (or re-download it if you've deleted it) and run the command below:  
`$ sudo ./uninstall.sh` *(This command will require root access.)* 

#### Updating EdPrelude:
To update EdPrelude, download the newest version from the link above, follow the instructions for installing again. You will be prompted before overwriting any of the old versions of files; confirm each overwrite to update.
