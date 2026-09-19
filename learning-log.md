# Learing Log

## Previously and Recently - Linux Fundamentals

## Learned

# Navigations

pwd = show current location
ls = show current files and directries
ls -l = show current stuffs with deatials
ls -a = show list with hidden stuffs
ls -la = show current stuffs with hidden  and details
cd = go to main location = cd ~
cd ../ = backword one directry = cd ..
cd ../../ = becaword 2 directries
cd Desktop = go to Desktop Directry

## Today

cd .. = parent directry = cd ../
cd ~ = home directry = cd 
cd / = root directry 


# Directories

mkdir = make a directry , actually directy means like a folder 
rmdir = remove folder

rm -rf = force delete directries

- Note , Some times we can not delete some folders using rmdir therefore we use some force deleting command .

# Files

touch = make a file
cat = show the inside the file content 
less = view a file page by page (easy to navigate)
tail = show bottom of file contents (10 lines by defoult)
head = show top of file contents (same)

# Copy , Move , Delete

cp = copy files only 
cp -r = copy directries and inside every things in that directry

mv = use to move and rename also we can do
 
rm = remove file
rm -r = remove the whole directry 
rm -rf = fource deleting directry


# Problems and Answers

1. what is the root directry and home directry  ? - The directry is the top of entire Linux filesystem. "whole linux house" , home directry is like a room in the >
2. what does mkdir -p = p stand for parent , anyway think if we cmd something mkdir Newprojects/first/icons and those folders does not exsist then this will make >
 




## Linux Fundermental - 2026 sep 18 

### Learing Log

# find =  Search / Filter (We can search anything from home or any directry)

- find = use to find files and directries.
as an example find . -name "errors.txt" (Meaning - Search from the current directry (. - means current directry , .. - back current and more one directry)) for somthing named errors.txt .

find . -name "hello.md" = search file name as hello.md
find . -name "*.txt" = Astric mark means whatever name (when we do not know file name) , this will show all .txt files
find . -type f = find  all files
find . -type d = find all directories

# grep =  Find Text Inside Files

- grep = where is the text 

grep "hello" file.txt = show the lines contain hello
grep "error" log.txt = show lines contain error

grep -r "error" . = Search for error inside files thoughout the current directory. (output is - file name : exact lines or line)

# Pipes / Redirection

| = this does send the output of one command into another command

ex, 
ls | less - take the output of ls and give it to less

ls | grep ".txt" - List files ----> search that list for .txt 


> - Redirect / overwrite
Send output into a file ,replacing its existing content.
ex,
ls > files.txt - Now the output of ls is stored in files.txt
echo "Hi it is mistake" >  invite.txt  - this masage overwrite in the text file content

>> - Redirect / append
Send output into a file /adding it in to end .
ex,
echo "Good Morning" > note.txt 
echo "Hello" >> notes.txt - add the Hello masage after the Good moring line

2> - Redirect Errors

2 respresents standard error (stderr). This is like error handling according to me.
ex,

ls /something-non-exist 2> error.txt - instead of showing the error on my terminal the error goes in to error.txt
command > output.txt 2> error.txt 
comamnd | grep "error"

























