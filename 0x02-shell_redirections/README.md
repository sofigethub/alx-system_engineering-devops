echo Hello, World  prints “Hello, World”, followed by a new line to the standard output.
echo "\"(Ôo)'" displays a confused smiley "(Ôo)'.
cat /etc/passwd Display the content of the /etc/passwd file.
cat /etc/passwd /etc/hosts Display the content of /etc/passwd and /etc/hosts
tail /etc/passwd Display the last 10 lines of /etc/passwd
head /etc/passwd Display the first 10 lines of /etc/passwd
head -3 iacta | tail -l displays the third line of the file iacta

echo "Best School" >> "\*\\\'\"Best School\"\'\\\*$\?\*\*\*\*\*:)" creates a file named exactly \*\\'"Best School"\'\\*$\?\*\*\*\*\*:) containing the text Best School ending by a new line.

ls -la > ls_cwd_content writes into the file ls_cwd_content the result of the command ls -la. If the file ls_cwd_content already exists, it should be overwritten. If the file ls_cwd_content does not exist, create it.

tail -1 < iacta >> iacta Write a script that duplicates the last line of the file iacta

find -name "*.js" -type f -delete deletes all the regular files (not the directories) with a .js extension that are present in the current directory and all its subfolders. 

find . -type d ! -path . -print | wc -l    Don't just count your directories, make your directories count

ls -1t | hed -10 displays the 10 newest files in the current directory.

sort | uniq -u   Create a script that takes a list of words as input and prints only words that appear exactly once.

grep "root"  /etc/passwd   Display lines containing the pattern “root” from the file /etc/passwd

grep -c "bin" /etc/passwd  Display the number of lines that contain the pattern “bin” in the file /etc/passwd

grep -A 3 "root" /etc/passwd   Display lines containing the pattern “root” and 3 lines after them in the file /etc/passwd.

grep -v "bin" /etc/passwd   Display all the lines in the file /etc/passwd that do not contain the pattern “bin”.

grep ^[[:alpha:]] /etc/ssh/sshd_config  Display all lines of the file /etc/ssh/sshd_config starting with a letter.

tr 'A' 'Z' | tr 'c' 'e' Replace all characters A and c from input to Z and e respectively.

tr -d 'c' | tr -d 'C' removes all letters c and C from input

rev  reverse its input.

cut -d: -f 1,6 /etc/passwd | sort displays all users and their home directories, sorted by users.

find -empty | rev |cut -d/ -f1 | rev      Write a command that finds all empty files and directories in the current directory and all sub-directories, Only the names of the files and directories should be displayed (not the entire path), hidden files should be listed, One file name per line                         

find -type f -name "*.gif" -printf "%f\n" | rev | cut -d '.' -f 2- | rev | LC_ALL=C sort -f     lists all the files with a .gif extension in the current directory and all its sub-directories.                   

cut -c1 | paste -s |tr -d "[:blank:]"   decodes acrostics that use the first letter of each line.

tail -n +2 | cut -f1 | sort | uniq -c | sort -nr |head -11 | tr -s ' ' | cut -d' ' -f3    parses web servers logs in TSV format as input and displays the 11 hosts or IP addresses which did the most requests.                         




















