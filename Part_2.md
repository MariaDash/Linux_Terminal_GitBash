# Part#2: Basic Linux commands created  with GitBash
## 1. Create dir_1 directory

```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir (main)
$ mkdir dir_1

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir (main)
$ ls
dir_1/

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir (main)
$
```
or if we want to make a tree:
```
mkdir -p  /name_dir1_1/name_dir_2
```
## 2. Change directory to dir_1

```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir (main)
$ cd dir_1

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```

## 3. Create directory inner_dir_1

```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ mkdir inner_dir_1

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ ls
inner_dir_1/

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```

## 4. Print, where I am

```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ pwd
/d/Testing_Course/Git/main_dir/sub_dir/dir_1

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```

## 5. Create an empty text file tf_1.txt in dir_1 directory

```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ touch tf_1.txt

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ ls
inner_dir_1/  tf_1.txt

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ cat tf_1.txt

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```

## 6. Create tf_2.txt file in dir_1 with following strings:
- the first 1
- the second 2
- the third 3

```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ cat > tf_2.txt
the first 1
the second 2
the third 3

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ cat tf_2.txt
the first 1
the second 2
the third 3

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```

## 7. Change directory to inner_dir_1

```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ cd inner_dir_1

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$
```

## 8. Create tf_3.txt file with any strings

```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$ cat > tf_3.txt
I am happy amd I know it
I am funny and I know it
I am goofy and I know it

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$
```

## 9. Add the string "the second 2" to the file tf_3.txt using "cat" command

```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$ cat >>tf_3.txt
the second 2

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$ cat tf_3.txt
I am happy amd I know it
I am funny and I know it
I am goofy and I know it
the second 2

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$
```

## 10. Add the string "the sec 2" to the file tf_3.txt using "cat" command

```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$ cat >> tf_3.txt
the sec 2

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$
```

## 11. Add the string "the sec 3" to the file tf_2.txt using "cat" command

```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$ cat >> /d/Testing_Course/Git/main_dir/sub_dir/dir_1/tf_2.txt
the sec 3

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$ cat /d/Testing_Course/Git/main_dir/sub_dir/dir_1/tf_2.txt
the first 1
the second 2
the third 3
the sec 3

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$
```
or another way to write path -  relative path. you can go level up and choose directory from that level for saving file:
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$ cat >> ../tf_2.txt
```
## 12. Add the string "the SeCoNd 2" to the file tf_3.txt using "cat" command

```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$ cat >> tf_3.txt
the SeCoNd 2

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$ cat tf_3.txt
I am happy amd I know it
I am funny and I know it
I am goofy and I know it
the second 2
the sec 2
the SeCoNd 2

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$
```

## 13. Add the string "the seConD 2" to the file tf_2.txt using "cat" command

```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$ cat >> /d/Testing_Course/Git/main_dir/sub_dir/dir_1/tf_2.txt
the seConD 2

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$ cat /d/Testing_Course/Git/main_dir/sub_dir/dir_1/tf_2.txt
the first 1
the second 2
the third 3
the sec 3
the seConD 2

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$
```
or
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$ cat ../tf_2.txt
```
## 14. Create text file tf_4.txt containing 15 strings
### 1. Creating numbers manually
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$ cat > tf_4.txt
1
2
3
4
5
6
7
8
9
10
11
12
13
14
15

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$
```
or 
### 2. Creating numbers automatically
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$ seq 15 | cat > tf_4.txt
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ 
```
or 
### 3. Creating strings automatically

```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ touch tf_6.txt; printf "Line %s\n" {1..15} > tf_6.txt

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ cat tf_6.txt
Line 1
Line 2
Line 3
Line 4
Line 5
Line 6
Line 7
Line 8
Line 9
Line 10
Line 11
Line 12
Line 13
Line 14
Line 15

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$

```
## 15. Create text file tF_5.txt containing 13 strings
### 1. Creating numbers manually
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$ cat > tF_5.txt
1
2
3
4
5
6
7
8
9
10
11
12
13

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$
```
or
### 2. Creating numbers automatically
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$ seq 13 | cat > tF_5.txt
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ 
```
or

Let's try with additional "string:" text and the numbers (need to create a similar for loop):
```
$ for string_number in {1..13}; do echo "string: ${string_number}"; done > tF_5.txt
```
Note: a sequence starts with `1` by default, but in case of loop we need to specify the range, the last number of range is included to the range.
Result:

```
string: 1
string: 2
string: 3
string: 4
string: 5
string: 6
string: 7
string: 8
string: 9
string: 10
string: 11
string: 12
string: 13
```

## 16. List all file in the directory

```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$ ls -la
total 3
drwxr-xr-x 1 Admin 197121   0 Apr 22 14:08 ./
drwxr-xr-x 1 Admin 197121   0 Apr 22 13:35 ../
-rw-r--r-- 1 Admin 197121  30 Apr 22 14:09 tF_5.txt
-rw-r--r-- 1 Admin 197121 111 Apr 22 14:00 tf_3.txt
-rw-r--r-- 1 Admin 197121  36 Apr 22 14:06 tf_4.txt

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$
```

## 17. Change directory from current inner_dir_1
go 1 level up:
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1 (main)
$ cd ..

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```
or if we want to go 2 level up:
```
$ cd ../..
```
## 18. Show the contents of tf_3.txt file

```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ cat /d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1/tf_3.txt
I am happy amd I know it
I am funny and I know it
I am goofy and I know it
the second 2
the sec 2
the SeCoNd 2

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```

## 19. Find path to tf_4.txt

```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ find -name tf_4.txt
./inner_dir_1/tf_4.txt

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```
or if we want to specify that we are searching only in current directory, we use `./` :
```
$ find ./ -name "tf_4.txt"
```
## 20. Clear the contents of the file tf_4.txt without deleting it

```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ cat ./inner_dir_1/tf_4.txt
1
2
3
4
5
6
7
8
9
10
11
12
13
14
15

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ echo -n > ./inner_dir_1/tf_4.txt

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ cat ./inner_dir_1/tf_4.txt

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```
or
Let's use the `>` operator and redirect the empty output to the file:
```
> inner_dir_1/tf_4.txt
```
## 21. Find path to files with 'tf' in the name. Case sensitive.

```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ find -name '*tf*'
./inner_dir_1/tf_3.txt
./inner_dir_1/tf_4.txt
./tf_1.txt
./tf_2.txt

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```

## 22. Find path to files with 'tf' in the name. Case insensitive.

```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ find -iname '*tf*'
./inner_dir_1/tf_3.txt
./inner_dir_1/tf_4.txt
./inner_dir_1/tF_5.txt
./tf_1.txt
./tf_2.txt

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```

## 23. Find strings in files where 'sec' is located in the current directory. Case sensitive.

### 1) Only in dir_1:
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ grep 'sec' ./*
grep: inner_dir_1: Is a directory
tf_2.txt:the second 2
tf_2.txt:the sec 3

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```
Note: an asterisk  means searching for strings in all the files
### 2) In dir_1 and in child directory inner_dir_1:
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ grep -r 'sec' *
inner_dir_1/inner_dir_1:the second 2
inner_dir_1/inner_dir_1:the sec 2
inner_dir_1/tf_3.txt:the sec 2
tf_2.txt:the second 2
tf_2.txt:the sec 3

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```

Option 2: if we can filter the files by formats, we can also skip the inner directory, so let's do this:
```
$ grep "sec" ./*.txt
```
As a result, we see no message:
```
./tf_2.txt:the second 2
./tf_2.txt:the sec 3
```
Option 3: if we don't know the files formats, we can just use -s parameter as a silent option for not displaying the message:
```
$ grep -s "sec" ./*.txt
```
As a result, we also see no message:
```
./tf_2.txt:the second 2
./tf_2.txt:the sec 3
```
Note: you can use `grep -n sec ./` to specify number of string where letter combination `sec` is located.

### 3 If we want to search strings in a folder 1 level up:
We are located in `dir1`, we need to go two level up to `main_dir` and go level down to `sub_dir` and search all files there:
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ grep 'sec' ../../sub_dir/*
```

## 24. Find strings in files where 'sec' is located in the current directory. Case insensitive.
### 1) Only in dir_1:
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ grep -i 'sec' ./*
grep: inner_dir_1: Is a directory
tf_2.txt:the second 2
tf_2.txt:the sec 3
tf_2.txt:the seConD 2

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```
### 2) In dir_ and in inner_dir_1:

```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ grep -ir 'sec' ./*
inner_dir_1/inner_dir_1:the second 2
inner_dir_1/inner_dir_1:the sec 2
inner_dir_1/inner_dir_1:the SeCoNd 2
inner_dir_1/tf_3.txt:the sec 2
inner_dir_1/tf_3.txt:the SeCoNd 2
tf_2.txt:the second 2
tf_2.txt:the sec 3
tf_2.txt:the seConD 2

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```
Advanced: you can color the pattern:
```
grep --color=always sec *
```
or not color at all:
```
grep --color=never sec *
```
## 25.  Find strings in files where  'sec' is standalone pattern and is located in the current directory. Case sensitive.
### 1) Only in dir_1:
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ grep -w 'sec' ./*
grep: inner_dir_1: Is a directory
tf_2.txt:the sec 3

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```
### 2) In dir_ and in inner_dir_1:
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ grep -rw 'sec' ./*
inner_dir_1/inner_dir_1:the sec 2
inner_dir_1/tf_3.txt:the sec 2
tf_2.txt:the sec 3

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```

## 26. Find strings in files where  'sec' is standalone pattern and is located in the current directory. Case insensitive.
### 1) Only in dir_1:
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ grep -iw 'sec' ./*
grep: inner_dir_1: Is a directory
tf_2.txt:the sec 3

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```
### 2) In dir_ and in inner_dir_1:
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ grep -iwr 'sec' ./*
inner_dir_1/inner_dir_1:the sec 2
inner_dir_1/tf_3.txt:the sec 2
tf_2.txt:the sec 3

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```

## 27. Find strings in files that contain  'second' letter combination and is located in the current directory. Case sensitive.
### 1) Only in dir_1:
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ grep 'second' ./*
grep: inner_dir_1: Is a directory
tf_2.txt:the second 2

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```
### 2) In dir_ and in inner_dir_1:
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ grep -r 'second' ./*
inner_dir_1/inner_dir_1:the second 2
tf_2.txt:the second 2

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```

## 28. Find strings in files that contain  'second' letter combination and is located in the current directory. Case insensitive.
### 1) Only in dir_1:
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ grep -i 'second' ./*
grep: inner_dir_1: Is a directory
tf_2.txt:the second 2
tf_2.txt:the seConD 2

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```
### 2) In dir_ and in inner_dir_1:
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ grep -ir 'second' ./*
inner_dir_1/inner_dir_1:the second 2
inner_dir_1/inner_dir_1:the SeCoNd 2
inner_dir_1/tf_3.txt:the SeCoNd 2
tf_2.txt:the second 2
tf_2.txt:the seConD 2

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```
## 29. Find strings in files that contain  'second' letter combination and is located in all directories level below . Case sensitive.
### 1) In dir_1 and in inner_dir_1
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ grep -r 'second' *
inner_dir_1/inner_dir_1:the second 2
tf_2.txt:the second 2

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```
or
```
$ grep -r 'second' ./*/* 
```
The 1st * means all the subdirectories, the 2nd * means all the files in subdirectories

### 2) In inner_dir_1 while located in dir_1:
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ grep -r 'second' ./*/
./inner_dir_1/inner_dir_1:the second 2
./inner_dir_1/inner_dir_1:the second 2
./inner_dir_1/tf_3.txt:the second 2

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```

## 30. Find only files and the path to files  containing strings with 'second' letter combination in the current directory. Case sensitive.
### 1) Relative path in dir dir_1
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ grep -ls "second" ./*      
./tf_2.txt
```

### 2) Absolute path only  in dir_1:
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ grep -l second *.* | xargs realpath
/d/Testing_Course/Git/main_dir/sub_dir/dir_1/tf_2.txt

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ 
```
One more absolute path with recursive search:
```
grep -rls "second" $PWD
```

## 31. Find all lines in all files where there is no "second" combination. Case sensitive.

```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ grep  -rv 'second' *
inner_dir_1/tf_3.txt:I am happy amd I know it
inner_dir_1/tf_3.txt:I am funny and I know it
inner_dir_1/tf_3.txt:I am goofy and I know it
inner_dir_1/tf_3.txt:the sec 2
inner_dir_1/tf_3.txt:the SeCoNd 2
inner_dir_1/tF_5.txt:1
inner_dir_1/tF_5.txt:2
inner_dir_1/tF_5.txt:3
inner_dir_1/tF_5.txt:4
inner_dir_1/tF_5.txt:5
inner_dir_1/tF_5.txt:6
inner_dir_1/tF_5.txt:7
inner_dir_1/tF_5.txt:8
inner_dir_1/tF_5.txt:9
inner_dir_1/tF_5.txt:10
inner_dir_1/tF_5.txt:11
inner_dir_1/tF_5.txt:12
inner_dir_1/tF_5.txt:13
tf_2.txt:the first 1
tf_2.txt:the third 3
tf_2.txt:the sec 3
tf_2.txt:the seConD 2

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```
## 32. Find files and the path to files  not containing strings with 'second'. Case sensitive.
### 1) Relative path 
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)

$ grep -Lrs 'second'
inner_dir_1/tf_4.txt
inner_dir_1/tF_5.txt
tf_1.txt

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```
### 2) Absolute path:
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ grep -rLs second . |xargs realpath
/d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1/tf_4.txt
/d/Testing_Course/Git/main_dir/sub_dir/dir_1/inner_dir_1/tF_5.txt
/d/Testing_Course/Git/main_dir/sub_dir/dir_1/tf_1.txt

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```
## 33. Print last 4 strings of any text file

```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ tail -4 tf_2.txt
the second 2
the third 3
the sec 3
the seConD 2

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```

## 34. Print first 4 strings of any text file

```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ head -4 tf_2.txt
the first 1
the second 2
the third 3
the sec 3

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```

## 35. One string command: create a directory & not empty file
### 1) Creating a file and directory in the current directory
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ mkdir newdir |echo "1 2 3 4 5 " > newfile1.txt

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ ls
inner_dir_1/  newdir/  newfile1.txt  tf_1.txt  tf_2.txt

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ cat newfile1.txt
1 2 3 4 5

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
``` 
### 2) Create a file in the new directory

```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ mkdir newdir && cat > newdir/newfile1.txt
1 2 3 4 5
2
3
4
5
6


Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ ls
dir_2/  dir_3/  inner_dir_1/  newdir/  tf_1.txt

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ ls newdir
newfile1.txt

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```

## 36. One string command. Move text files containing word "sec" in any other directory
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ grep -rlw "sec" | xargs mv -t dir_2

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ls dir_2
inner_dir_1  tf_2.txt  tf_3.txt
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```

## 37. One string command. Copy text files containing word "sec" in any other directory
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ grep -rlw "sec" | xargs cp -t dir_3

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ ls dir_3
inner_dir_1  tf_2.txt  tf_3.txt

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```

## 38. One string command. Find all strings containing "sec" in all files . Print them all to a new file
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ grep 'sec' * | cat > allfile.txt
grep: inner_dir_1: Is a directory

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ cat allfile.txt
tf_2.txt:the second 2
tf_2.txt:the sec 3

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```
Another way:
Here, with `grep -rh` (where `-h` "cuts" the file name , as we need only lines from files).
```
$ grep -rh "sec" ./ | xargs -I{} echo {} > tf_38.txt
```

## 39. One string command: Delete all text file with strings containig letter combination "sec"
### 1) If combination "sec'
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ grep -rl sec | xargs rm

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```
or
```
grep -rl "sec" ./ | xargs -I{} rm -f {}
```
### 2) If standalone word "sec"
```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ grep -rlw sec | xargs rm

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```

## 40. Print "Good job!"

```
Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$ echo 'Good job!'
Good job!

Admin@DESKTOP-V6V9F0T MINGW64 /d/Testing_Course/Git/main_dir/sub_dir/dir_1 (main)
$
```
