# Redirection Exercise

Download the files for this exercise:

[Wildlife.zip](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/5347afb9-a379-4ccc-a6a7-25da129f3ad0/Wildlife.zip)

Unzip the `Wildlife` folder and navigate to it via the command line.

## Your Task

You are taking part in a wildlife survey in a remote portion of the Peruvian Amazon! This morning, three of your research assistants each went on transect walks where they recorded the individual species they observed. Your (simple) job is to combine their findings into a new file that contains all the species that were observed!

1. Create a new file called `all-species.txt` that contains the combined contents of `angela-survey.txt`, `nico-survey.txt`, and `juan-survey.txt`. Do this using a single command!
   1. R: I could do that by using `cat stdin > stdout` where stdin is all the three surveys and stdout is the all-species.txt file.
2. The problem with the `all-species.txt` file is that it contains duplicate entries! Use a single command to sort the lines in alphabetical order, only sorting uniques, and send the output to a new file called `sorted-animals.txt`
   1. R: I could do that by using `sort -ud all-species.txt > sorted-animals.txt`. The `-ud` options allow me to sort only unique values in a dictionary order (alphabetically), and i redirect the output (stdout) to a new file as requested.
3. Now, you go out for a nice morning stroll and stumble upon a large anaconda sunning itself on a log. You should add this observation to the list of species!!
   1. Start by appending the current date to the end of the `sorted-animals.txt` file using a command (don't open the file manually!)
      1. R: I've used the command `date >> sorted-animals.txt` to do that.
   2. Then append the text "Green Anaconda" to the end of `sorted-animals.txt`
      1. R: I've used the command `echo "Green anaconda" >> sorted-animals.txt` to do that.
4. Run the non-existent command `ughhh` and redirect any error messages so that they are **appended** to the sorted-animals.txt file.
