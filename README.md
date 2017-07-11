# Taaabs-Playground

Client side application for creating and testing taaabs components.

## Required

This application requires [bower](https://bower.io/) to install... Or you can download all the dependencies one by one with git, but you really don't want to do this :)

## How to install

First, clone this repo.

```sh
git clone https://github.com/TaaabsElements/taaabs-playground.git
cd taaabs-playground
```

Then, clone each Taaabs component repo, using the `taaabs-clone-list` file.

```sh
mkdir taaabs-elements
cd taaabs-elements
for f in `cat ../taaabs-clone-list`; do `git clone $f`; done
```

Create a symlink to the `bower_components`.

```sh
mkdir ../bower_components
ln -s ./* ../bower_components/
```

Finally, downlaod the rest of the dependencies with `bower`.

```sh
cd ..
bower install
```

## How to use

Well, launch a server at the root of taaabs-playground. That's it. For example:

```sh
python -m SimpleHTTPServer 3030
```
