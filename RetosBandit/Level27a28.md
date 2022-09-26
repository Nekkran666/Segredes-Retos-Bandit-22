# Level 27a28

## Objetivo
There is a git repository at `ssh://bandit27-git@localhost/home/bandit27-git/repo`. The password for the user `bandit27-git` is the same as for the user `bandit27`.

## Datos de acceso
bandit27
YnQpBuifNMas1hcUFk70ZmqkhUU2EuaS
## Solucion
```bash
bandit27@bandit:~$ ls
bandit27@bandit:~$ cat /etc/bandit_pass/bandit27
YnQpBuifNMas1hcUFk70ZmqkhUU2EuaS
bandit27@bandit:~$ mkdir /tmp/solu
mkdir: cannot create directory ‘/tmp/solu’: File exists
bandit27@bandit:~$ mkdir /tmp/so
bandit27@bandit:~$ cd /tmp/so
bandit27@bandit:/tmp/so$ git clone ssh://bandit27-git@localhost/home/bandit27-git/repo
Cloning into 'repo'...
The authenticity of host 'localhost (127.0.0.1)' can't be established.
ED25519 key fingerprint is SHA256:C2ihUBV7ihnV1wUXRb4RrEcLfXC5CXlhmAAM/urerLY.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Could not create directory '/home/bandit27/.ssh' (Permission denied).
Failed to add the host to the list of known hosts (/home/bandit27/.ssh/known_hosts).

                      This is an OverTheWire game server.
            More information on http://www.overthewire.org/wargames

!!! You are trying to log into this SSH server on port 22, which is not intended.

bandit27-git@localhost: Permission denied (publickey).
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
```

## Notas adicionales
No me deja clonar el repositorio 

## Referencias

