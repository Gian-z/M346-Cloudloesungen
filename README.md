# M346-Cloudloesungen
#readme #ops #tbz

## KN01
![p1](./KN01/Screenshot%202023-05-16%20102703.png)
![p2](./KN01/Screenshot%202023-05-16%20102746.png)
![p2](./KN01/Screenshot%202023-05-16%20102848.png)

## KN2

### a)
![324](./KN02/Screenshot%202023-05-23%20084738.png)
![234](./KN02/Screenshot%202023-05-23%20084823.png)
![](./KN02/Screenshot%202023-05-23%20084847.png)
*(Connection hat nicht funktioniert.)*

### b)
![](./KN02/Screenshot%202023-05-23%20092032.png)
![](./KN02/Screenshot%202023-05-23%20092012.png)
![](./KN02/Screenshot%202023-05-23%20091954.png)
![](./KN02/Screenshot%202023-05-23%20091934.png)

# B) -> SSH
![](./KN02/Pasted%20image%2020230523094146.png)
![](./KN02/Pasted%20image%2020230523094441.png)
![](./KN02/Pasted%20image%2020230523094535.png)

# C) -> YAML
```yaml
#cloud-config
users: # Liste von usen
  - name: ubuntu # Erstes Entry in der Liste (username ubuntu)
    sudo: ALL=(ALL) NOPASSWD:ALL # Sudocommands für diesen Benutzer
    groups: users, admin # Gruppenzuweisungen
    home: /home/ubuntu # Das Homeverzeichnis des Benutzers
    shell: /bin/bash # Shell configuration
    ssh_authorized_keys: # Mit dem Benutzer assoziierte SSH-Keys
      - ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQCibIsaqY7lwA3ZxLaFUT1/UroxYK35ptCX
2+pinj1jS9d60KuqiSWM2JmvwgijB3Wt7HhL2TfH6KdQAeNK1EIcUaxowkyVJlwk
35cr9DVEY5MH3te/rrZNyC4hUlvcwL/Ik2zFcVV5D9/J9ZlKWI/MKUY5shSmwz6V
PHdO+Ucfdlj8eLySYajlYXSE8ygml0tCO36c7p+WHfymKVWxMMhBTJ9QVFxzse/9
GUy12hNHDqRWyA84GfXaLDJTOSsPZb7skm5dS9FAESbyg+vRsVPx6pCLrCYkG4pY
zUg7HnzuAUFOAqPeX/oZRH3a1VsXrv+ydg7EE2PJ4hg23VyUK/E9 aws-key       
ssh_pwauth: false # Passwortauthorisierung per ssh
disable_root: false # Disable root login
package_update: true # Autoupdate von Packages
packages: # Packagereferenzen
  - curl 
  - wget
```
![](./KN02/Pasted%20image%2020230523103614.png)
![](./KN02/Pasted%20image%2020230523103821.png)
![](./KN02/Pasted%20image%2020230523103854.png)

# KN03
![](./KN03/Pasted%20image%2020230523113737.png)

