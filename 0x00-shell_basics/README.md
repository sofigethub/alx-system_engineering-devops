pwd  prints the absolute path name of the current working directory

ls Display the contents list of current directory

cd ~ changes the working directory to the user’s home directory

ls -l Display current directory contents in a long format

ls -la Display current directory contents, including hidden files (starting with .) Useing the long format

ls -lna Display current directory contents.Long format with user and group IDs displayed numerically

And hidden files (starting with .)

mkdir /tmp/my_first_directory Creates a directory named my_first_directory in the /tmp/ directory

mv /tmp/betty /tmp/my_first_directory Move the file betty from /tmp/ to /tmp/my_first_directory

rm /tmp/my_first_directory/betty  Delete the file betty in /tmp/my_first_directory

rmdir /tmp/my_first_directory Delete the directory my_first_directory that is in the /tmp directory

cd - changes the working directory to the previous one

ls -al . .. /boot  lists all files n the current directory and the parent of the working directory and the /boot directory (in this order), in long format.

file /tmp/iamafile prints the type of the file named iamafile in the /tmp directory

sln -s /bin/ls __ls__ Create a symbolic link to /bin/ls, named __ls__ in current directory

cp  *.html ..   copies all the HTML files from the current working directory to the parent of the working directory
