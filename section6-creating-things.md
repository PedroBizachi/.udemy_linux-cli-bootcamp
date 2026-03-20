# Making Files And Folders Exercise

To get some practice creating files and folders from the command-line, we'll be creating a standard React project file structure. Don't worry at all if you don't know React, we're just making a bunch of empty files and folders!

1. Create a new folder called `my-app`
2. Navigate to `my-app` and inside create two new empty files called `README.md` and `package.json`
3. Still inside of `my-app` create a new folder called `public`. Without `cd`-ing into `public`, create an `index.html` file inside of it.
4. Create a new folder called `src` inside of `my-app`. Navigate inside of it.
5. Using a single line, create the following four files inside of `src`: `App.css`, `App.js`, `index.css`, and `index.js`

Your folder structure should now look like this:

```bash
my-app/
  README.md
  package.json
  public/
    index.html
  src/
    App.css
    App.js
    index.css
    index.js
```

### BONUS

<aside>
💡 Using a single command, create a new directory inside of `src` called `components`, and inside of that new `components` directory create a new directory called `Navbar`.   Do this using a single command, without first creating the `components` directory.

</aside>

Your folder structure would now look like this:

```bash
my-app/
  README.md
  package.json
  public/
    index.html
  src/
		**components/
			Navbar/**
    App.css
    App.js
    index.css
    index.js
```
