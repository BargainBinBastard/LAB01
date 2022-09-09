b 02

- Name: Robert Croop
- Email: croop.2@wright.edu

## Part 1 Answers

The answers for this section are to help you record what steps  
are needed to create a file locally (in your cloned repo)  
and push them (sync) with GitHub

1. Add a file for tracking:  "git add [filename]
2. Commit changes: git commit [filename]
3. Sync local commits with GitHub: git push [filename]

## Part 2 Answers

For each, write the command used or answer the question posed.

1. sudo adduser bob
2. /home/bob
3. no, no permission
4. su bob (then enter password)
5. cd bob
6. yes, he has permission
7. exit
8. cd ubuntu

## Part 3 Answers

For each, write the command used or answer the question posed.

1. sudo addgroup crew
2. sudo usermod -a -G crew bpb, sudo usermod -a -G crew ubuntu
3. sudo chgrp Crew DirA
4. su bob
5. touch testfile.txt
6. because bob was part of the group that owns the folder

## Part 4 Answers

For each, write the command used or answer the question posed.

1. sudo touch sudowho.txt
2. It has read and writerpermissions for the owner, and read permissions for group and other. Notably, the owner, unlike that of all other files, is "root".
3. vim sudowho.txt (Gave me a warning that I was "modifying a read-only file", but modification seems to have worked regardless. Strange.)

## Part 5 Answers

1. `ssh` command before configuring `config` file: ssh -i labuser.pem ubuntu@44.211.102.140
2. HostName: 44.211.102.140
3. User: BargainBinBastard
4. IdentityFile:/home/bargainbinbastard/labuser.pem
5. `~/.ssh/config` contents:

```
Host aws
        HostName 44.211.102.140
        User ubuntu
        IdentityFile ~/labuser.pem
```

6. `ssh` command after configuring `config` file: ssh aws
