# RunJava

## Description

`RunJava.sh` is a shell script designed to simplify the process of compiling and executing [Java](https://docs.oracle.com/en/java/) projects directly from the terminal. It searches for ***Java*** source files or packages, compiles them if necessary, and executes the main Java class.

## Get started

1. Clone the repository:
    ```bash
    git clone https://github.com/Gabriel-c0Nsp/RunJava.git
    ```

2. Navigate to the repository:
    ```bash
    cd RunJava
    ```

3. Make sure the script has executable permissions. If not, run the following command:
    ```bash
    chmod +x runjava.sh
    ```

4. Now you can execute the script using the following command:
    ```bash
    ./runjava.sh
    ```

## Recommendations
You can easily run this script by simply just typing `runjava` (or whatever you want) in your terminal, by setting an alias to your `.bashrc` or `.bash_profile`. If you're not using bash, you can search how to create aliases for you're specific shell.

First, you need to identify the current directory of the repository. This can be achieved with the following command:
   ```bash
   pwd
   ```
This output is important for the following process. The output of the `pwd` command is personal and will be referred in this documentation as `{current_directory}` for generalization purposes.

Finally, you can add the following instructions to your `.bashrc` or `.zshrc` file:

   ```bash
   export PATH=$PATH:{current_directory}/RunJava/
   alias runjava='runjava.sh'
   ```
Don't forget to change the path in the `export PATH=...` command as needed.

Now you can try the `runjava` command anywhere in your terminal and check the result.
