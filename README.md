# rlist
todo list rust in fs

```
A command line to-do app written in Rust

USAGE:
    rlist [OPTIONS] <SUBCOMMAND>

FLAGS:
    -h, --help       Prints help information
    -V, --version    Prints version information

OPTIONS:
    -j, --journal-file <journal-file>    

SUBCOMMANDS:
    add     
    done    
    help    Prints this message or the help of the given subcommand(s)
    list   
3: buy protein         
```

Examples:

```bash
➜  rlist git:(main) cargo run -- -j test.json add "buy milk"
➜  rlist git:(main) ✗ cargo run -- -j test.json add "buy onions"
➜  rlist git:(main) ✗ cargo run -- -j test.json add "buy protein"
➜  rlist git:(main) ✗ cargo run -- -j test.json list
1: buy milk                                           [2021-04-18 21:33]
2: buy onions                                         [2021-04-18 21:33]
3: buy protein         
➜  rlist git:(main) ✗ cargo run -- -j test.json done 2
➜  rlist git:(main) ✗ cargo run -- -j test.json list
1: buy milk                                           [2021-04-18 21:33]
2: buy protein                                        [2021-04-18 21:33]

```
