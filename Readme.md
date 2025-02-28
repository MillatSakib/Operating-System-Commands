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
