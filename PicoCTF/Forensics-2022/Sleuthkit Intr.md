# Sleuthkit Intr

## Descripcion
Download the disk image and use `mmls` on it to find the size of the Linux partition. Connect to the remote checker service to check your answer and get the flag. Note: if you are using the webshell, download and extract the disk image into `/tmp` not your home directory.

-   [Download disk image](https://artifacts.picoctf.net/c/114/disk.img.gz)
-   Access checker program: `nc saturn.picoctf.net 52279`

## Pistas
```bash
                                                                                                                  
┌──(kali㉿kali)-[~/PicoCTF/forensic2022/slk]
└─$ ls 
disk.img.gz
                                                                                                                   
┌──(kali㉿kali)-[~/PicoCTF/forensic2022/slk]
└─$ gzip -d disk.img.gz   
                                                                                                                   
┌──(kali㉿kali)-[~/PicoCTF/forensic2022/slk]
└─$ ls -la
total 102408
drwxr-xr-x 2 kali kali      4096 Oct 24 22:33 .
drwxr-xr-x 3 kali kali      4096 Oct 24 22:32 ..
-rw-r--r-- 1 kali kali 104857600 Mar 15  2022 disk.img
                                                                                                                   
┌──(kali㉿kali)-[~/PicoCTF/forensic2022/slk]
└─$ mmls -v  
Missing image name
mmls [-i imgtype] [-b dev_sector_size] [-o imgoffset] [-BrvV] [-aAmM] [-t vstype] image [images]
        -t vstype: The type of volume system (use '-t list' for list of supported types)
        -i imgtype: The format of the image file (use '-i list' for list supported types)
        -b dev_sector_size: The size (in bytes) of the device sectors
        -o imgoffset: Offset to the start of the volume that contains the partition system (in sectors)
        -B: print the rounded length in bytes
        -r: recurse and look for other partition tables in partitions (DOS Only)
        -v: verbose output
        -V: print the version
Unless any of these are specified, all volume types are shown
        -a: Show allocated volumes
        -A: Show unallocated volumes
        -m: Show metadata volumes
        -M: Hide metadata volumes
                                                                                                                   
┌──(kali㉿kali)-[~/PicoCTF/forensic2022/slk]
└─$ mmls disk.img 
DOS Partition Table
Offset Sector: 0
Units are in 512-byte sectors

      Slot      Start        End          Length       Description
000:  Meta      0000000000   0000000000   0000000001   Primary Table (#0)
001:  -------   0000000000   0000002047   0000002048   Unallocated
002:  000:000   0000002048   0000204799   0000202752   Linux (0x83)
                                                                                                                   
┌──(kali㉿kali)-[~/PicoCTF/forensic2022/slk]
└─$ ^[[200~nc saturn.picoctf.net 52279~
zsh: bad pattern: ^[[200~nc
                                                                                                                   
┌──(kali㉿kali)-[~/PicoCTF/forensic2022/slk]
└─$ nc saturn.picoctf.net 52279 
What is the size of the Linux partition in the given disk image?
Length in sectors: 202752 
202752
Great work!
picoCTF{mm15_f7w!}

```


## Solucion 

## Notas Adicionales

## Referencias