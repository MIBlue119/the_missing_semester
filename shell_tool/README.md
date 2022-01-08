

## Resource
- [Bird brother's introduction to basic linux command](https://linux.vbird.org/linux_basic/redhat6.1/linux_06command.php)
- [Bird brother's introduction about the bash datatpipeline](http://linux.vbird.org/linux_basic_train/unit08.php)
- [The missing semester](https://missing.csail.mit.edu/)
    - [the shell](https://missing.csail.mit.edu/2020/course-shell/)
    - [shell tools and scripts](https://missing.csail.mit.edu/2020/shell-tools/)
- [unofficial-bash-strict-mode](http://redsymbol.net/articles/unofficial-bash-strict-mode/)
- [grep's regular expression](http://benjr.tw/97395)

## Tools
### Cheatsheet/Tutorial
- [tldr-pages](https://github.com/tldr-pages/tldr) : cheatsheets for console commands
    - It could support the practical use case for the console command. we don't need to open browser to find the commands.
    - How to install?
    ```
    $pip3 install tldr 
    ```
    - How to use?
    ```
    $ tldr the_command_you_want_to_search
    ```
- `man`: man(manual)the command built-in console provides the command introduction
    - How to use?
    ```
    $man the_command_you_want_to_search
    ```
    - Grep the specific patterns from the manaual results
        - Example: If i want to find the options `-h` for command `sort`?
        ```
        $man sort | grep -e "-h"
        ```
### Checker
- [shellcheck](https://github.com/koalaman/shellcheck): A static alanysis tool for shell script 
    - How to install?
    ```
    #At mac
    $brew install shellcheck
    #At linux
    $apt-get install shellcheck
    ```
    - It also equipped with some plugins for editor
        - [vscode-shellcheck](https://github.com/vscode-shellcheck/vscode-shellcheck)
    - we could use this to check at our CI pipeline
        - Example: [shell check at linting](https://github.com/full-stack-deep-learning/fsdl-text-recognizer-2021-labs/blob/174ebbdc065442175d9457b7a97d6e065f3d9cd0/lab8/tasks/lint.sh#L33)
        ```
        find . -name "*.sh" -print0 | xargs -0 shellcheck || FAILURE=true
        ```