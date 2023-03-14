# Lab Report 5
In this lab, I will show my finished grade.sh and demostrate how it works on different files. 

## bash script
This is what my bash script looks like after I finished:
![Image](script.png)

It has the following funcitons:
1. Clone the repository of the student submission to a directory name. 
![Image](script1.png)

2. Check that the student code has the correct file submitted, and also give correct messages.
![Image](script2.png)

3. Get the student code and the test file into the same directory using the ```cp``` command.
![Image](script3.png)

4. Compile the test and student's code with the appropriate classpath commands. Also, give correct messages if either compilation is successful or fails.
 
![Image](script4.png)

5. Run the tests and report the grade or the error messages based on the Junit output. 
![Image](script5.png)

## Examples
I tried several example files to show that the grade.sh works. 
I first typed ```bash grade.sh``` and copied ```https://github.com/ucsd-cse15l-f22/list-methods-corrected``` into the terminal, and the output I reveived is as follows:
![Image](eg1.png)
It shows that the desired file is found in the student's submission, the file successully compiled, and the test all passed. 

Then I tried a different submission: ```https://github.com/ucsd-cse15l-f22/list-methods-compile-error``` into the terminal. The screenshot below is the output I got:
![Image](eg2.png)
It shows that the file is found but could not successfully compiled because of an syntax error in the line ```result.add(0, s)```. It also prints out the error messages in the terminal. 

I also tried the submission ```https://github.com/ucsd-cse15l-f22/list-methods-filename```. It also as an error in it.
![Image](eg3.png)
The messages printed out in the terminal shows that the file name cannot not be found, meaning that in the file name that the student submitted does not match the required file name. 

Overall, the bash script gives the right output for several different student's submissions. 
