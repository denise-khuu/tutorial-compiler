
# Structure

## Repositories

    |--tutorial-compiler
    |--tutorials

## Tutorials

    |-- tutorials
        |-- [playbook-name]
            /--index.asciidoc

Write your own tutorials in "./tutorials/[playbook-name]/index.asciidoc".
You will find all the details in the tutorials [Developement](https://github.com/devonfw-forge/tutorials/wiki/Development) page.

## Commands

### Runners

    |-- tutorial-compiler
        |--runners
            |--[runner]
                /--index.ts

**runner**
* console
* katacoda
* vscode
* wikiConsole 
* wikiEclipse
* wikiEditor

Create your own commands as shown in tutorial-compilers's [Developement](https://github.com/devonfw-forge/tutorials/wiki/Development) page inside the "./index.ts"-files.

### Assertions 

    |--tutorial-compiler
        |--assertions

Add assertions by adding a new class into the "./tutorial-compiler/assertions"-folder 
Learn more about it in [Development](https://github.com/devonfw-forge/tutorials/wiki/Development)

## Workspace

### Workspace without Devonfw IDE  
    |-- tutorial-compiler
        |--build
            |--working

The default workspace is "./tutorial-compiler/build/working". 
The console runner will run all commands inside the working folder.
You will find in the [Functions](https://github.com/devonfw-forge/tutorial-compiler/wiki/Functions) page the phrase "relative to workspace", which means relative to "./working".
You can set a new workspace with the function [changeWorkspace](https://github.com/devonfw-forge/tutorial-compiler/wiki/Functions).

### Workspace with Devonfw IDE 

    |-- tutorial-compiler
        |--build
            |--working
                |--devonfw
                    |--workspaces
                        |--main

The functions 
* [restoreDevonfwIde](https://github.com/devonfw-forge/tutorial-compiler/wiki/Functions)
* [installDevonfwIde](https://github.com/devonfw-forge/tutorial-compiler/wiki/Functions)

will change the workspace to the "./tutorial-compiler/build/working/devonfw/workspaces/main".
The phrase "relative to workspace" means in this case relative to "./main"
You can set a new workspace with the function [changeWorkspace](https://github.com/devonfw-forge/tutorial-compiler/wiki/Functions).


## Katacoda tutorials

    |-- tutorial-compiler
        |--build
            |--output
                |--katacoda
                    |--[playbook-name]

You can find the generated katacoda tutorial inside "./tutorial-compiler/build/output/katacoda/[playbook-name]"
You can copy the whole folder to add it to you katacoda ropository.