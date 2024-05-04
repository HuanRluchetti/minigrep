# minigrep - Word Searcher in Files

This is a Rust command line application called "minigrep" designed to search for a word in an existing file and return the lines where that word appears.

## How to Use

### Search for a word in an existing file
```sh
cargo run body -- poem.txt
```

### Search while ignoring the case of letters
To search while ignoring the case of letters, use the IGNORE_CASE environment variable and assign the value 1 to it.
```sh
IGNORE_CASE=1 cargo run -- to poem.txt
```

### Save the search result to an existing file
```sh
cargo run -- body poem.txt > output.txt
```

### Create a new file via command line
To create a new file via the command line:
```sh
cargo run > new.txt
```
 
## Main Commands
- `cargo run <word> -- <file.txt>`: Searches the specified word in the provided file and displays the corresponding lines.
- `IGNORE_CASE=1 cargo run -- <word> <file.txt>`: Searches the word in the file, ignoring the case of letters.
- `cargo run -- <word> <search-file.txt> > <result-file.txt>`: Saves the search result to an existing file.
- `cargo run > new.txt`: Creates a new file via the command line.

##
Let me know if there's anything else you need!

