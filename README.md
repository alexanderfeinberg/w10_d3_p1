# Practice: SQLite3 CLI

Now, you will practice using the Command Line Interface (CLI) in SQLite3.

## Getting Started

Download starter. `cd` into the __sql-practice__ folder.

As you work, write down any questions you have for the upcoming discussion
session.

## Step 1: Use built-in documentation

Run `sqlite3`. You can begin with no database.

> Tip: Notice the prompt changes to "sqlite>". That's how you know you will be
> able to run SQL statements and SQLite3 commands.

You can view the available commands for SQLite using `.help`. Run this
now and look for the commands to

* View the list of tables
* View the table schema

Write down what you found. You'll need to use them in the next section.

Exit the CLI.

> Tip: If you can't remember the keyboard shortcut you can look again at the
> built-in documentation to see if there is a command for exiting the CLI.

## Step 2: Run `sqlite3` to explore a database

Start SQLite on a new database named __example.db__.

View the tables in the database by entering the command you found in Step 1.

View the schema of the database by entering the command you found in Step 1.

> Think about it: Do you know why you don't find any tables or schema?

Run the command `.read example.sql`. This will execute the SQL in the
__example.sql__ file.

Repeat the command for viewing the tables in the database. You should see

```plaintext
samples
```

Repeat the command for viewing the schema of the database. You should see

```plaintext
CREATE TABLE samples (id INTEGER PRIMARY KEY AUTOINCREMENT, name TEXT);
CREATE TABLE sqlite_sequence(name,seq);
```

Finally, run a simple query to see the data in the samples table by entering

```sql
SELECT * FROM samples;
```

This should show you

```plaintext
1|You found me!
2|Yippee!!
3|Yay!!!
```

## Exit the CLI

Use `Ctrl+d` to exit the cli.

> Tip: Now your prompt should return to normal, which probably means it ends
> with "$".

Congratulations! You have successfully used the SQLite3 CLI.