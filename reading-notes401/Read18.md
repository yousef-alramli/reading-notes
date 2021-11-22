# Python Regular Expression 

A Regular Expressions (RegEx) is a special sequence of characters that uses a search pattern to find a string or set of strings. ... Python provides a re module that supports the use of regex in Python. Its primary function is to offer a search, where it takes a regular expression and a string.

## Basic Patterns: Ordinary Characters

you can easily tackle many basic patterns in Python using ordinary characters. Ordinary characters are the simplest regular expressions. They match themselves exactly and do not have a special meaning in their regular expression syntax.

## Wild Card Characters: Special Characters

Special characters are characters that do not match themselves as seen but have a special meaning when used in a regular expression. For simple understanding, they can be thought of as reserved metacharacters that denote something else and not what they look like.


But before you do, the examples below make use of two functions namely: search() and group().
With the search function, you scan through the given string/sequence, looking for the first location where the regular expression produces a match.
The group function returns the string matched by the re. You will see both these functions in more detail later.


**characters :**
- the dot (**.**) - A period. Matches any single character except the newline character.
- **^** - A caret. Matches the start of the string.
- $ - Matches the end of string.
- **[a-zA-Z0-9]** - Matches any letter from (a to z) or (A to Z) or (0 to 9).
- Backslash **\ -** can be used in front of all the metacharacters to remove their special meaning
- **\w** - Lowercase 'w'. Matches any single letter, digit, or underscore.
- **\W** - Uppercase 'W'. Matches any character not part of \w (lowercase w).
- **\s** - Lowercase 's'. Matches a single whitespace character like: space, newline, tab, return.
- **\S** - Uppercase 'S'. Matches any character not part of \s (lowercase s).
- **\d** - Lowercase d. Matches decimal digit 0-9.
- **\D** - Uppercase d. Matches any character that is not a decimal digit.
- **\t** - Lowercase t. Matches tab.
- **\n** - Lowercase n. Matches newline.
- **\r** - Lowercase r. Matches return.
- **\A** - Uppercase a. Matches only at the start of the string. Works across multiple lines as well.
- **\Z** - Uppercase z. Matches only at the end of the string.

- **\b**- Lowercase b. Matches only the beginning or end of the word.

**Repetitions**
- **+** - Checks if the preceding character appears one or more times starting from that position.
- **. * .** - Checks if the preceding character appears zero or more times starting from that position.
- **?** - Checks if the preceding character appears exactly zero or one time starting from that position.
- **{x}** - Repeat exactly x number of times.
- **{x,}** - Repeat at least x times or more.
- **{x, y}** - Repeat at least x times but no more than y times.

## Grouping in Regular Expressions
The group feature of regular expression allows you to pick up parts of the matching text. Parts of a regular expression pattern bounded by parenthesis () are called groups. The parenthesis does not change what the expression matches, but rather forms groups within the matched sequence. You have been using the group() function all along in this tutorial's examples. The plain match.group() without any argument is still the whole matched text as usual.

## Greedy vs. Non-Greedy Matching
When a special character matches as much of the search sequence (string) as possible, it is said to be a "Greedy Match". 

The pattern <.*> matched the whole string, right up to the second occurrence of >.

## Function provided by 're'
The re library in Python provides several functions to make your tasks easier. You have already seen some of them, such as the re.search(), re.match()

# shutil 
The shutil in Python is a module that offers several functions to deal with operations on files and their collections. It provides the ability to copy and removal of files. In a way, it is similar to the OS Module; however, the OS Module does have functions dealing with collections of files.

## Copying File Metadata
By default when a new file is created under Unix, it receives permissions based on the umask of the current user. To copy the permissions from one file to another, use copymode().

## Working With Directory Trees
shutil includes three functions for working with directory trees. To copy a directory from one place to another, use copytree(). It recurses through the source directory tree, copying files to the destination. The destination directory must not exist in advance.

## Finding Files
The which() function scans a search path looking for a named file. The typical use case is to find an executable program on the shell’s search path defined in the environment variable PATH.


## Archives
Python’s standard library includes many modules for managing archive files such as tarfile and zipfile. There are also several higher-level functions for creating and extracting archives in shutil. get_archive_formats() returns a sequence of names and descriptions for formats supported on the current system.


## File System Space
It can be useful to examine the local file system to see how much space is available before performing a long running operation that may exhaust that space. disk_usage() returns a tuple with the total space, the amount currently being used, and the amount remaining free.



