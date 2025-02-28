## Linux Commands

#### Change Directory:

We use the command `cd` for change the directory of our terminal. Like below:

```sh
cd /home/abc
```

#### List all files:

If we want to see all file on a directory then we can use the `ls` command. The example are given below:

```sh
ls -a #for see all file include hidden files
```

```sh
ls -l #It displays all kind of information like permission, owner, size and modification
```

#### Symlink:

There are two type of symlink. They are:

- Soft Link
- Hard Link

**Soft Link:** Soft link are loosely connected with file. If the main file are renamed or delete then the symlink are broken if we make the symlink with Soft Link. For making the command a demo command are given below:

```sh
ln -s <Path of main file> <name of linking file>
```

**Hard Link:** If we want to link a file strongly then we have to use the hard Link. We do whatever like delete, rename or anything the Hard Link are not broken.A demo command are given below:

```sh
ln  <Path of main file> <name of linking file>
```

#### System Information:

**See All System Information:** `uname -a` return the whole system information. The information are like below:

```sh
Linux sakib-virtual-machine 6.8.0-52-generic #53-Ubuntu SMP PREEMPT_DYNAMIC Sat Jan 11 00:06:25 UTC 2025 x86_64 x86_64 x86_64 GNU/Linux
```

**See Kernel name:** Return only the kernel name. As simple as it.

```sh
uname -s
```

Output:

```sh
Linux
```

**See kernel version:** For get kernel version only you can enter the command below:

```sh
uname -v
```

Output:

```sh
#53-Ubuntu SMP PREEMPT_DYNAMIC Sat Jan 11 00:06:25 UTC 2025
```

**See all environment Variable:** For see all environment variable we can use the command `env`.

**See current directory:** If we want to see the current directory then we can execute the command below:

```sh
pwd
```

Output:

```sh
/home/sakib/Desktop
```

**See current and old directory:** For see current and old directory we can use the command below:

```sh
env | grep PWD
```

Output:

```sh
PWD=/home/sakib
OLDPWD=/home/sakib/Desktop
```

## Current User:

To see current user we can execute the command below:

```sh
whoami
```

To see the detailed information of user you can use command below:

```sh
who
```

We can also see display the boot time using `-b` flag. The command are given below:

```sh
who -H
```

## Password:

For set password on any user we can execute the command below:

```sh
sudo passwd username
```

**Force to change password**

If you want to force a user to change their password to their next login then you can execute the command below:

```sh
sudo passwd --expire username
```

**Lock a user**

Root or super user can lock/disable an user without deleting the account. User can't access their account until the super user are unlock the account. The command are given below:

```sh
sudo passwd -l username
```

**Unlock a locked user account**

I the super user want then he can unlock a locked account using the `-u` flag.

```sh
sudo passwd -u username
```

**Expiry date of password:**

Super user can also set the expiry date of a password also using the command below:

```sh
sudo passwd -x 30 username
```

## File Create and Edit:

We can make a file using the `touch` command like below:

```sh
touch hello.txt
```

We can read text type document file using the command below:

```sh
cat hello.txt
```

We can edit and make a file using vim editor using the command below:

```sh
vi hello.txt #hello.txt are file name
```
