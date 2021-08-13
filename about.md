---
title: Citation File Format (CFF) - About
---

{% include toc %}

The Citation File Format is a human- and machine-readable file format in [YAML 1.2](http://www.yaml.org/spec/1.2/spec.html) which provides
citation metadata for software (and datasets). 

Since its [inception in 2017](#2017-initiation), it has been developed as a community format within the 
international research software sustainability,
research software engineering, 
and scholarly communications communities.

The Citation File Format is maintained openly on GitHub: <i class="fa fa-github"></i> 
<https://github.com/citation-file-format/citation-file-format>.

# Rationale

> Citations have several important purposes: to **uphold intellectual honesty** (or avoiding plagiarism), to **attribute** prior or unoriginal work and ideas to the correct sources, to allow the reader to **determine independently** whether the referenced material supports the author's argument in the claimed way, and to help the reader **gauge the strength and validity** of the material the author has used. (Source: [Citation - Wikipedia](https://en.wikipedia.org/w/index.php?title=Citation&oldid=1038525167))

## Why software citation?

Research isn't conducted in a vacuum, it builds on prior work.
To **uphold their intellectual honesty**, researchers are required to cite the prior work their research builds on.
Modern research very often builds on software, which is used to collect, create, process, analyze and visualize research data, or to simulate complex scenarios for example.
Therefore, research software should be cited.

Research software constitutes an important and valid research output in itself.
The people that develop and maintain this software often work in academia, 
and may be evaluated, hired, and promoted partly based on citations to their work.
When researchers use software in their work 
and **attribute** this software to their creators through citation, 
they provide academic credit to the developers and maintainers
who may rely on it for their careers.
Also, attribution provides links between academic works, 
and helps us understand the history and provenance of an academic work,
of which software may be an important part.
Therefore, research software should be cited.

If someone wants to **determine independently** whether the argument or research results presented in an academic work are correct and should be treated as scientific knowledge,
they need access to all material underpinning the work, so that they can reproduce the results.
They also need access to the material if they want to **gauge its strength and validity**.
Access to the material that has been used in research is provided through citations, 
and in any computational research the material typically includes software.
Therefore, research software should be cited.

## Why the Citation File Format?

1. General rationale
  1. provide citation info
  2. CITATION files
2. Rationale for CFF 
  1. and its signle-mindedness & implementation details
  2. as opposed to otherformats


# Community governance

State now
Community input
Plans

## Steering committee

# History timeline

## Status

The spectrum of available concepts for software citation metadata files reaches
from non-standardized `CITATION` files as suggested by Robin
Wilson [1] to full transitive credit encoded in JSON-LD
[2].

Along this spectrum, Citation File Format is located somewhere between these two extremes as it adds
machine-readability and thus a greater re-use potential to `CITATION` files,
but does not offer transitive credit capabilities (yet), or support for all
citation use cases as outlined by Smith et al. [3].

Citation File Format aims at providing a practical solution, and human-friendly properties such
as readability and writability, for the most common software citation use
cases, i.e., *1. Use software for a paper*, *2. Use software in/with new software*,
and *15. Store software entry* (cf. Table 2, [3], p. 6).

The basic structure of Citation File Format (i.e., having a *message* and one or more
*references*) explicitly reflects the structure of plain-text `CITATION` files
and manifests its status as a compromise between what is currently *useful* and
*usable*, and what is *desired* (fully transitive credit and attribution). As such, it has value both as a discrete format with everyday application and as a input format populating other citation formats.

## Context

Software citations enhance the dissemination of code, improve software sustainability and ensure authors receive credit for development work. The Citation File Format is an indirect outcome of the discussion group "DS3. Development and
implementation of a standard format for CITATION files." at the [Workshop on
Sustainable Software for Science: Practice and Experiences
(WSSSPE5.1)](http://wssspe.researchcomputing.org.uk/wssspe5-1/) (6 September
2017, Manchester, UK). The group discussed the potential and outlined
requirements for a format for machine-readable CITATION files,
and has authored a [blog post](https://software.ac.uk/blog/2017-12-12-standard-format-citation-files) on the subject,
published on the [blog](http://software.ac.uk/blog/) of the [Software Sustainability
Institute](http://software.ac.uk/).

Members of the group were:

- Stephan Druskat (Humboldt-Universität zu Berlin, Germany), *Lead*
- Neil Chue Hong (Software Sustainability Institute, University of Edinburgh, UK)
- Raniere Silva (Software Sustainability Institute, University of Manchester, UK)
- Radovan Bast (University of Tromsø, Norway)
- Andrew Rowley (University of Manchester, UK)
- Alexander Konovalov (University of St. Andrews, UK)

One requirement for the [blog post](https://software.ac.uk/blog/2017-12-12-standard-format-citation-files) was to be able to make a concrete suggestion
for a format for these machine-readable CITATION files, which triggered the
development of Citation File Format.

[^no-file-no-use]: Not providing a file with software citation metadata is not considered a valid option here.

# Releases

## Pre-1.1.0

Older versions for CFF are listed in the following table.

|       Version        |                                    Specifications                                    | Schema |                                 DOI                                 | Release |
|----------------------|--------------------------------------------------------------------------------------|--------|---------------------------------------------------------------------|---------|
| 1.0.3 | Core module: [PDF](/assets/pdf/cff-specifications-1.0.3.pdf) | [1.0.3-1](https://github.com/citation-file-format/schema/releases/tag/1.0.3-1)      | [10.5281/zenodo.3515946](https://doi.org/10.5281/zenodo.3515946)    |         |
| 1.0.2 | Core module: [PDF](/assets/pdf/cff-specifications-1.0.2.pdf) | [1.0.2](https://github.com/citation-file-format/schema/releases/tag/1.0.2)      | [10.5281/zenodo.1120256](https://doi.org/10.5281/zenodo.1120256)    |         |
| 1.0.1 | Core module: [PDF](/assets/pdf/cff-specifications-1.0.1.pdf) | [1.0.1](https://github.com/citation-file-format/schema/releases/tag/1.0.1)      | [10.5281/zenodo.1117789](https://doi.org/10.5281/zenodo.1117789)    |         |
| 1.0.0 | Core module: [PDF](/assets/pdf/cff-specifications-1.0.0.pdf) | -      | [10.5281/zenodo.1108269](http://doi.org/10.5281/zenodo.1108269)    |         |
| 1.0-RC1 | [PDF](/assets/pdf/cff-specifications-1.0-RC1.pdf) | -      | -    |         |
| 0.9-RC1 | [PDF](/assets/pdf/cff-specifications-0.9-RC1.pdf) | -      | [10.5281/zenodo.1003150](https://doi.org/10.5281/zenodo.1003150) |         |

## Contributing

Contributions to CFF are welcome! Please have a look at the 
[guidelines for contributing](https://github.com/citation-file-format/citation-file-format/blob/master/CONTRIBUTING.md).

# References

[1] R. Wilson, “Encouraging citation of software–introducing CITATION files.” 2013 [Online]. Available: https://goo.gl/7gZuSY

[2] D. S. Katz and A. M. Smith, “Transitive Credit and JSON-LD,” Journal of Open Research Software, vol. 3, no. 1, p. e7, Nov. 2015. 

[3] A. M. Smith, D. S. Katz, K. E. Niemeyer, and FORCE11 Software Citation Working Group, “Software citation principles,” PeerJ Comput. Sci., vol. 2, no. e86, 2016 [Online]. Available: https://doi.org/10.7717/peerj-cs.86

# Timeline

<!-- Capture Markdown content for reuse in timeline HTML -->
<!-- Note: capture names cannot be just year ints -->
{% capture content2021 %}
## 2021
{: .timelineheader}
- CFF 1.2.0 released (doi:[10.5281/zenodo.5171937](https://doi.org/10.5281/zenodo.5171937))
- CFF 1.1.0 released (doi:[10.5281/zenodo.4813122](https://doi.org/10.5281/zenodo.4813122))
{% endcapture %}

{% capture content2020 %}
## 2020
{: .timelineheader}
Registries workshop
{% endcapture %}

{% capture content2019 %}
## 2019
{: .timelineheader}
RSE Hackathon?
      CW Hack thing
{% endcapture %}

{% capture content2018 %}
## 2018
{: .timelineheader}
CFF 1.0.3 released (doi:[10.5281/zenodo.1120389](https://doi.org/10.5281/zenodo.1120389))
{% endcapture %}

{% capture content2017 %}
## 2017: Initiation
{: .timelineheader}
- [WSSSPE5.1](http://wssspe.researchcomputing.org.uk/wssspe5-1/) workshop:
  - Lightning talk "Should `CITATION` files be standardized?" (doi:[10.6084/m9.figshare.3827058.v4](https://doi.org/10.6084/m9.figshare.3827058.v4))
  - Discussion group & blog post "A standard format for CITATION files" ([link](https://software.ac.uk/blog/2017-12-12-standard-format-citation-files))
- CFF 1.0.0 released (doi:[10.5281/zenodo.1108269](https://doi.org/10.5281/zenodo.1108269))
{% endcapture %}

<div class="timeline">
  <div class="timelinecontainer timelineright">
    <div class="timelinecontent">{{ content2021 | markdownify }}</div>
  </div>
  <div class="timelinecontainer timelineleft">
    <div class="timelinecontent">{{ content2020 | markdownify }}</div>
  </div>
  <div class="timelinecontainer timelineright">
    <div class="timelinecontent">{{ content2019 | markdownify }}</div>
  </div>
  <div class="timelinecontainer timelineleft">
    <div class="timelinecontent">{{ content2018 | markdownify }}</div>
  </div>
  <div class="timelinecontainer timelineright">
    <div class="timelinecontent">{{ content2017 | markdownify }}</div>
  </div>
</div>