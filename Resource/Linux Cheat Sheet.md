# Linux Cheat Sheet
## Working with Files
1. Print working directory
> pwd

2. List directory contents;
> ls [options] [file ...]

options:

>ls -a

Show all file

>ls -l

List in long format, that will show a message as:
>-rwxr-xr-x  1 user  staff  33432 Mar 11 13:11 hello

The first character should be '-', 'd', '-' means it's a normal file, 'd' means it's a directory;<br>
After that is three group of 'rwx', represents the current user permissions, user group permissions and other user permissions respectively. 'r' means have read permission, 'w' means have write or modify permission, 'x' means execute permission. These can also present by numbers, 'r' = 4, 'w' = 2, 'x' = 1, for example, 'rwxr-xr-x' = 755. <br>
Then user and user group, file size, last modify time and file name.<br>


>ls -S

Sort by size, largest first

>ls -t

Sort by time modified, most recent first

>ls -r

Reverse sort order

3. Change working directory
>cd [dir]

shortcuts:<br>
>cd .

Current directory

>cd ..

Parent directory

>cd ~

Your home directory

>cd ~user

User's home directory

3. Make directory
>mkdir directory ...

4. Rename source to target
>mv source target

5. Relocate each source into directory
>mv source ... directory

6. Copy each source into target
>cp [options] source ... target

7. Remove each file
>rm [options] file ...

Options:
> rm -d [file]

Remove empty directories

> rm -r [file]

Remove files and directories recursively

> rm -f [file]

Do not prompt for confirmation, <p color='red'>DANGEROUS</p>