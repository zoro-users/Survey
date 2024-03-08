# Survey


# Google docs link 
(https://docs.google.com/document/d/1gFsyIt4kbwtvTkdLef_t4nID6iTsrGoWtJKwfnVXlQE/edit?usp=sharing)

# we transfer link

https://we.tl/t-7lxl36siV0

# Edge install

Install Microsoft Edge on RHEL 9 and derivatives
As you can imagine, Edge is not present in the official repositories of RHEL 9 and therefore of any derivative of it. However, this does not make it difficult to install, on the contrary it is simple.

First, open a terminal and update the entire system
```
sudo dnf update
```
Then, install a package needed to add repositories without any problem
```
sudo dnf install dnf-utils
```
As a rule, the above command is already installed by default, but it is better to be certain.

As Edge is not in the official RHEL 9 repositories, then you have to add an external one. The good thing is that it is from Microsoft, so we can be confident that it is not malicious.

To do this run:
```
sudo dnf config-manager --add-repo https://packages.microsoft.com/yumrepos/edge
```
Then, add the GPG key of the same one
```
sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
```
Then refresh the repositories
```
sudo dnf update
```
And finally, install Microsoft Edge on RHEL 9 and derivatives with this command
```
sudo dnf install microsoft-edge-stable
```
Pass the Blue color cmds in the terminal... 
