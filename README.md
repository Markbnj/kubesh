# kubesh
A bash script to create a useful shell environment for working with kubernetes using kubectl. Modifies the prompt to include the current context name to make it easy to know what cluster you're working on, and also provides several convenience functions to make it easy to switch between contexts.

## Use

Just copy the `kubesh` script somewhere on your path and mark it executable (`chmod 755 kubesh`). Then run the script to create the shell environment. Requires kubectl and sed.

PR's welcome!
