# egypt

Egypt is a simple tool for creating call graphs of C programs. Egypt neither analyzes source code nor lays out graphs. Instead, it leaves the source code analysis to GCC and the graph layout to Graphviz, both of which are better at their respective jobs than egypt itself could ever hope to be. Egypt is simply a very small Perl script that glues these existing tools together.

You will also need [gcc](http://gcc.gnu.org/), [Perl](http://www.perl.com/), and [Graphviz](http://www.graphviz.org/).

The most recent release of original egypt (version 1.10) can be downloaded [here](http://www.gson.org/egypt/download/egypt-1.10.tar.gz).

To install, extract the compressed tar file, cd to the egypt directory, and type:
```
perl Makefile.PL
make
make install
```
or simply
```
install.sh
```

Then, for documentation type
```
man egypt
```
or
```
perldoc egypt
```
for additional information.

Here is an example of a call graph generated using egypt:
![example](https://raw.github.com/vasilenkos/egypt/master/output_sample.png)
