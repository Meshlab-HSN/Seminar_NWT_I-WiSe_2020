How to ssh login into your team VW:

Each team has a dedicated port to its VM:\
Meshlab_NWT1_2020

 team_ids        ssh port: 22100\
 team_ims        ssh port: 22101\
 team_iptv       ssh port: 22102\
 team_nms        ssh port: 22103\
 team_voip       ssh port: 22104\
 team_ip-failo.  ssh port: 22105\
 team_vlan       ssh port: 22106\
 team_rem-acc    ssh port: 22107


```ssh -l root -p my_team_Port 5.102.161.62 -i /User/Desktop/my_private_key```

In case you want to add another public key to your VM (from your team member), just add this new public ssh key to the authorized_key file with an editor of your choise:

```vim.tiny /root/.ssh/authorized_keys```
append a new line with the content of the public key you want to add & save file
