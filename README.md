# shell_extensions
Storing my own alias and shell scripts to make life easier

## Add path to shell
To load these on start of terminal I do the following
```
extensions_path="path_to_shell_extensions_repo"

[ -f "$extensions_path/.zsh_aliases" ] && source $extensions_path/.zsh_aliases && echo "Aliases Loaded"
[ -f "$extensions_path/.zsh_git" ] && source $extensions_path/.zsh_git && echo "GIT Aliases Loaded"
[ -f "$extensions_path/.zsh_kubernetes" ] && source $extensions_path/.zsh_kubernetes && echo "Kubernetes Aliases Loaded"
[ -f "$extensions_path/.zsh_mix" ] && source $extensions_path/.zsh_mix && echo "Mix Aliases Loaded"
```

## Useful environment variables
*KUBE_EXEC_POD_NAME_MATCH_DEFAULT* - default pod name you want to use for executing commands
*KUBE_REMOTE_COMMAND_DEFAULT* - default command to execute if none is supplied
*KUBE_DB_POD_NAME_MATCH_DEFAULT* - default pod name you want to use for the database
*KUBE_DB_PORT_DEFAULT* - default remote port number for you database
*KUBE_PORT_FORWARD_DEFAULT* - default local port number you want to forward to 
