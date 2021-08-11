---
---

{% include toc %}

# What is a `CITATION.cff` file?

`CITATION.cff` files are plain text files with human- and machine-readable citation information for software (and datasets).
Code developers can include them in their repositories to let others know how to correctly cite their software.

This is an example of a simple `CITATION.cff` file:

{% highlight yaml %}
cff-version: 1.2.0
message: "If you use this software, please cite it as below."
authors:
  - family-names: Druskat
    given-names: Stephan
    orcid: https://orcid.org/0000-0003-4925-7248
title: "My Research Software"
version: 2.0.4
doi: 10.5281/zenodo.1234
date-released: 2021-08-11
{% endhighlight %}

The format of `CITATION.cff` files is the **Citation File Format (CFF)**.

# Why you should add a `CITATION.cff` file to your repository!

It is very easy to *correctly* cite a paper: all the necessary information (*metadata*) can be found on the title page or the article website.
Software and datasets have no title page, the relevant information is often less obvious.

People who want to cite your software may ask questions like:

<i class="fa fa-question-circle"></i> What is the name of the software (it’s probably not `my_scripts/run.m` or `analysis.py`)?
{: .notice--info}

<i class="fa fa-question-circle"></i> What label should I use to uniquely identify the version of the software I have used?
{: .notice--warning .text-right}

<i class="fa fa-question-circle"></i> What is the appropriate set of people that should be cited as authors?
{: .notice--success}

The person who wants to cite your software will probably not be able to answer these questions accurately and consistently themselves, but you can!
Give them all the right information in a `CITATION.cff` file, and they can cite your software *correctly*.

Also, if you publish your software in an archive or registry, they (or their systems) can re-use the citation metadata from your `CITATION.cff` file.

## Supported by GitHub <i class="fa fa-github"></i>

![image-left](/assets/images/github.png){: .align-left} When you put a `CITATION.cff` file in the default branch of your GitHub repository, it is automatically linked from the repository landing page,
and the citation information is rendered on the repository page, and also provided as BibTeX snippet which users can simply copy! 
This makes it easy for other users to cite your software project, using the information you've provided.  
[Read more ...](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/creating-a-repository-on-github/about-citation-files)

## Supported by Zenodo <i class="icon-zenodo"></i>

![image-left](/assets/images/zenodo.svg){: .align-left} When you have a `CITATION.cff` file in your GitHub repository, make a release and publish it on Zenodo via the Zenodo-GitHub integration, 
Zenodo will use the citation information you've provided to populate the publication entry! 
This makes it easier for software developers and maintainers to publish their software with complete and correct metadata.  
[Read the announcement ...](https://twitter.com/ZENODO_ORG/status/1420357001490706442)

## Supported by Zotero <i class="icon-zotero"></i>

![image-left](/assets/images/zotero.png){: .align-left} When you have a `CITATION.cff` file in your repository, and someone uses the Zotero browser plugin to import a reference to your repository 
into their Zotero reference manager, it will use the citation information you've provided to populate the reference entry! 
This makes it easier for users to get a complete and correct reference to your software,
that they can use when they cite your software in their work!  
[Read the announcement ...](https://twitter.com/zotero/status/1420515377390530560)

# Create a `CITATION.cff` file now!

You can start by copy-and-pasting the [example above](#what-is-a-citation-cff-file) into the root of your code repository, and adapt the information to your software.

You can also use a simple website to fill in the citation information for your software.
To do so, go to the [`cffinit` website](https://citation-file-format.github.io/cff-initializer-javascript/).

To learn more about how to work with the Citation File Format, have a look at the [documentation](https://github.com/citation-file-format/citation-file-format/blob/main/README.md).

The Citation File Format is much more powerful than the minimal example above suggests. 
It also allows you to record the *references* for your software, for example, 
to make visible the work that your own work builds on.
To find out what citation-relevant information you can provide in `CITATION.cff` files,
have a look at the [guide to the Citation File Format](https://github.com/citation-file-format/citation-file-format/blob/main/schema-guide.md).

# Tools for working with `CITATION.cff` files

Different tools exist to help you work with `CITATION.cff` files:

- The **initializer** can help you create a `CITATION.cff` file from scratch: <https://citation-file-format.github.io/cff-initializer-javascript/>.
<!--- The **validator** checks whether a `CITATION.cff` file is formatted correctly: [TODO link].-->
- The **converter** can convert a `CITATION.cff` to other formats (e.g., to *BibTeX*, *RIS*, *CodeMeta*, and others): <https://github.com/citation-file-format/cff-converter-python>.

There are further tools for specific use cases, and different environments.
The documentation has a brief [overview of available tools](https://github.com/citation-file-format/citation-file-format#tools-to-work-with-citationcff-files-wrench).

# Have an idea? Found a problem?

We try to make contributing to CFF as easy as possible! Even tweeting a problem may be helpful, it's *that* easy.

Better still, if you can think of something that would make `CITATION.cff` files better, or you have found something that didn't work as you would have expected:
Please check out how you can share your idea or bug report in the [contribution guide on GitHub](https://github.com/citation-file-format/citation-file-format/blob/master/CONTRIBUTING.md).

