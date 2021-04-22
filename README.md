Iptables-graph
======================

Tools for iptables to generate call graph.

Example Command
---------------------

Generate iptables of your local linux in graphviz graph foramt.

```
$ sudo iptables-save | ./iptables-graph
digraph {
    graph [pad="0.5", nodesep="0.5", ranksep="2"];
    node [shape=plain]
    rankdir=LR;
...
```

Test Command
---------------------

Generate iptables graph to svg file.

```
$ cat example.txt | ./iptables-graph > a.dot
$ dot -Tsvg a.dot -o a.svg
```
