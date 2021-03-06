Q-OS
====


Q OS is a versatile operating system designed with the new features of 64 bit "long mode" CPU's in mind that focuses on making everything as simple as possible for the end user. In designing it and, now, coding it, I have taken every aspect of what we consider to be a "Good OS" and removed everything that people find distracting and, in the end, symply useless.


By studying inexperienced people using operating systems such as Linux Distributions and the popular Windows and OS X systems through sources such as the OSFirstTimer channel on YouTube, I have decided on three key features that I will implement into Q OS as some of the key differences from current operating systems. Q OS is built from scratch using the Assembly language for the bootloader and parts of the kernel as well as C++ for the most part of the code. The main unique features I will be implementing into Q OS are as follows:


Tiny Files
----------


When we program in the 21st Ceuntry, we have so much more processing power and resources avalable than in the early days of computing that we often waste large portions of storage and CPU power just by writing inefficient and messy code. As computers continue to get more powerful, so will the level of inefficiency in a typical program such as a word processer where the programmers will save time while developing the software by writing - as I mentioned before - inneficient code that has no benifit whatsoever to the end user. 


If we, as programmers, continue to let our code become more inneficient just because we are able to with such powerful computers that are avalable to nearly everybody in the world now, computers will have to cost more than they are actually worth because of the excessive computational power and storage space they will need to cope with such inneficient programming. An example of this incredible waste of storage space can be seen in how an entire program used to fit within a 64KB space on a disk, but now you can't even write a letter in that amount of space using a word processer such as Microsoft Word or Apple's 'Pages'. Obviously, applications have became more advanced, but so has the languages we have avalable to use to create them with. Theoretically this should allow us to create more advanced programs in only a little more space, but our bad habits as programmers have prevented this from happening.


In Q OS, I aim to solve this problem in two main ways. The first of which is by giving any computer with a freshly installed copy of Q OS (when it is complete) built in programs that suit most people's needs in computing such as a word processor, web browser, presentation and chart creation programs and other typical preinstalled software, but the entire package of built-in apps will all fit within less than a 1GB space. This is not even a very hard goal to acomplish when the right routines and programming habbits are adopted in order to create tiny code files.


Logical Extensions
------------------


For a long time, our files have been appended with what we know as a "File Extension". This is a simple, typically three leter long abbreviation that tells the computer what kind of file it is - for example, .jpg indicates a kind of photo, .mov is a video encoded with Apple's "QuickTime" encoder, .doc is a text document made using the "Microsoft Word" software, and so on.


But to an inexperienced computer user, what do all these extensions mean? I surveyed a random selection of around 100 people living in Melbourne, where I live, and less than 20 of them had any clue what the file extensions after a file actually mean. Even worse, less than 10 were able to translate certain extensions into what they meant!


Obviously this is not an ideal setup. In Q OS I am going to solve this by creating logical file extensions that are easy to understand even to someone who has only just touched a computer for the first time, and store the actual file type in the old format with three leter extensions only in the metadata of the file. Advanced users will be able to see the origional file extensions, but the file type itself is a completely different structure than in current systems so adapting to my design is a much better option if you plan to use Q OS for any extended period of time. 


Some examples of my Logical Extensions are .photo for any photo file no matter if it is a photoshop file, a vector image, a .png image or any other kind of still picture, it will have the .photo extension. .movie is for anything that moves. Animations, .gif's, Films, Movies and more are considered a moving picture format and will be .movie. .code is a powerful new extension for us programmers. Whilst some programmers will be apprehensive to use this at first, it lets programmers and developers define the programming language, version and other metadata at the top of the file and also helps make your folders of code look neater and more beautiful with the same extension for every code file, from binary to html. There are many other Logical Extensions that I will be implementing into Q OS and I belive they will make file managment much easier.


Terminal Rethought
------------------


After over a decade of Unix-style terminals, many users will have began to discover the limitations of command line interaction with your computer. In Q OS, I am redesigning the command line interface from the ground up. This begins with over 2000 brand new commands. The most powerful of any of these is arguablely the new <code>do</code> command, however. Here is a brief example of what this powerful command lets you do with the forthcoming Q OS Terminal:


<code>do js for(i=0;i<10;i++) { console.log(i); }</code><br>
This is using the all new <code>do</code> command to execute javascript inside the terminal. The syntax for the <code>do</code> commmand is as follows:<br>
<code>do language code</code><br>
Although the <code>do</code> syntax itself is simple to use, what you can create with <code>do</code> is incredible. The Terminal now allows you to create and store variables that are stored in memory until you close the window. But that's not even the best part. The <code>do</code> command supports a huge number of programming languages. Examine this command:<br>
<code>do asm add eax, ebx</code><br>
Yes, Q OS even supports running Assembly Language code directly in the Terminal. All this power is possible by intergrating multiple language compilers into the Terminal that run when the correct <code>do</code> syntax is supplied by the user and generate an output when nessesary.
