# Expansion Exercise

## Part 1 - Making Some Files

1. Create the following 60 files **using a single command** with the powers of expansion!
   1. I've used the command `touch {morning,afternoon}-day-{1..30}` to complete this task.

```bash

morning-day-1
morning-day-2
...
morning-day-30

afternoon-day-1
afternoon-day-2
...
afternoon-day-30
```

2. For this next bit, you'll need to use the following command: `date +"%m-%d-%y"` This command will print out the current date using the format _month-day-year_, like **09-19-21**. Use this command to create a new file with the name **_todos-DATE.txt_**, where DATE is the output of the above date command. For example, if we ran the command on September 19th 2021, the resulting file would be named `todos-09-19-21.txt`.
   1. I've used the command ``touch todos-`date +"%m-%d-%y"`.txt`` to complete this task.

## Part 2

Using the files that we created in the previous section...

- List out all the files that end with the number `9`
  1.  I've used the command `ls *9` to complete this task.
- List out all the filenames where the second to last character is `1`
  1.  I've used the command `ls *1?` to complete this task.
- List out all the files that start with afternoon and then end with the number `7`
  1.  I've used the command `ls afternoon*7` to complete this task.
- Make a new folder called `Mornings`, and move all the files that start with `morning` inside of it.
  1.  I've used the command `mv morning* Mornings/` to complete this task.

## Part 3

- Using a SINGLE command (with expansion), create the following folder structure. You will need to use the `-p` option with mkdir!

```bash
Year/
	Winter/
		Yard/
		House/
	Spring/
		Yard/
		House/
	Summer/
		Yard/
		House/
	Fall/
		Yard/
		House/
```

1.  I've used the command `mkdir --parents Year/{Winter,Spring,Summer,Fall}/{Yard,House}` to complete this task.

- Finally, in each of the `Yard/` and `House/` Directories create a `todos.txt` file and a `done.txt` file. Do this with a single line, without changing directories! Use expansion! The resulting folder/file structure should look like this:

```bash
Year/
	Winter/
		Yard/
			todos.txt
			done.txt
		House/
			todos.txt
			done.txt
	Spring/
		Yard/
			todos.txt
			done.txt
		House/
			todos.txt
			done.txt
	Summer/
		Yard/
			todos.txt
			done.txt
		House/
			todos.txt
			done.txt
	Fall/
		Yard/
			todos.txt
			done.txt
		House/
			todos.txt
			done.txt
```

1.  I've used the command `touch Year/{Winter,Spring,Summer,Fall}/{Yard,House}/{todos,done}.txt` to complete this task.
