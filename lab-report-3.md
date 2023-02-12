Lab Report 3
==========


Researching grep Commands
--------------

* -v, --invert-match
* -m, --max-count=NUM
* -c, --count
* -n, --line-number

grep -v
--------

I found grep -v by using the command grep --help from the command line.
>   -v, --invert-match        select non-matching lines

````
[cs15lwi23apk@ieng6-201]:~:122$ grep -v ".txt" find-results.txt 
skill-demo1-data
skill-demo1-data/.git
skill-demo1-data/.git/info
skill-demo1-data/.git/info/exclude
skill-demo1-data/.git/hooks
skill-demo1-data/.git/hooks/commit-msg.sample
skill-demo1-data/.git/hooks/prepare-commit-msg.sample
skill-demo1-data/.git/hooks/update.sample
skill-demo1-data/.git/hooks/pre-rebase.sample
skill-demo1-data/.git/hooks/pre-merge-commit.sample
skill-demo1-data/.git/hooks/push-to-checkout.sample
skill-demo1-data/.git/hooks/pre-push.sample
skill-demo1-data/.git/hooks/pre-commit.sample
skill-demo1-data/.git/hooks/post-update.sample
skill-demo1-data/.git/hooks/pre-receive.sample
skill-demo1-data/.git/hooks/applypatch-msg.sample
skill-demo1-data/.git/hooks/fsmonitor-watchman.sample
skill-demo1-data/.git/hooks/pre-applypatch.sample
skill-demo1-data/.git/branches
skill-demo1-data/.git/description
skill-demo1-data/.git/refs
skill-demo1-data/.git/refs/heads
skill-demo1-data/.git/refs/heads/main
skill-demo1-data/.git/refs/tags
skill-demo1-data/.git/refs/remotes
skill-demo1-data/.git/refs/remotes/origin
skill-demo1-data/.git/refs/remotes/origin/HEAD
skill-demo1-data/.git/objects
skill-demo1-data/.git/objects/pack
skill-demo1-data/.git/objects/pack/pack-b98cb6a4ca64cc7b2944f0fa07d3e03927d66064.pack
skill-demo1-data/.git/objects/pack/pack-b98cb6a4ca64cc7b2944f0fa07d3e03927d66064.idx
skill-demo1-data/.git/objects/info
skill-demo1-data/.git/HEAD
skill-demo1-data/.git/config
skill-demo1-data/.git/logs
skill-demo1-data/.git/logs/refs
skill-demo1-data/.git/logs/refs/remotes
skill-demo1-data/.git/logs/refs/remotes/origin
skill-demo1-data/.git/logs/refs/remotes/origin/HEAD
skill-demo1-data/.git/logs/refs/heads
skill-demo1-data/.git/logs/refs/heads/main
skill-demo1-data/.git/logs/HEAD
skill-demo1-data/.git/packed-refs
skill-demo1-data/.git/index
skill-demo1-data/written_2
skill-demo1-data/written_2/non-fiction
skill-demo1-data/written_2/non-fiction/OUP
skill-demo1-data/written_2/non-fiction/OUP/Abernathy
skill-demo1-data/written_2/non-fiction/OUP/Berk
skill-demo1-data/written_2/non-fiction/OUP/Castro
skill-demo1-data/written_2/non-fiction/OUP/Fletcher
skill-demo1-data/written_2/non-fiction/OUP/Kauffman
skill-demo1-data/written_2/non-fiction/OUP/Rybczynski
skill-demo1-data/written_2/travel_guides
skill-demo1-data/written_2/travel_guides/berlitz1
skill-demo1-data/written_2/travel_guides/berlitz2
````
The grep -v command used above prints out the lines that do not contain ".txt". This is helpful for excluding specific words/phrases from an output.

````
[cs15lwi23apk@ieng6-201]:non-fiction:134$ grep -v ".txt" find.txt 
./
./OUP
./OUP/Abernathy
./OUP/Berk
./OUP/Castro
./OUP/Fletcher
./OUP/Kauffman
./OUP/Rybczynski
````
The grep -v command used above prints out the lines that do not contain ".txt". This is helpful for excluding specific words/phrases from an output.

grep -m
------

I found grep -m by using the command grep --help from the command line.
>   -m, --max-count=NUM       stop after NUM matches

````
[cs15lwi23apk@ieng6-201]:~:137$ grep -m 5 ".txt" find-results.txt 
skill-demo1-data/written_2/non-fiction/OUP/Abernathy/ch1.txt
skill-demo1-data/written_2/non-fiction/OUP/Abernathy/ch14.txt
skill-demo1-data/written_2/non-fiction/OUP/Abernathy/ch15.txt
skill-demo1-data/written_2/non-fiction/OUP/Abernathy/ch2.txt
skill-demo1-data/written_2/non-fiction/OUP/Abernathy/ch3.txt
````
The grep -m command used above prints out only 5 lines at most of lines that contain the characters ".txt". This is helpful for maxing out how many lines appear so that it does not print out a bunch of lines.

````
[cs15lwi23apk@ieng6-201]:~:138$ grep -m 7 ".txt" grep-results.txt 
skill-demo1-data/written_2/non-fiction/OUP/Abernathy/ch1.txt
skill-demo1-data/written_2/non-fiction/OUP/Abernathy/ch14.txt
skill-demo1-data/written_2/non-fiction/OUP/Abernathy/ch15.txt
skill-demo1-data/written_2/non-fiction/OUP/Abernathy/ch2.txt
skill-demo1-data/written_2/non-fiction/OUP/Abernathy/ch3.txt
skill-demo1-data/written_2/non-fiction/OUP/Abernathy/ch6.txt
skill-demo1-data/written_2/non-fiction/OUP/Abernathy/ch7.txt
````
The grep -m command used above prints out only 7 lines at most of lines that contain the characters ".txt". This is helpful for maxing out how many lines appear so that it does not print out a bunch of lines.

grep -c
------

I found grep -c by using the command grep --help from the command line.
>-c, --count               print only a count of matching lines per FILE

````
[cs15lwi23apk@ieng6-201]:~:139$ grep -c ".txt" find-results.txt 
224
````
The grep -c command used above prints out the number of lines from the file that contain ".txt" in the file. This is useful for determining how many lines in a file contain a specific phrase/word.

````
[cs15lwi23apk@ieng6-201]:~:142$ grep -c "OUP" grep-results.txt 
45
````
The grep -c command used above prints out the number of lines from the file that contain "OUP" in the file. This is useful for determining how many lines in a file contain a specific phrase/word.

grep -n
------

I found grep -n by using the command grep --help from the command line.
> -n, --line-number         print line number with output lines

````
[cs15lwi23apk@ieng6-201]:~:144$ grep -n "Rybc" grep-results.txt 
43:skill-demo1-data/written_2/non-fiction/OUP/Rybczynski/ch1.txt
44:skill-demo1-data/written_2/non-fiction/OUP/Rybczynski/ch2.txt
45:skill-demo1-data/written_2/non-fiction/OUP/Rybczynski/ch3.txt
````
The grep -n command used above prints out the line number with the line that contains "Rybc" in the line. This is helpful for determining where a phrase is within the file, making it easier to find where the phrase is.

````
[cs15lwi23apk@ieng6-201]:~:147$ grep -n "Vallarta" find-results.txt 
278:skill-demo1-data/written_2/travel_guides/berlitz2/Vallarta-History.txt
279:skill-demo1-data/written_2/travel_guides/berlitz2/Vallarta-WhatToDo.txt
280:skill-demo1-data/written_2/travel_guides/berlitz2/Vallarta-WhereToGo.txt
````
The grep -n command used above prints out the line number with the line that contains "Vallarta" in the line. This is helpful for determining where a phrase is within the file, making it easier to find where the phrase is.
