# HTB or THM Tunnel IP in promt line same as pwnbox from HTB
Kali zsh file with extra vpn shell files for adding IP in PS1 header.
The VPN files are originally from https://github.com/theGuildHall/pwnbox but have been modified to integrate into the kali zsh shell.

## Prompt string to be modified
```
PROMPT=$'%F{%(#.blue.green)}┌──${debian_chroot:+($debian_chroot)──}$(/opt/vpnbash.sh)(%B%F{%(#.red.blue)}%n%(#.💀.㉿)%m%b%F{%(#.blue.green)})-[%B%F{reset}%(6~.%-1~/…/%4~.%5~)%b%F{%(#.blue.green)}]\n└─%B%(#.%F{red}#.%F{blue}$)%b%F{reset} '
```
## Placing VPN*.sh files
For this to work you have to place the `vpn*.sh` file in the folder `/opt`

## Once all done
```
source ~/.zshrc
```
![image](https://user-images.githubusercontent.com/3829939/114279840-e1139300-9a36-11eb-9829-e750cae06df3.png)
