# Assingment-2_Llerena
Assignment #2 -  PROGRAMMING WITH PYTHON 2

This is a project to generate random passwords with certain restrictions I have set myself. 
It consists of two functions, `memorable_generation` and `random_generation`, neither of which takes any arguments to run. 

The program begins with a user input that is designed to simulate a path selection for these two functions, so it only accepts ‘1’ and ‘2’ as valid responses.


“Memorable Generation” begins with a numeric input in the range [2, 6]; I set this rule myself to avoid having passwords that are too long. Next, the text file is opened to add all the words to an empty list called `word_list`. Using `random.sample`, you can select `n` words from the list. f{w}... was used to put a random single digit at the end of each word, `“-”.join` is used to concatenate the words into a single string. 

"random_generation" generates the password character by character, including letters, digits, and punctuation [sometimes]. It works much the same way when taking input. A number between [4, 12] is allowed, but the user is then asked if they want to include punctuation in the password. A “yes” response is expected if so. Since the generation is random with repetition, `random.choices` is used, and finally, the elements are concatenated.

Finally, an additional function for saving the password, called `save_progress`, was developed and implemented at the end of the previous two functions. It takes the directory name as its first argument, which varies depending on the function. The second argument is the name of the text file, and finally, the password is passed to it.
