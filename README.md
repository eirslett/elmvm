# ELMVM - Elm Version Manager

This is a utility, similar to nvm (Node.js Version Manager) which
lets you have multiple versions of the Elm platform installed, and
switch between them easily.

The project is inspired by [Node Version Manager (nvm)](https://github.com/creationix/nvm).

##### Supported operating systems

MacOS is supported. (not tested on Linux yet)

## Installation

Some basic knowledge about the terminal, bash and terminal configuration is assumed.

- Download the `elmvm` script (or `git clone` this repository)
- Run `source path/to/elmvm` in the terminal. (using the path where you put the script)

You can do the `source` command inside `.bash_profile` if you want to load it automatically
in every terminal session.


## Usage

`elmvm --help` will show you how commands can be used.

#### List of Elm versions you have installed

```
$ elmvm ls
0.15.1
0.16
0.17
0.17.1
0.18
```

#### List of Elm versions available online

```
$ elmvm ls-remote
0.18
0.17.1
0.17
0.16
0.16.0
master
0.15.1
```

#### Installing a version of Elm

```
elmvm install 0.18
```

#### Activating a specific version of Elm

```
elmvm use 0.18
```

Running the `elm` command should now include which version of Elm is active.
Note that the elm version will only be active for the current terminal session, it's not
persisted between sessions. (Support is not implemented yet)

### Contributing

Send pull requests.

### License

Apache 2.0
