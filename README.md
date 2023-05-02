Download Link: https://assignmentchef.com/product/solved-cmpsc311-homework-02
<br>
Writing a program on Linux machine (Testing Little Endian)

At the completion of the program, please submit two files to canvas: hw2.pdf

test_endian.c




Hw2.pdf file should contain two screenshots. First screenshot shows that you are logged into the W204 machine, used linux command to change into the directory ~311/hw2handout/ for your hw2, and use pwd and ls command to show where you are. It should look similar to this:




Second screenshot shows that you successfully run the program. It should look something like this. Or if you failed to write a program to pass the test, show us what result you get from running driver program.




Your homework grade is made up by two parts. 5 points for successfully setting up the hw2 files on a W204 machine and compile and run the code, demonstrated by the two screenshots in pdf submission; 5 points for writing correct code in the file test_endian.c. Your program should compile and work with the rest of the files we provided you to build driver program. Your code will be judged by correctness of implementation, style and comment. You may remove the comment or other code we supplied in the function that you don’t need.




Please double check that you submission correctly contained two files (hw2.pdf and test_endian.c) when you are done. We will not take late submissions for any reason/oversight. We will open a new submission as a late submission where you use up to 2 of your 5 grace days. And start early so that you can use help from either the teaching staff or resolve account issues with <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="3159545d415554425a715242541f4142441f5455441f">[email protected]</a>













Part 1: Getting started on a Linux Machine

Please follow these steps to get the homework files into your account on W204 linux machines.




<ol>

 <li>Download ​<strong>tar</strong>​ file from canvas onto your own machine. Make a note of what directory your downloaded file is. It usually is in “yourhomedirectory/Downloads”.</li>

 <li>If you computer is off campus, please connect to vpn.ist.psu.edu with Cisco AnyConnect, using your psu network id and password. Otherwise, proceeds to the next step.</li>

 <li>Login to a W204 machine. At the command prompt, type in these commands

  <ol>

   <li><em>pwd&lt;enter&gt;</em></li>

  </ol></li>

</ol>

This command will show where you are in the system’s tree shape file structure. The root of the tree is the “/” directory. And your home directory is usually of the form “/home/ugrads/abc1234”. In the future you can always refer to your home directory as a “~/”.

<ol>

 <li><em>ls&lt;enter&gt;</em></li>

</ol>

This command (letter El Es) will list what files and directories are in your home directory. If your home directory does not contain a directory (folder) named 311 yet, proceed to the next step, otherwise, skip to step 4.

<ol>

 <li><em>mkdir &lt;space&gt; 311&lt;enter&gt;</em></li>

</ol>

This command will create a directory (folder) named 311 in your current home directory. You should organize all of the course materials from cmpsc311. And in the next step, this would be the destination directory where you are coping files remotely from your own desktop onto machines in W204.

<ol>

 <li>Repeat step b to make sure you now have a directory 311 in your home directory.</li>

</ol>

<ol start="4">

 <li>This is the tricky step, and we will give two different sets of directions for Mac users and Windows users. The goal of this step is to learn how to copy files remotely from your own computer onto w204 computers.</li>

</ol>




Mac users:

Open up a new terminal window. The following steps only works in the terminals that ​<strong>ARE NOT</strong>​ remotely logged into W204 linux machines. You have to use these commands from your local machine.




<ol>

 <li><em>pwd&lt;enter&gt;</em></li>

</ol>

Find out what directory your terminal is in.

<ol>

 <li><em>cd &lt;space&gt; ~/Downloads&lt;enter&gt;</em></li>

</ol>

This is to change your working directory to the Downloads folder where your downloaded tar file is.

<ol>

 <li><em>ls&lt;enter&gt;</em></li>

</ol>

Make sure that hw2handout.tar file is in this directory we are in.

<ol start="33">

 <li><em>scp&lt;space&gt; hw2handout.tar&lt;space&gt; <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="cab3bfbdfbfd8aa9b9afe7baf8fafea3a4b9bef9f9e4a9b9afe4bab9bfe4afaebf">[email protected]</a>:311/ &lt;enter&gt;</em></li>

</ol>

This command is remotely connect to a machine in W204 and copy the file

hw2handout.tar from your local computer to the remote machine, into the directory 311 that we created earlier.

The command will prompt you for your CSE account password. Type in, and even though there is no prompt for your duo-push, you will have to go to your phone to approve the push sent automatically.

When your password is entered and you approved your DUO-push on the phone, you will see something like this:







<ol>

 <li>Congratulations, you have successfully copied the file onto W204’s machines!</li>

</ol>







Windows Users:

Open up a new command window. This can be done by typing “cmd” in the run bar. This is not the terminal from PuTTY that you used to log into W204 machines!

<ol>

 <li><em>dir&lt;enter&gt;</em></li>

</ol>

This is to check if you are in your home directory and if you see the Downloads directory in here.

<ol>

 <li><em>cd &lt;space&gt; Downloads&lt;enter&gt;</em></li>

</ol>

This is to change your working directory to the Downloads folder where your downloaded tar file is.

<ol>

 <li><em>dir&lt;enter&gt;</em></li>

</ol>

This is to check if you have hw2handout.tar file in the Downloads directory.

<ol start="33">

 <li><em>pscp&lt;space&gt;hw2handout.tar&lt;space&gt;<a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="98e1edefa9afd8fbebfdb5e8aaa8acf1f6ebecababb6fbebfdb6e8ebed">[email protected]</a></em></li>

</ol>

<em>.edu:311/ &lt;enter&gt;</em>

This step is assuming that you have already installed PuTTY on your computer, and we are using PuTTY’s secure cp tool “pscp”. If you have installed but the computer complains that it doesn’t recognize the command “pscp”, you will need to add PuTTY’s path into the system. Go to Control Panel -&gt; System -&gt; Advanced System settings -&gt; Environment Variables; add “C:Program FilesPuTTY”; to a new line when you edit Path variable.

This command is remotely connect to a machine in W204 and copy the file hw2handout.tar from your local computer to the remote machine, into the directory 311 that we created earlier.

The command will prompt you for your CSE account password. Type in, and even though there is no prompt for your duo-push, you will have to go to your phone to approve the push sent automatically.

When your password is entered and you approved your DUO-push on the phone,

you will see something like this:




<ol>

 <li>Congratulations, you have successfully copied the file onto W204’s machines!</li>

</ol>




<ol start="5">

 <li>Now we have copied our file to W204 machine, all the following operations will be done in the terminal AFTER you log into a W204 machine.</li>

 <li>Login to a W204 machine. Now change your working directory to 311. <em>cd&lt;space&gt;~/311&lt;enter&gt; </em></li>

</ol>

This command will change your working directory to 311.

<ol start="7">

 <li><em>ls&lt;enter&gt;</em></li>

</ol>

This command will show what you have in the directory. If you have followed earlier steps correctly, you should see hw2handout.tar in the directory.

<ol start="8">

 <li><em>tar&lt;space&gt;xvf&lt;space&gt;hw2handout.tar</em></li>

</ol>

This command will unpack the tar file into a directory that contains all the file you need for hw2.

<ol start="9">

 <li><em>ls&lt;enter&gt;</em></li>

</ol>

Now you should see a directory hw2handout in your folder.

<ol start="10">

 <li><em>cd&lt;space&gt;hw2handout&lt;enter&gt;</em></li>

</ol>

Change the working directory to hw2handout

<ol start="11">

 <li><em>make&lt;enter&gt;</em></li>

</ol>

This command will compile test_endian.c and build an executable file named driver in your directory that you can test your code.

<ol start="12">

 <li><em>./driver&lt;enter&gt; </em></li>

</ol>

Load and run the program driver. If you have edited test_endian.c correctly, it will say:










***************************** Passed all test.

*****************************

At the end of the run.

<ol start="13">

 <li>You will repeat the process of step 11/12 everytime after you edit your test_endian.c program and save it.</li>

</ol>




Part 2: Edit / Compile / Run a program




Complete the function ​is_little_endian​ in the test_endian.c file to check if Dr. Evil’s store function is storing a 4 byte int properly in little endian form.




Dr. Evil implemented many different store functions that will store a 4 byte value into 4 bytes in any arbitrary order. For example, it might store the value 0x12345678 into the memory starting at address 0x1000 as the following:







<table width="624">

 <tbody>

  <tr>

   <td width="156">0x1000</td>

   <td width="156">0x1001</td>

   <td width="156">0x1002</td>

   <td width="156">0x1003</td>

  </tr>

  <tr>

   <td width="156">0x78</td>

   <td width="156">0x56</td>

   <td width="156">0x34</td>

   <td width="156">0x12</td>

  </tr>

 </tbody>

</table>




Which would be in little endian style where the least significant byte is stored at the first location, the second least significant byte in the second location and so on.




Dr. Evil could also store the same value 0x12345678 into the memory starting at address 0x1000 as the following order:







<table width="624">

 <tbody>

  <tr>

   <td width="156">0x1000</td>

   <td width="156">0x1001</td>

   <td width="156">0x1002</td>

   <td width="156">0x1003</td>

  </tr>

  <tr>

   <td width="156">0x78</td>

   <td width="156">0x12</td>

   <td width="156">0x34</td>

   <td width="156">0x56</td>

  </tr>

 </tbody>

</table>




Which is not little endian or big endian.




Dr. Evil’s store function is sent to you to check as a function pointer. You may use the function pointer just as a regular function that takes an int pointer and an int value as arguments. It will store the int value into the 4 byte location pointed to starting at location pointed to by the int pointer. Please make changes to the following code so that your function returns 1 when store is little endian, and 0 otherwise. You can use byte_ptr that is also pointed to at the beginning of x to check for specific byte after value is stored in x.Here is the code you start with.

#include ​”test_endian.h” int​ is_little_endian(​void​ (*store)(​int​*,​int​)) {

​int​ x;

​unsigned​ ​char​ *byte_ptr = (​unsigned​ ​char​*)(&amp;x);   store(&amp;x, ​1​);

​return​ ​0​;

}