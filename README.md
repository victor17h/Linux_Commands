#Linux commands

- Check hidden files or directories with `ls -a` or `ls -al`.
- A wildcard is a symbol or set of symbols that stands in for other characters. If we want the list of files that start with O, end with d and have two characters in betweeen we use `ls -l O??d`, if we want the ones that start with O and end with d we use `ls -l O*d`, if we want the ones that start with O, end with d and hace a or c we use `ls O[ac]d`
- Flags are a way to set options and pass arguments to the command you run. Ruuning `ls -l` will include more information in the result and change the format of what is returned.
- Different process managements: Process status `ps`, list of process in the background `ps -f`, to know more info of the process `ps -ef`
- Type `ps aux` to see all running process in Linux.
- To kill a process use `kill -l`.
- Show all running process including background using `$ sudo ps -aux | less` or `ps aux | more`.
- To kill a process in the background use `kill %n` or `kill %2`.
- Change permissions use `chmod +rwx filename` to add permissions, `chmod -rwx directoryname` to remove permissions, `chmod +x filename`, to allow executable permissions, or `chmod -wx filename``to take out write and executable permissions.
- To check permission configuration of a file use `ls -l filename`. Result will show first file type, then user, next group and finally others.
- `chomd 777 file` means everybody can do everything to this file, `chmod 400 file` means to protect a file against accidental overwriting, `chmod 600 filename` means a private file only changeable by the user who entered this command, `rwx` means read, write and execute permissions for the owner of the file.
- To review the start of a file use `head -5 /etc/passwd`, to review the last few entries use `tail -5 /etc/passwd`, to sort files by login name use `sort /etc/passwd`, use `nl filename` to show number line, use `wc option filename` for word count.
- A pipe is a form of redirection (transfer of standard output to some other destination) that is used in Linux and other Unix-like operating systems to send the output of one command/program/process to another command/program/process for further processing. You can make it do so by using the pipe character `l`.
- `stdin` is the standard input stream. This accepts text as input. Text output from the command to the shell is delivered via the `stdout` standatd out stream. Error messages from the command are sent through the `stderr` standard error stream.
