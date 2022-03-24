
# Student Data Management System

Using basic C++ functions and File handling. 
First we create a class named Student in which we declare some variales and some class
functions.Then we start with the main function in which first we use setprecision() sets
the decimal precision to be used to format floating-point values on output operations then 
basic information is printed. By using the switch method we differentiate the functions such 
create_student_record, search_student_record etc. These functions called as per input.

Here we use iomanip header file which The header <iomanip> is part of the Input/output library 
of the C++ Standard Library. It defines the manipulator functions resetiosflags(), setiosflags(), 
setbase(), setfill(), setprecision(), and setw(). These functions may be conveniently used by 
C++ programs to affect the state of iostream objects. 

We use <fstream> This header file includes the definitions for the stream classes ifstream, 
ofstream and fstream. In C++ file input output facilities implemented through fstream.h header 
file. • It contain predefines set of operation for handling file related input and output, fstreamclass 
ties a file to the program for input and output operation.

#File Mode

1) ios::out :- It open file in output mode (i.e write mode) and place the file
pointer in beginning, if file already exist it will overwrite the file

2) ios::in :- It open file in input mode(read mode) and permit reading from the file. 

3) ios::app :- It open the file in write mode, and place file pointer at the end of file i.e to
add new contents and retains previous contents. If file does not
exist it will create a new file.

4) ios::binary :- Opens a file in binary mode.


#File.write(reinterpret_cast<char *> (&stud), sizeof(student))

File.read(reinterpret_cast<char *> (&stud), sizeof(student)) Reads the student structure data directly 
from a file into the memory occupied by st. The cast is because read expects a char*, and this 
is how you convert a pointer of one type to a pointer of a completely unrelated type. Such code will 
only work when the file is written to and read from in binary mode, not to mention you pretty much have 
to create the file and read it on the exact same machine to be certain it will work as expected.
