## bash script that simplifies gzip header and `cat`s remaining data from stdin to stdout
```console
$ file ./rfc-gzip.html.gz
./rfc-gzip.html.gz: gzip compressed data, was "rfc-gzip.html", last modified: Mon Feb 10 13:45:14 2003, max compression, from FAT filesystem (MS-DOS, OS/2, NT), original size modulo 2^32 21737
$ /path/to/gzsimp if=./rfc-gzip.html.gz of=./simped.gz
$ file ./simped.gz 
./simped.gz: gzip compressed data, original size modulo 2^32 21737
```