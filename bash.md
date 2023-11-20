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

##### list all file with extension .example
```
ls | grep \\.example
```

##### create directories dir1...dirNUM 
```
mkdir dir{1..NUM}
```

##### print human overview of disk usage 
- df stands for disk free
```
df -h
```

##### print unix time
```
date +%s
```

##### set ENV_VAR to "ENV_VAR" [no spaces!] for current shell
```
ENV_VAR="ENV_VAR"
```

##### set ENV_VAR to "ENV_VAR" [no spaces!] for current shell and all processes launched from it
- to set permanently for all future bash sessions add this to ~.bashrc
```
export ENV_VAR="ENV_VAR"
```

##### print values of environment ENV_VAR_1, ENV_VAR_2, ..., ENV_VAR_N 
- to print all env key value pairs omit arguments
```
printenv ENV_VAR_1, ENV_VAR_2, ..., ENV_VAR_N
```
