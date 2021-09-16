'''yacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$  man mkdir
'''vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ mkdir ABC
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ ls
ABC  Desktop  Documents  Downloads  Music  Pictures  Public  Templates  Videos
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ ls -l
total 36
drwxrwxr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep 16 10:43 ABC
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Desktop
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Documents
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Downloads
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Music
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep 12 12:18 Pictures
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Public
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Templates
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Videos
'''vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ pwd
/home/vyacheslavurbuntu
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ tree

Command 'tree' not found, but can be installed with:

sudo snap install tree  # version 1.8.0+pkg-3fd6, or
sudo apt  install tree  # version 1.8.0-1

See 'snap info tree' for additional versions.

vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ root

Command 'root' not found, but can be installed with:

sudo snap install root-framework

vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ tree

Command 'tree' not found, but can be installed with:

sudo snap install tree  # version 1.8.0+pkg-3fd6, or
sudo apt  install tree  # version 1.8.0-1

See 'snap info tree' for additional versions.

vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ cd ABC
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~/ABC$ pwd
/home/vyacheslavurbuntu/ABC
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~/ABC$ cd home
bash: cd: home: No such file or directory
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~/ABC$ cd /home/^C
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~/ABC$ cd /home/vyacheslavurbuntu
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ ls -l
total 36
drwxrwxr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep 16 10:43 ABC
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Desktop
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Documents
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Downloads
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Music
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep 12 12:18 Pictures
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Public
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Templates
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Videos
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ ls -a
.              .bash_logout  Desktop    .local    .profile   .thunderbird
..             .bashrc       Documents  .mozilla  Public     Videos
ABC            .cache        Downloads  Music     .ssh
.bash_history  .config       .gnupg     Pictures  Templates
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ cd ABC
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~/ABC$ ls -l
total 0
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~/ABC$ ls -a
.  ..
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~/ABC$ cd ..
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ cd ..
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:/home$ cd ..
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:/$ pwd
/
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:/$ cd /hopme
bash: cd: /hopme: No such file or directory
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:/$ cd /home
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:/home$ pwd
/home
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:/home$ cd ..
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:/$ cd ..
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:/$ cd ..
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:/$ whoami
vyacheslavurbuntu
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:/$ ls
bin    dev   lib    libx32      mnt   root  snap      sys  var
boot   etc   lib32  lost+found  opt   run   srv       tmp
cdrom  home  lib64  media       proc  sbin  swapfile  usr
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:/$ ls -l
total 459344
lrwxrwxrwx   1 root root         7 sep  4 11:45 bin -> usr/bin
drwxr-xr-x   4 root root      4096 sep  4 11:55 boot
drwxrwxr-x   2 root root      4096 sep  4 11:47 cdrom
drwxr-xr-x  20 root root      4080 sep 16 10:40 dev
drwxr-xr-x 130 root root     12288 sep  4 11:55 etc
drwxr-xr-x   3 root root      4096 sep  4 11:47 home
lrwxrwxrwx   1 root root         7 sep  4 11:45 lib -> usr/lib
lrwxrwxrwx   1 root root         9 sep  4 11:45 lib32 -> usr/lib32
lrwxrwxrwx   1 root root         9 sep  4 11:45 lib64 -> usr/lib64
lrwxrwxrwx   1 root root        10 sep  4 11:45 libx32 -> usr/libx32
drwx------   2 root root     16384 sep  4 11:45 lost+found
drwxr-xr-x   2 root root      4096 aug 19 13:29 media
drwxr-xr-x   2 root root      4096 aug 19 13:29 mnt
drwxr-xr-x   2 root root      4096 aug 19 13:29 opt
dr-xr-xr-x 231 root root         0 sep 16 10:39 proc
drwx------   4 root root      4096 sep  4 11:50 root
drwxr-xr-x  29 root root       780 sep 16 10:40 run
lrwxrwxrwx   1 root root         8 sep  4 11:45 sbin -> usr/sbin
drwxr-xr-x   8 root root      4096 aug 19 13:48 snap
drwxr-xr-x   2 root root      4096 aug 19 13:29 srv
-rw-------   1 root root 470287360 sep  4 11:45 swapfile
dr-xr-xr-x  13 root root         0 sep 16 10:39 sys
drwxrwxrwt  18 root root      4096 sep 16 11:03 tmp
drwxr-xr-x  14 root root      4096 aug 19 13:32 usr
drwxr-xr-x  14 root root      4096 aug 19 13:47 var
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:/$ cd /home
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:/home$ pwd
/home
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:/home$ cd /home/vyacheslavurbuntu
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ pwd
/home/vyacheslavurbuntu
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ ls -l
total 36
drwxrwxr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep 16 10:43 ABC
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Desktop
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Documents
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Downloads
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Music
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep 12 12:18 Pictures
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Public
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Templates
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Videos
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ cd /home
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:/home$ tree

Command 'tree' not found, but can be installed with:

sudo snap install tree  # version 1.8.0+pkg-3fd6, or
sudo apt  install tree  # version 1.8.0-1

See 'snap info tree' for additional versions.

vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:/home$ cd /home/vyacheslavurbuntu
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ cd /
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:/$ cd ¬
bash: cd: ¬: No such file or directory
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:/$ cd /home/vyacheslavurbuntu
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ touch a.txt
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ ls
ABC    Desktop    Downloads  Pictures  Templates
a.txt  Documents  Music      Public    Videos
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ ls -lt
total 36
-rw-rw-r-- 1 vyacheslavurbuntu vyacheslavurbuntu    0 sep 16 11:12 a.txt
drwxrwxr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep 16 10:43 ABC
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep 12 12:18 Pictures
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Desktop
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Documents
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Downloads
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Music
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Public
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Templates
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Videos
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ cat a.txt
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ echo

vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ man echo
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ echo 12345> b.txt
bash: 12345: Bad file descriptor
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ echo 12345 > a.txt
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ echo 12345 > b.txt
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ ls -l
total 44
drwxrwxr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep 16 10:43 ABC
-rw-rw-r-- 1 vyacheslavurbuntu vyacheslavurbuntu    6 sep 16 11:17 a.txt
-rw-rw-r-- 1 vyacheslavurbuntu vyacheslavurbuntu    6 sep 16 11:18 b.txt
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Desktop
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Documents
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Downloads
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Music
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep 12 12:18 Pictures
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Public
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Templates
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Videos
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ cat b.txt
12345
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ cat a.txt
12345
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ echo 2 > c.txt
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ ls -l
total 48
drwxrwxr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep 16 10:43 ABC
-rw-rw-r-- 1 vyacheslavurbuntu vyacheslavurbuntu    6 sep 16 11:17 a.txt
-rw-rw-r-- 1 vyacheslavurbuntu vyacheslavurbuntu    6 sep 16 11:18 b.txt
-rw-rw-r-- 1 vyacheslavurbuntu vyacheslavurbuntu    2 sep 16 11:23 c.txt
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Desktop
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Documents
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Downloads
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Music
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep 12 12:18 Pictures
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Public
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Templates
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Videos
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ hexdump -C a.txt
00000000  31 32 33 34 35 0a                                 |12345.|
00000006
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ echo 67890 > b.txt
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ ls -lt
total 48
-rw-rw-r-- 1 vyacheslavurbuntu vyacheslavurbuntu    6 sep 16 11:26 b.txt
-rw-rw-r-- 1 vyacheslavurbuntu vyacheslavurbuntu    2 sep 16 11:23 c.txt
-rw-rw-r-- 1 vyacheslavurbuntu vyacheslavurbuntu    6 sep 16 11:17 a.txt
drwxrwxr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep 16 10:43 ABC
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep 12 12:18 Pictures
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Desktop
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Documents
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Downloads
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Music
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Public
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Templates
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Videos
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ cat b.txt
67890
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ hexdump -C b.txt
00000000  36 37 38 39 30 0a                                 |67890.|
00000006
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ echo abcd > c.txt
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ ls -lt
total 48
-rw-rw-r-- 1 vyacheslavurbuntu vyacheslavurbuntu    5 sep 16 11:27 c.txt
-rw-rw-r-- 1 vyacheslavurbuntu vyacheslavurbuntu    6 sep 16 11:26 b.txt
-rw-rw-r-- 1 vyacheslavurbuntu vyacheslavurbuntu    6 sep 16 11:17 a.txt
drwxrwxr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep 16 10:43 ABC
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep 12 12:18 Pictures
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Desktop
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Documents
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Downloads
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Music
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Public
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Templates
drwxr-xr-x 2 vyacheslavurbuntu vyacheslavurbuntu 4096 sep  4 11:52 Videos
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ cat c.txt
abcd
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ hexdump -C c.txt
00000000  61 62 63 64 0a                                    |abcd.|
00000005
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ nano b.txt
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ nano b.txt
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$ cat b.txt
Hello the world !!!
vyacheslavurbuntu@vyacheslavurbuntu-VirtualBox:~$
