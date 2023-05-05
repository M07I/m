
### **`man`** command in Linux

**`man`** command is a *tool* used to display a *manual* for any command that we can run on the terminal.  
**`man`** pages are mainly stored in the **`/usr/share/man directory`**.

###### How To Navigate the Man Page

+ To move forward one line: ***j, e, ^E, ^N, or the Return key***   
If you use a number, like ***5j ( or 5e, 5^E, 5^N, etc.)*** you move five lines forward.

+ To move backward one line, ***k ( or ^Y, y, ^K, or ^P)***.  
You can use a number, like ***5k ( or 5^Y, 5y, 5^K, 5^P, etc.)*** to move five lines backward.

+ To move to the top: ***g***
+ To move to the end of the manual: ***G***
+ To move forward one window: ***f ( or ^F, ^V, or space)***
+ To move backward one window: ***b ( or ^B or ESC-v)***
+ To move one-half window forward: ***d (or ^D)***
+ To move one-half window backward: ***u (or ^U)***
+ To shift the view to the right or left: ***use the right and left arrows***
+ To jump to an option: **/** (the name of the option we want to find), __example:$ man ls
/-h__
+ To get help: ***h***
+ To continue the search: ***n***
+ To  quit the page: ***q***

###### Searching by Keyword

If we’re unsure of the name of a command, we can use a search string to look for a keyword that matches the manual. Using the -k flag with man makes it equivalent to the apropos command:

**`$ man -k passwd   
chgpasswd (8)        - update group passwords in batch mode`**

Let’s strictly limit the results from the matched string by adding a caret (^):  

**`$ man -k '^passwd'
passwd (1)           - change user password`**

###### Running a Command Within the **`man`**

The man page allows us to run commands inside it without switching consoles. For example, if we want to test ls, we type **`!ls`**  
Afterward, we press Enter and get the output displayed. We hit Enter again to return to the **`man`** page.



