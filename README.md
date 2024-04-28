# Sistematic Literature Review (SLR) about debugging in the automation domain

This repository contains the results of a Sistematic Literature Review carried out in may 2023 about debugging in the automation domain which is the subject of a journal paper. An extract of the paper is presented below about the process carried out for the SLR. The results can be seen in the [results.csv](./results.csv) file.

## Research Questions

To know more about the automation domain and to analyze the current situation of debugging of PLC software, the following RQs were defined as the basis for the SLR:

- RQ1: What are the characteristics of automation systems that have an impact on the debugging of PLC software?
- RQ2: What are the existing debugging capabilities of PLC software?

## Search Strategy

The following terms were used when searching for studies that tackle the RQs. All these terms were in the resources in at least the title, abstract or author keywords.

```
(
 Programmable Logic Controller OR
 (
  PLC AND
  NOT Power Line Communications
 )
)
AND
(
 software OR
 program OR
 debug
)
```

the following list of digital libraries was used:

- [Scopus](https://www.scopus.com) 
- [ACM Digital Library](https://dl.acm.org) 
- [IEEE Explore](https://ieeexplore.ieee.org)

## Study Selection

From the information in the title, abstract and author keywords, inclusion and exclusion criteria were properly defined before conducting the SLR:

- Inclusion Criteria:
    - Studies that focus on any stage of the software development process ---not only debugging--- at the PLC level.
    - Studies mentioning any form of debugging done in the automation domain.
    - Studies subject to peer review such as journals and papers from conference proceedings.
    - Book chapters tackling the RQs.
- Exclusion Criteria: 
    - Studies that focus on the automation process but omit any evaluation of software in PLC.
    - Studies that focus on software development on higher levels above PLCs in the automation pyramid.
    - Studies whose main purpose is to present specific use-cases where PLCs are used.
    - Resources not written fully in English.

## Execution of the Search

A [custom-made software](https://github.com/cochicde/slr_tools) was developed to efficiently perform the search and the study selection.

During the search phase, the tool allows defining the search terms, getting the needed resources' information from the digital libraries and storing this information locally in a database. Next, during the study selection phase, the tool shows the users the resources stored in the database and they can easily include or exclude these to store this information back in the database.

The search was carried out on May 15th 2023 and returned the following amount of entries from the different digital libraries:

- Scopus: 6890
- ACM Digital Library: 137
- IEEE Explore: 1764

Since Scopus is an index of resources with links to other digital libraries, there were a significant number of overlaps, and after filtering duplicates, the total amount of resources found was 7202.
 
After reading the title, abstract and keywords of all the found entries, the inclusion and exclusion criteria were applied which left 156 resources. Among the main reasons to filter out the resources in this first phase, the following were found:

- PLC is only mentioned but is not the main focus: 70,7%.
- Wrong domain: 17,3%.
- Resource is not a paper or book chapter: 2,2%.

These 156 resources were read fully and only the amount of 50 presented information relevant to the RQs. The results can be seen in the [results.csv](./results.csv) file.

