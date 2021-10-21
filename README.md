# fictional-computing-machine

## Operation not permitted
You might find that you have to change file and directory ownership to `vscode`.
Sometimes the container creates `root`-owned i-nodes within the workspace. You
can revert ownership for all file-system nodes recursively using the following
shell command.
```bash
sudo chown -R vscode:vscode .
```
