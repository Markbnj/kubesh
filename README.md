# kubesh
A bash script to create a useful shell environment for working with kubernetes using kubectl. Modifies the prompt to include the current context name to make it easy to know what cluster you're working on, and also provides several convenience functions to make it easy to switch between contexts.

![kubesh](kubesh_cast.gif)

## Use

Just copy the `kubesh` script somewhere on your path and mark it executable (`chmod 755 kubesh`). Then run the script to create the shell environment. Requires kubectl and sed.

```
NAME
  kubesh - sets up a shell environment for kubernetes kubectl tool with a
  number of useful commands.

SYNOPSIS
  kubesh [-h] [-n]

DESCRIPTION
  Kubesh displays the current kubernetes context in the shell prompt and adds
  some commands to make it easier to switch between contexts. Run kubesh and
  type 'help' at the shell prompt for more information on commands.

OPTIONAL ARGUMENTS
  -n
    Start with the context prompt disabled.
  -h
    Display this help. All other arguments are ignored.
```

## History

  - 0.1.0 (4/17/2017): initial release
  - 0.2.0 (4/19/2017): added ability to toggle the prompt display on/off
  - 0.2.1 (4/19/2017): sourced .bashrc in subshell so aliases would work
  - 0.2.2 (4/22/2017): handle the case where no kubectl context exists at start
  - 0.3.0 (4/27/2017): now watched the kubeconfig for external changes and reboots the shell

## PR's welcome!
