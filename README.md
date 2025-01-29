# Odin Raylib Template

A game template using the `Odin` programming language and the `Raylib` video game library based on the tutorial series by Karl Zylinski.

## Requirements

Download the latest Odin release `dev-2025-01` and extract it to a directory of your choice.

```
wget https://github.com/odin-lang/Odin/releases/download/dev-2025-01/odin-ubuntu-amd64-dev-2025-01.zip
unzip odin-ubuntu-amd64-dev-2025-01.zip
tar -xvzf dist.tar.gz
sudo mv odin-linux-amd64-nightly+2025-01-08 /opt
sudo rm -rf /opt/odin
sudo mv /opt/odin-linux-amd64-nightly+2025-01-08 /odin
rm dist.tar.gz
```

Create a soft link in a `PATH` directory which points to the odin executable.

```
ln -s /opt/odin/odin bin/odin
```

Ensure that odin works as expected.

```
odin
```

Set up to use the following compiler flags
```
-vet -strict-style
```

Install `Clang` which is used for linking:
```
sudo apt install clang
```

## Run

The game can be built and run as follows.

```
odin run ./src -vet -strict-style -out:bin/odin-raylib-template
```

Or simply run the created executable directly.

```
./bin/odin-raylib-template
```

## References

* [Odin programming language](https://odin-lang.org/)
* [Raylib video game library](https://www.raylib.com/)
* [Raylib cheatsheet](https://www.raylib.com/cheatsheet/cheatsheet.html)
* [CLang](https://clang.llvm.org/)
* [Odin + Raylib tutorials](https://www.youtube.com/playlist?list=PLxE7SoPYTef1jYHJ6NxNgocVjQKkq7eEa)
