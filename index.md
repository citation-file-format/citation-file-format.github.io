---
---

{% include toc %}

# What is a `CITATION.cff` file?

`CITATION.cff` files are plain text files with human- and machine-readable citation information for software.
Code developers can include them in their repositories to let others know how to correctly cite their software.

A `CITATION.cff` file looks like this:

{% highlight yaml %}
cff-version: 1.1.0
message: If you use this software, please cite it as below.
authors:
  - family-names: Druskat
    given-names: Stephan
    orcid: https://orcid.org/0000-0003-4925-7248
title: "My Research Software"
version: 2.0.4
doi: 10.5281/zenodo.1234
date-released: 2017-12-18
{% endhighlight %}

The format of `CITATION.cff` files is the **Citation File Format (CFF)**.

# Why you should add a `CITATION.cff` file to your repository!

It is very easy to *correctly* cite a paper: all the necessary information (*metadata*) can be found on the title page or the article website.
Software has no title page, the relevant information is often less obvious.

People who want to cite your software may ask questions like:

<i class="fa fa-question-circle"></i> What is the name of the software (given that it’s probably not `my_scripts/run.m` or `analysis.py`)?
{: .notice--info}

<i class="fa fa-question-circle"></i> What label should I use to uniquely identify the version of the software I have used?
{: .notice--warning .text-right}

<i class="fa fa-question-circle"></i> What is the appropriate set of people that should be identified as authors?
{: .notice--success}


The person who wants to cite your software will probably not be able to answer these questions accurately and consistently themselves, but you can!
Give them all the right information in a `CITATION.cff` file, and they can cite your software correctly.

Also, if you publish your software in an archive or registry, they (or their systems) can re-use the citation metadata from your `CITATION.cff` file as well.

# Create a `CITATION.cff` file now!

You can start by copy-and-pasting the [example above](#what-is-a-citation-cff-file) into the root fo your code repository, and adapt the information to your software.

You can also use a simple website to fill in the citation information for your software.
To do so, go to the [TODO `cffinit` website]().

You can also learn more about the *Citation File Format (CFF)*, which is the format used for `CITATION.cff` files.
It can do more than you can see in the example.
To learn about the format, go to the [Citation File Format documentation](https://github.com/citation-file-format/citation-file-format/blob/master/README.md).

# Tools for working with `CITATION.cff` files

Different tools exist to help you work with `CITATION.cff` files:

- The **initializer** can help you create a `CITATION.cff` file from scratch: <https://citation-file-format.github.io/cff-initializer-javascript/>.
- The **validator** checks whether a `CITATION.cff` file is formatted correctly: [TODO link].
- The **converter** can create a `CITATION.cff` file from existing metadata (e.g., from a *BibTeX* file), and convert it to other formats (e.g., to *BibTeX*, *RIS*, *CodeMeta*, and others): <https://github.com/citation-file-format/cff-converter-python>.
- The **schema** ultimately defines *what* can go into a `CITATION.cff` file, and *how*: [TODO link].

There are further tools for specific use cases. Here are some examples:

- The *Maven CFF Plugin* for Java projects built with Maven automatically creates a `CITATION.cff` draft from available metadata, including metadata for dependencies.
- *doi2cff* automatically creates a `CITATION.cff` file from a Zenodo DOI: <https://github.com/citation-file-format/doi2cff>.
- *ruby-cff* manipulates `CITATION.cff` files in Ruby: <https://github.com/citation-file-format/ruby-cff>.
- *cff-reader-java* is a Java library reading `CITATION.cff` files into a POJO model: <https://github.com/citation-file-format/cff-reader-java>.

# Events

Community events are a great way to learn about the Citation File Format, and contribute to making the citation of (research) software easier!

Past and upcoming events are listed on the [Events page](./events/).

# Have an idea? Found a problem?

We try to make contributing to CFF as easy as possible! Even tweeting a problem may be helpful, it's *that* easy.

Better still, if you can think of something that would make `CITATION.cff` files better, or you have found something that didn't work as you would have expected:
Please check out how you can share your idea or bug report in the [contribution guide on GitHub](https://github.com/citation-file-format/citation-file-format/blob/master/CONTRIBUTING.md).

