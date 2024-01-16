# Lab Report 1

## cd command
* __No arguments__
  
  ![Image](cd-no-args.png)
  
  Directory: root

  Running `cd` without any arguments results in the terminal path being reset to the home directory. This behavior is intentional and is meant to be used to reset the terminal working location.

  This is not an error.
* __Directory argument__

  ![Image](cd-direc-arg.png)
  
  Directory: root

  Running `cd` with a directory argument does excactly what it is defined to do and directs the terminal in the direction of directory argument provided. Any commands given will now take place in the directory provided unless `cd` is called again pointing the terminal to another direction.

  This is not an error.
* __File Argument__

  ![Image](cd-file-arg.png)

  Directory: /lecture1

  Running `cd` with a file argument is not a valid command and will result in no change.

  This is an error as the `cd` command expects a directory as an argument.
## ls command
* __No arguments__

  ![Image](ls-no-args.png)
  
  Directory: root

  Running `ls` with no arguments will list the contents of the current directory.

  This is not an error.
* __Directory argument__

  ![Image](ls-direc-arg.png)
  
  Directory: root

  Running `ls` with a directory as an arugment will list the contents inside of that directory. The directory path will remain the same and does not change like the `cd` command.

  This is not an error.
* __File Argument__

  ![Image](ls-file-arg.png)
  
  Directory: root

  Running the `ls` command on a file argument does not operate like the other ls commands and instead lists the information of the file. In this case, running the `ls` command returns the file path of the file passed as an argument.

## cat command
* __No arguments__

  ![Image](cat-no-args.png)

  Directory: root
* __Directory argument__

  ![Image](cat-direc-arg.png)

  Directory: root
* __File Argument__

  ![Image](cat-file-arg.png)

  Directory: root
