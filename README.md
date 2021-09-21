# Rust Markdown to graph
This program converts a Markdown file into a graph. For now, it only creates .dot file which graphviz uses to build graph.

It translate headings in a Markdown files into graph nodes and levels into edges. That is, children headings are adjacent to a parent heading.

## Example
If you have the following simple Markdown file, the program would create a dot file, which in turn can be converted in the following image using graphviz command line.

> # H1
> ## H2_1
> ## H2_2
> ### H3_1
> #### H4_1
> #### H4_2
> ##### H5
> H is an abbreviation of Heading.

![Sample image](./examples/test.jpg)

## Caution
In this moment, for some reasons this program fails to handle README.md, so if you will try it, please use some other Markdown files.