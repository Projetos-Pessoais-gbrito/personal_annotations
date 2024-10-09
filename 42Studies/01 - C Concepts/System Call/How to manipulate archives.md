To manipulate archives in c, first we have to use open, like the example bellow:
```c
	fd = open(filename, O_RDONLY)
	Open function has three flags to open the archive, see the example bellow:
	O_RDONLY
	O_WRONLY
	O_RDWR
```
When we use open we can say, that we are asking to the system to borrow for a minute the capacity to manipulate.

#### File table entries

![[Pasted image 20241008235159.png]]

Fd has 3 possibles outs, 0 standard-input, 1 standard-error, 2 standard out

stdin -> read from fd 0 -> Whenever it reads from stdin through fd 0 and saves o a file named /dev/tty

stdout -> fd -> 1. Every thing is from video screen and written to stdout in screen.

stderr -> fd -> 2. We see any error on the video screen

#### Open()

If we open one more archive, that archive will come out with 3, that's the new out.

```c
	open("./path/text.txt", O_RDONLY);
```
Check out the website bellow for more contents: [Geeks for Geeks](https://www.geeksforgeeks.org/input-output-system-calls-c-create-open-close-read-write/)

How C open file in OS
- Find the existing file
- Creeate file table entry
- Set the first unused descriptor
- Return -1 in case of error

#### Read()

Right after we open the archive we do have to **read**, o use that function, we have to do like the example bellow:

![[Pasted image 20241009081552.png]]

In case of sucess read returns the size of archive in bytes.

See example bellow in C
```c
	size_t cnt = (char *)calloc(100, sizeof(char));
	char buf[cnt];
	size_t bytes_readed;
	
	while(bytes_readed = read(fd, buf[cnt], cnt) > 0)
	{
		printf("Those bytes are as follows:" %s\n", c);
	}
```

Possible returns
- return Number of bytes read on success
- return 0 on reaching the end of file
- return -1 on error
- return -1 on signal interrupt
#### Close()

Its important to use the **Close** function when we are working with files

Close function destroy the file entry that we reserved to open the archive.
Set the file descriptor table to NULL.

The return value on fd is **0** in case of success and **-1** in case of error.





