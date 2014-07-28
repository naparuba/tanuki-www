Title: Installing XXXXXX
Slug: intro/getting-started/install


# Install XXX

XXX must first be installed on every node that will be a member of a
XXX cluster. To make installation easy, XXX is distributed as a
[binary package](/downloads.html) for all supported platforms and
architectures. This page will not cover how to compile XXX from
source.

## Installing XXX

To install XXX, find the [appropriate package](/downloads.html) for
your system and download it. XXX is packaged as a "zip" archive.

After downloading XXX, unzip the package. Copy the `XXX` binary to
somewhere on the PATH so that it can be executed. On Unix systems,
`~/bin` and `/usr/local/bin` are common installation directories,
depending on if you want to restrict the install to a single user or
expose it to the entire system. On Windows systems, you can put it wherever
you would like.

### OS X

If you are using [homebrew](http://brew.sh/#install) as a package manager,
than you can install XXX as simple as:
```
brew cask install XXX
```

if you are missing the [cask plugin](http://caskroom.io/) you can install it with:
```
brew install caskroom/cask/brew-cask
```

## Verifying the Installation

After installing XXX, verify the installation worked by opening a new
terminal session and checking that `XXX` is available. By executing
`XXX` you should see help output similar to that below:

```
$ XXX
usage: XXX [--version] [--help] <command> [<args>]

Available commands are:
    agent          Runs a XXX agent
    force-leave    Forces a member of the cluster to enter the "left" state
    info           Provides debugging information for operators
    join           Tell XXX agent to join cluster
    keygen         Generates a new encryption key
    leave          Gracefully leaves the XXX cluster and shuts down
    members        Lists the members of a XXX cluster
    monitor        Stream logs from a XXX agent
    version        Prints the XXX version
```

If you get an error that `XXX` could not be found, then your PATH
environment variable was not setup properly. Please go back and ensure
that your PATH variable contains the directory where XXX was installed.

Otherwise, XXX is installed and ready to go!
