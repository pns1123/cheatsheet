##### append output of command to file
```
command >> file
```

##### overwrite file with output of command
```
command > file
```

##### compute SHA-256 checksum of file
```
shasum -a 256 file
```

##### extract archive.tar.gz
- x stands for extract
- f stands for file; specify filename after f
- v (optional) stands for visible and prints extracted files
- z (optional) use gzip
- tar stands for Tape ARchive
- a tarball or .tar file is a collection of files wrapped up in a single file for easy storage
- tarballs are often compressed, e.g. with gzip; these compressed tarballs have the .tar.gz extension
- when extracting compressed tarballs the tar command will recognize the compression algorithm 
```
tar -xf archive.tar.gz
tar -xvf archive.tar.gz
tar -xvzf archive.tar.gz
```
