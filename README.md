# phantomenv

rbenv, but for phantomjs.

## Installation

To install the latest stable release:

```
git clone -b v0.0.8 https://github.com/wfarr/phantomenv.git ~/.phantomenv
```

Then add the following to your shell config at the end:

```
export PATH="$HOME/.phantomenv/bin:$PATH"
eval "$(phantomenv init -)"
```

## Usage

```
» phantomenv help
Usage: phantomenv <command> [<args>]

Some useful phantomenv commands are:
   exec        Execute a command from a particular PhantomJS version.
   shell       Set PHANTOMENV_VERSION for the lifetime of a shell.
   local       Persist the preferred PhantomJS version in the cwd.
   global      Persist the preferred PhantomJS default version.
   install     Install a version of PhantomJS.
   uninstall   Uninstall a version of PhantomJS.
   version     Show the current PhantomJS version.
   versions    Display all versions of PhantomJS installed in `${PHANTOMENV_ROOT}/versions/*'.
   rehash      Rehash phantomenv shims (run this after installing executables)

See `phantomenv help <command>' for information on a specific command.
```

## Credits

This library was heavily, heavily, heavily inspired by
[@sstephenson](https://github.com/sstephenson)'s
[rbenv](https://github.com/sstephenson/rbenv) and
[ruby-build](https://github.com/sstephenson/ruby-build) projects.
A few ideas were also taken from [nvm](https://github.com/creationix/nvm).

A number of patterns and utilities are borrowed from that project,
and it is my hope that phantomenv provides the same simplicity,
elegance, and usability that I've come to love in rbenv and ruby-build
for PhantomJS users.
