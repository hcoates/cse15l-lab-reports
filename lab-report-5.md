Lab Report 3
==========

Researching find Commands
--------------

* -name
* -iname
* -type f
* -empty
* -size

I found all of these commands thoruh a google search and using [this link](https://www.booleanworld.com/guide-linux-find-command/).

-name
--------

````
[cs15lwi23apk@ieng6-201]:OUP:379$ find Abernathy/ -name ch1.txt
Abernathy/ch1.txt
````


The find Abernathy -name ch1.txt finds the ch1.txt file within Abernaty and prints out the path. This is helpful for finding specific files in a directory if you know the name of the file.

````
[cs15lwi23apk@ieng6-201]:skill-demo1-data:384$ find written_2/ -name ch1.txt
written_2/non-fiction/OUP/Abernathy/ch1.txt
written_2/non-fiction/OUP/Berk/ch1.txt
written_2/non-fiction/OUP/Fletcher/ch1.txt
written_2/non-fiction/OUP/Kauffman/ch1.txt
written_2/non-fiction/OUP/Rybczynski/ch1.txt
````
The find written_2/ -name ch1.txt command used above recursively searches and prints out the paths of files named ch1.txt within written_2 and its sub folders. This is helpful for finding a specific file when you know the name of the file.

-iname
--------

````
[cs15lwi23apk@ieng6-201]:skill-demo1-data:410$ find written_2/ -iname ch4.txt
written_2/non-fiction/OUP/Berk/CH4.txt
written_2/non-fiction/OUP/Kauffman/ch4.txt
````
The find Abernathy -iname ch4.txt finds the ch4.txt files within written_2 and its subdirectories regardless of capitalization. This is helpful for finding a specific files without knowing the capitlization.

````
[cs15lwi23apk@ieng6-201]:skill-demo1-data:440$ find -iname EMPTY
./emptyDir/empty
````
The find -iname EMPTY command used above recursively searches and prints out the files and directories named empty regardless fo capitlization. 

-type f
------

````
[cs15lwi23apk@ieng6-201]:skill-demo1-data:388$ find written_2/non-fiction/OUP/Berk -type f              
written_2/non-fiction/OUP/Berk/CH4.txt
written_2/non-fiction/OUP/Berk/ch1.txt
written_2/non-fiction/OUP/Berk/ch2.txt
written_2/non-fiction/OUP/Berk/ch7.txt
````
The find written_2/non-fiction/OUP/Berk -type f command used above prints out any files within the Berk directory. This is helpful finding all the files within a specific directory.

````
[cs15lwi23apk@ieng6-201]:skill-demo1-data:390$ find written_2/non-fiction/OUP/Rybczynski/ -type f 
written_2/non-fiction/OUP/Rybczynski/ch1.txt
written_2/non-fiction/OUP/Rybczynski/ch2.txt
written_2/non-fiction/OUP/Rybczynski/ch3.txt
````
The find written_2/non-fiction/OUP/Rybczynski/ -type f command used above prints out only the files within the Rybczynski directory. This is helpful for finding all the files within a directory.

-empty
------

````
[cs15lwi23apk@ieng6-201]:skill-demo1-data:404$ find emptyDir/ -empty
emptyDir/empty.txt
emptyDir/empty
````
The find emptyDir/ -empty command used above prints out the empty directories and files within emptyDir. This is useful for finding any empty directoires or files.

````
[cs15lwi23apk@ieng6-201]:skill-demo1-data:405$ find written_2/ -empty
````
The find written_2/ -empty command used above prints out nothing because the directory written_2 has no empty directories or files. This is useful for making sure non of the files or directories are empty if they are all supposed to have values in them. 

-size
------

````
[cs15lwi23apk@ieng6-201]:skill-demo1-data:448$ find written_2 -size +100k
written_2/non-fiction/OUP/Berk/CH4.txt
written_2/non-fiction/OUP/Berk/ch2.txt
written_2/travel_guides/berlitz1/WhereToFrance.txt
written_2/travel_guides/berlitz1/WhereToIndia.txt
written_2/travel_guides/berlitz1/WhereToItaly.txt
written_2/travel_guides/berlitz1/WhereToJapan.txt
written_2/travel_guides/berlitz1/WhereToMalaysia.txt
written_2/travel_guides/berlitz2/Canada-WhereToGo.txt
written_2/travel_guides/berlitz2/China-WhereToGo.txt
written_2/travel_guides/berlitz2/Portugal-WhereToGo.txt
````
The -size flag used above prints out the paths of the files that are bigger than 100k. This is helpful for finding files or directories greater than a specific size.

````
[cs15lwi23apk@ieng6-201]:skill-demo1-data:454$ find written_2 -size -2k
written_2/travel_guides/berlitz1/HandRIbiza.txt
written_2/travel_guides/berlitz1/HandRIstanbul.txt
````
The -size -2k flag used above prints out the paths of files that are smaller than 2k in size. This is helpful for finding files or directories smaller than a specific size.
