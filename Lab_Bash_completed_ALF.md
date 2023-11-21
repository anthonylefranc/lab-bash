Lab-Bash - ALF


    1/Using the echo command print in console "Hello World". Here is some info about echo command [https://discuss.codecademy.com/t/what-are-practical-uses-of-the-echo-command/394788]

    	echo "Hello World"

    2/Create a new directory called new_dir.

    	mkdir new_dir
    
    3/Delete/Remove the directory new_dir.

    	rm -rf new_dir
    
    4/Copy the file sed.txt from the lorem folder and paste it to the folder lorem-copy folder.

		cp lorem/sed.txt lorem-copy/

    5/Copy the other two files from the lorem folder to lorem-copy folder in just one line using semicolon ;.

    	cp lorem/sed.txt lorem-copy ; cp lorem/lorem.txt lorem-copy

    6/Show the sed.txt file content from the lorem folder.

    	cat sed.txt

    7/Show the at.txt file and lorem.txt file contents from lorem folder.

    	cat at.txt ; cat lorem.txt

    8/Print the first 3 rows in sed.txt file from lorem-copy folder.

    	head -3 sed.txt

    9/ Print the last 3 rows in sed.txt file from lorem-copy folder.

    	tail -3 sed.txt

    10/ Add Homo homini lupus. at the end of sed.txt file in the lorem-copy folder.

    	echo "Homo hominis lupus" >> sed.txt

    11/ Print the last 3 rows in sed.txt file from lorem-copy folder. You should see Homo homini lupus..

    	tail -3 sed.txt

    12/ sed command is used to replace the text in a file. Use the sed command to replace all occurances of et with ET in the file at.txt file present in the folder lorem. You can use the following link to refer to sed commands [https://www.linode.com/docs/guides/manipulate-text-from-the-command-line-with-sed/] Check the contents of the sed.txt file using cat command.+

    	sed -r -i.bak 's/et/ET/g' at.txt
    
    13/ Find who is the system user.

    	whoami

    14/ Find the current path of the directory you are in.

    	fwd

    15/ List all files with the extension .txt in lorem folder.

    	grep '.txt' lorem

    16/ Count the rows in sed.txt file from lorem folder. Look concatenate cat and wc with the pipe |.

		cat lorem/sed.txt | wc -l

    17/ Count the files which start with lorem in all directories.

    	grep 'lorem' -a -R

Bonus

    18/ Store your name in a variable with read command.

    	read -p "Enter my name: " antho_name

    19/ Print that variable.

		echo $antho_name

    20/ Create a new directory named with variable name.

    	mkdir "$antho_name"

    21/ Remove that directory.

    	rm -rf "$antho_name"git add 
