# Working With Files Exercise

[[FilesExercise.zip](http://filesexercise.zip)](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/8c10648f-ff91-46f3-a922-a2c4983c10d1/FilesExercise.zip)

Once you have downloaded the above zip file, unzip it! It contains two files: `poem.txt` and `purchases.txt`

## Part 1

- Use a command to print out the entire contents of the `poem.txt` file. Use an option so that the output also includes line numbers.
  - R: I can use `cat -n poem.txt` to print the entire contents of the poem with line numbers, it printed 132 lines.
- That is a headache to read all at once! Read poem.txt using `less` instead.
  - Scroll down one line at a time
    - R: With `down arrow`
  - Scroll up one line at a time
    - R: With `up arrow`
  - Scroll down one "page" at a time
    - R: With `f` key.
  - Scroll up one "page" at a time
    - R: With `b` key.
- Search within less for the term "Dog". Can you find the line that contains it?
  - **BONUS:** can you run a case-insesitive search? The poem contains both "dog" and "Dog" on separate lines.
    - R: I can use the command `less -i poem.txt`. That option will ignore case when doing searches on the file, so i can run the command `/dog` and find both "dog" and "Dog".
- Now it's time to do some research! Find the option to tell less to open with lines numbers displayed. Open `poem.txt` this way
  - R: Using the option `-N` i can see the lines numbers being displayed.
- Then find the "command" you can type into less to go to exactly 50% of the way through the file.
  - R: I can just type `:50%` to go half way through the file.
- Use a command to find the number of **words** in `poem.txt`
  - R: I can use `wc --words poem.txt` to find 839 words in that file.
- Run a command to print out the first 4 lines of `poem.txt`
- Run a command to print out the last 8 lines of `poem.txt`

## Part 2

- Run a command to print out the lines in `purchases.txt` in reverse order (last line printed first)
- Run a command to print out the lines in `purchases.txt`, sorted alphabetically.
- Run a command to count the number of **lines** in `purchases.txt`
- Run a command to print out the lines in `purchases.txt`, sorted by the price (the final column) in the dataset in REVERSE order (highest price to lowest price)
