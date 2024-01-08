# project1_OS_1
Shell Scripting and Regexes
1. Big Files
Write a shell script called bigfiles that prints out a directory listing with each file size followed by its name of the 7 largest files in the /usr/bin directory. The sizes and files should be sorted in descending (reverse) order with the largest file first.

Think of how you can pipe commands together to make this happen in a single line.

Example output:

15181424 fileproviderctl
12455552 parl5.30
6045856 kmutil
4693872 vim
3898064 sqlite3
3780304 dig
3762464 delv
2. Command Line Arguments
A special variable $1 holds the first command line argument for a script. Write a script called arg1 with one line:

echo $1
Then run it like this:

% sh arg1 Hello
You should see Hello on the output, or whatever you typed as an argument. Any place $1 is placed in the script, whatever you typed for the first argument will be substituted there.

3. Saving Web Data
Like with $1, $2 is the second command line argument. Write a script called geturl that gets a file from a URL and saves it with the given filename, like so:

% sh geturl https://example.com/ example.html
Hint: if you're using curl, using the -s flag will put it in "silent" mode and cause it to not output the progress information.

4. Generalizing bigfiles
Copy the bigfiles script from part 1 to bigfiles2 and modify it to work on the directory specified as a command line argument.

For testing, in Unix, a single period . means "the current directory", and .. means the parent directory.

5. Grepping with Regexes
Write a shell script called vowelending that will show all filenames (including the extension--foo.txt should not match) of a directory specified on the command line that end with a vowel, upper or lowercase. Use ls -a to get the directory listing.

6: Grepping Part 2
Write a shell script called findlink that takes a URL as an argument and prints the lines that match an anchor tag, that is, tags beginning with <a. Don't forget the single quotes around that regex!
