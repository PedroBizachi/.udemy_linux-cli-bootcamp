# Piping Exercise

Download the starter files here:

[PokemonExercise.zip](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/65520ea7-129d-4e78-9719-69bfbb7c66e0/PokemonExercise.zip)

Unzip the file. The resulting folder contains a subfolder called `PokeDex/` which in turn contains a whole bunch of files, each named for a specific Pokemon like:

```bash
PokemonExercise/
	PokeDex/
		100Voltorb
		101Electrode
	  619Mienfoo
		...
```

## Your Task

Complete the following challenges using the starter files. Make sure that you navigate to the `PokemonExercise/` directory, **but do NOT run any of the following commands from inside the `PokeDex/`** folder. I repeat: any files that you create for the exercise should live inside of `PokemonExercise/` NOT `PokeDex/`

- Count the number of Pokemon files in the `PokeDex/` folder. You'll need to combine commands to make this work!
  - R: I can simply run `ls PokeDex/` and pipe the results to `wc -l`, so the final command will look like this `ls PokeDex/ | wc -l` and it will give me the result of 719 Pokemon.
- Next, create a new single file called `all-pokemon.txt` in the `PokemonExercise` folder (NOT the `PokeDex` folder)that contains the LOWERCASED name of every single Pokemon file in the directory, sorted in numerical order! The end result should look like this:
  - R: I little more complicated, but possible. First i again need to list the files using `ls PokeDex/`, pipe the result to a numerical sort with `sort -n`, then pipe again to the `tr A-Z a-z` command to change upper to lower case, so i can redirect the final result to the specified file. The final command should look like `ls PokeDex/ | sort -n | tr A-Z a-z | cat > all-pokemon.txt`.

```bash
1bulbasaur
2ivysaur
3venusaur
4charmander
5charmeleon
6charizard
7squirtle
8wartortle
9blastoise
10caterpie
11metapod
12butterfree
...
```

- Now that we have this file that includes all the Pokemon in numerical order, let's print out the three pigeon-related Pokemon: pidgey, pidgeotto, and pidgeot. Using the command-line, print out lines 16-18. It should look like this:

```bash
16pidgey
17pidgeotto
18pidgeot
```

- Next, up let's isolate the original 151 Pokemon. Using a single pipeline...
  - output the first 151 lines of the `all-pokemon.txt` file
  - remove all digits 0-9 from the lines (using `tr` )
  - sort the now number-less lines alphabetically
  - store the new result in a file called `original-151.txt` in `PokemonExercise`
  ```bash
  abra
  aerodactyl
  alakazam
  ...
  wigglytuff
  zapdos
  zubat
  ```
