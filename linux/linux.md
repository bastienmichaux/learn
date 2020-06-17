# Linux

## Basic commands

```bash
# print working (current) directory's absolute path
pwd

# print current user's name
whoami

# change directory
cd path/to/directory
```

## Find

Find file by name

```bash
find . -name "foo*"
```

## List files

```bash
# list files in current directory
ls
# same (default dir is current dir)
ls .
# list parent folder
ls ..
# list arbitrary folder
ls /etc

# also list hidden files
ls -a
# long format
ls -l
```

## Keyboard shortcuts

Most CLI on Linux have the following keyboard shortcuts:
- up/down arrow to recall past commands (`history`)
- tab for auto-completion
- ctrl + c soft stops an ongoing process
- ctrl + z force stops an ongoing process

## Managing directories

```bash
# create directory named "foo"
mkdir foo
# delete it
rmdir foo
```

## Managing files

```bash
# create an empty file named "foo.txt"
touch foo.txt
```

## Managing the system

```bash
# available disk space
df

# disk usage information
du

# list running processes
ps -aux

# list running processes, auto-refresh monitoring
top

# kill process (get PID from "ps" or "top" commands)
kill <PID>
kill 4928

# print detailed service status
service <service_name> status
```

## Copy files

### `cp`

### Secure copy (`scp`)

```bash
# copy local file to remote machine
scp local_file remote_user@remote_machine:remote_path

# copy file from remote machine to local machine
scp remote_user@remote_machine:remote_path local_file
```
