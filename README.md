# Prep kali for HTB or THM
Kali zsh file with extra vpn shell files for adding IP in PS1 header.

## Prompt string to be modified
```
PROMPT=$'%F{%(#.blue.green)}┌──${debian_chroot:+($debian_chroot)──}$(/opt/vpnbash.sh)(%B%F{%(#.red.blue)}%n%(#.💀.@)%m%b%F{%(#.blue.green)})-[%B%F{reset}%(6~.%-1~/…/%4~.%5~)%b%F{%(#.blue.green)}]\n└─%B%(#.%F{red}#.%F{blue}$)%b%F{reset} '
```
## Placing VPN*.sh files
For this to work you have to place the `vpn*.sh` file in the folder `/opt`

## Once all done
```
source ~/.zshrc
```
