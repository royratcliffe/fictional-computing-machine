# fictional-computing-machine

Template for VS Code development container using Docker from Docker Compose.
```bash
$ lsb_release -a
```
Gives you Debian 11 Bullseye Linux.

    No LSB modules are available.
    Distributor ID: Debian
    Description:    Debian GNU/Linux 11 (bullseye)
    Release:        11
    Codename:       bullseye

## Operation not permitted
You might find that you have to change file and directory ownership to `vscode`.
Sometimes the container creates `root`-owned i-nodes within the workspace. You
can revert ownership for all file-system nodes recursively using the following
shell command.
```bash
sudo chown -R vscode:vscode .
```
