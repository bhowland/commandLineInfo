https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/findstr

https://stackoverflow.com/questions/17945514/find-files-which-does-not-contains-selected-string

https://superuser.com/questions/1332287/how-do-i-find-files-containing-string-a-and-not-containing-string-b-and-outp

https://unix.stackexchange.com/questions/178362/rsync-recursively-with-a-certain-depth-of-subfolders

https://linux.die.net/man/1/rsync

https://www.redswitches.com/blog/rsync-exclude-directory/#:~:text=To%20exclude%20a%20specific%20directory,included%20in%20the%20data%20transfer.

https://www.redswitches.com/blog/rsync-command/

https://askubuntu.com/questions/85137/rsync-not-actually-copying-files

https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/robocopy

grep -Lr "KAR" . | xargs grep -l "VIN"

find . -type f -name "*VIN*" ! -exec grep -q "KAR" {} \; -print

grep -Lr "KAR" . | grep "VIN"

find . -type f -name "*VIN*" | grep -v "KAR"

grep -Lr "KAR" .


grep -Lr "KAR" *.*

findstr /I /S /M /C:".*KAR.*" *.* > results.txt & findstr /V /G:results.txt *.*

findstr /I /S /M /C:"KAR" *.* > results.txt & findstr /V /G:results.txt *.*
