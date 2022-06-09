Command line for the win

1. Your first challenge is to print "hello world" on the terminal in a single command. R// echo hello world o printf “hello world”
2. Print the current working directory. R// echo $(pwd)
3. List names of all the files in the current directory, one file per line. R// ls *
4. There is a file named access.log in the current directory. Print the contents. R// cat access.log
5. Print the last 5 lines of "access.log". R// tail -n 5 access.log
6. Create an empty file named take-the-command-challenge in the current working directory. R// touch take-the-command-challenge
7. Create a directory named tmp/files in the current working directory R// mkdir -p /tmp/files
8. Copy the file named take-the-command-challenge to the directory tmp/files R// cp take-the-command-challenge tmp/files
9. Move the file named take-the-command-challenge to the directory tmp/files R// mv take-the-command-challenge tmp/files
10. Create a symbolic link named take-the-command-challenge that points to the file tmp/files/take-the-command-challenge. R// ln -s tmp/files/*
11. Delete all of the files in this challenge directory including all subdirectories and their contents. R// find -delete
12. There are files in this challenge with different file extensions. Remove all files with the .doc extension recursively in the current working directory. R// rm -r **/*.doc
13. There is a file named access.log in the current working directory. Print all lines in this file that contains the string "GET" R// cat access.log | grep GET
14. Print all files in the current directory, one per line (not the path, just the filename) that contain the string "500" R// grep -ls 500 *
15. Print the relative file paths, one path per line for all filenames that start with "access.log" in the current directory. R// ls
16. Print all matching lines (without the filename or the file path) in all files under the current directory that start with "access.log" that contain the string "500". R// grep -r -h "500" --include access.log
17. Extract all IP addresses from files that start with "access.log" printing one IP address per line R// grep -ro ^[0-9.]* --include access.log
18. Count the number of files in the current working directory. Print the number of files as a single integer R// ls -l | wc -l
19. 
