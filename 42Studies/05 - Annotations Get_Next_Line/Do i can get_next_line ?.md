<h2 align="center">First thoughts</h2> 
<div>
	<p align="justify-center">First to do this project i have to understand the use of the function open()
	</p>
	<p align="justify-center">
		Then i have to use the function read, whatout to read man, when you read all specfied lenght that you put on read you have to put a null character on final of buff.
	</p>
</div>
<h2 align="center">All bout fds bellow</h2>
<p align="justify-center">Every time i write on fd = 1 i write in an archive in system that holds that content momentarly</p>
![[ls -l of fd.png]]

![[Example_reading_a_file.png]]

To encounter that visualizations on windows you can type lsof -p 'pid of the process'

<h3 align="center">Final result turns like that</h3>
![[fd with a file extra.png]]

<h3 align="center">Files descriptor in linux</h3>
![[all about fd.png]]

<p align = "justify-center">The image above it shows how fds are on system, they are of type c that is equal to xxxxx, with that you can note that everything on linux is a file.</p>
	<h3 align="center" >Functions needed and its mannuals</h3>
<h4 align="center">Read()</h4>
https://man7.org/linux/man-pages/man2/read.2.html

![[man_read.png]]

<p>The read func holds the last position readed so it can read from the start of the last pos holded, like example bellow</p>
![[ex_read_func.png]]

<h4 align="center">Malloc()</h4>
![[man_malloc.png]]

<h4 align="center">Free</h4>
![[free.png]]

Parei de ver na parte do linked list