
Windows (PowerShell) version 

In the Visual Studio Code PowerShell terminal:

code --list-extensions > extensions.list

Machine B:

Copy extension.list to the machine B

In the Visual Studio Code PowerShell terminal:

 cat extensions.list |% { code --install-extension $_}
 
 For Ubuntu
 
 cat extensions.list | xargs -L 1 code --install-extension
