---
layout: post
icon: fas fa-atom
title: Open Source Science
order: 6
toc: true
date: 2024-05-22 16:00:00 +0600
---

<!-- markdownlint-capture -->
<!-- markdownlint-disable -->
> The Satellite Needs Working Group Management Office strongly encourages all SNWG Implementation team members take the time to enroll in and complete [NASA's Transform to Open Science (TOPS) OSS 101 course](https://nasa.github.io/Transform-to-Open-Science/).
{: .prompt-tip }

<!-- markdownlint-restore -->

## What is Open Source Science?
“Open Science is the principle and practice of making research products and processes available to all, while respecting diverse cultures, maintaining security and privacy, and fostering collaborations, reproducibility, and equity”.
[_The White House Office of Science and Technology Policy Memo, 2022 (adapted)_](https://open.science.gov/)

<!-- markdownlint-disable-next-line -->
<div align="center">

  As open as <strong>possible</strong>,<br>

  as restricted as <strong>necessary</strong>,<br>
  
  and <strong>always</strong> secure.

</div>

## Open Source Data Management Plan (OSDMP)

_In keeping with the [NASA Plan for Increasing Access to Results of Federally Funded Research](https://smd-cms.nasa.gov/wp-content/uploads/2023/05/NASA_Plan_for_increasing_access_to_results_of_federally_funded_research1.pdf) the [SMD Strategy for Data Management and Computing for Ground Breaking Science 2019-2024](https://smd-cms.nasa.gov/wp-content/uploads/2023/06/SDMWG_Full_Document_v3.pdf), and [SPD-41A](https://science.nasa.gov/researchers/science-data/science-information-policy/), SMD's Scientific Information Policy, which was updated late in 2022, most proposers to ROSES-2023 must provide an "Open Science and Data Management Plan", (formerly called the Data Management Plan) or an explanation of why one is not necessary given the nature of the work proposed. This Open Science and Data Management Plan (OSDMP) must address how publications, data, and software will be made available, see below and the [SMD Open-Source Science Guidance] at https://science.nasa.gov/oss-guidance for more detail and examples._

### Open Data in the OSDMP

- **What:** "A description of data types, volume, formats, and (where relevant) standards”;<br>
- **When**: “A description of the schedule for data archiving and sharing;”<br>
-  **Where**: “A description of the intended repositories for archived data, including mechanisms for public access and distribution;”<br>
- **How**: “A discussion of how the plan enables long-term preservation of data;”<br>
- **Who**: “A discussion of roles and responsibilities of team members in accomplishing the OSDMP. If funds are required for data management activities, these should be covered in the normal budget and budget justification sections of the proposal.

### Open Software in the OSDMP

- Acknowledge that “software needed to validate the scientific conclusions of a peer-reviewed publication resulting from an award, e.g., data underlying figures, maps, and tables in a publication must be made available at the time of publication.
    Include:
        - Expected software types
        - Repositories and timeline for sharing software
        - Description of software that are exempt from software sharing requirements<br>
- Acknowledge that the remaining scientifically useful software must be made available at the end of the award<br>
- Acknowledge that “publicly available software projects developed under the grant must include a code of conduct and guidelines for contributors and when released, have a digital persistent identifier, such as a Digital Object Identifier, associated with it to support citation.”<br>
- Acknowledge that “software should be released with an open, permissive license such as Apache 2.0, BSD 3-Clause “Revised” License, or MIT License. Any limitations to sharing the software should be described as part of the SMP.”<br>

### Open Publications in the OSDMP

- Acknowledge that the “as-accepted manuscript or the version of record of peer-reviewed publications must be made publicly available at the time of publication. <br>

Note: There are two options for compliance with this requirement: <br>
    (1) the manuscript is individually uploaded to NASA PubSpace by the time of publication or <br>
    (2) It is published in a journal that makes it openly available at the time of publication and also it is indexed by either CHORUS or ADS”

## Open Data

### Consider
- What is the nature of the data I am collecting or creating?
- How can the data be safely stored?
- Who can access the data without manipulating it (view-only)?  
- Who can access the data AND manipulate the data?
- Is my data understandable for others to use?
- Is my data in an accessible format that makes it easy for others to work with? 
- Is the data format widely used in my community?
- Does the data format I've chosen have adequate metadata support in my community?
- Are the tools needed to read the data format readily available in my community?
- Is my data easy to find?
- How private or open should my data be?
    - What does my supervisor or Principal Investigator say?
    - What does my grant/contract say?
    - What does my organization say?
    - What does my funding agency say?
    - If I am planning to publish, what does the publisher say?
<br>

### Data Attributes to document

| Data Description      | Full data use documentation |
| Data Quality          | Storage requirements        |
| Backup                | Access                      |
| Sharing               | Re-use                      |
| Preservation          | Archival                    |
| Responsibilities      | Resources                   |

### Data Deposit Locations

The following are examples of data repositories that can be used to host open data. Inclusion on this site does not indicate endorsement. 

- [4TU.Centre for Research Data](https://data.4tu.nl/): Data repository
- GitHub
- [Re3data](https://www.re3data.org/): Registry of Research Data Repositories 
- [CoreTrustSeal](https://www.coretrustseal.org/): offers to any interested data repository a core level certification based on the Core Trustworthy Data Repositories Requirements.  This universal catalog of requirements reflects the core characteristics of trustworthy data repositories.

### Data Preservation

Consider
- What type of data am I creating?
- What is the level of sensitivity of the data I am creating?
- Will future work or publications use this data as a base?
- Is the data unique?
- Is it easy to replicate the data?
- Are the costs of replication disproportionately high?
- Is there a formal obligation to preserve data for the longer term?
- Who is responsible for the management of data preservation?

<i class="fa fa-shuttle-space"></i> Tip: Data Management Costing Tool
A group at the Delft University of Technology has developed a [costing tool that allows a rough estimation of FTE resources](https://forms.gle/8mUXX3TWTr85eyK47).


## Open Software

_Research software includes various components like source code, algorithms, scripts, workflows, and executables created during or for research. It does not cover software like operating systems, libraries, dependencies, and packages that are used in research but weren't specifically developed for it. Research software should have persistent identifiers, be stored in repositories, be properly cited, and described with metadata. It is unique because it is executable, evolves with versioning, and depends on a specific development system._

|                         Open Source vs FAIR                       |
| :-------------------------------------------------------- | :--------------- |
| OS Software: released with a license <br> granting user rights | FAIR Software: provided via executable <br> without releasing source code |


|                         FAIR Data vs FAIR Software                      |
| :--------------------------------------------------- | :--------------- |
|Focus is on actions taken at the <br>**end of archiving** | Requires **ongoing action** from the start of the project,<br> such as in code documentation and modularization |

### FAIR Software

**F**indable: archive your software with a persistent identifier (DOI) and describe it with accurate metadata.
<br>

**A**ccessible: make your software available either directly or through a standardized protocol, allowing users to obtain and access the software and its documentation.

**I**nteroperable: your software should use community standards, formats, and protocols to ensure compatibility and interoperability with other tools and systems.

**R**eusable: your software should be well documented, modular, and designed in a way that promotes its reuse, allowing others to build upon or integrate it in their work.

## Open Publications

### Paths to Publication

**Golden Road:** A journal publishes the article open access with immediate access to the publication and free for anyone to read. Author pays “Article Processing Charge” (APC) for publishing.<br>
    _Diamond/Platinum Access:_ journal publishes the article open access with immediate access to the publication and free for anyone to read. Free to author publication costs covered by research department that runs the journal.<br>
    _Hybrid:_ Subscription-based journals offering a paid open access publishing option 
<br>

**Green Road:** Publishing in a subscription based journal, then self-archiving your publication and giving access to those without a subscription to the journal. 

### Contribution Licenses

CC - Creative Commons<br>
BY - BY original author<br>
SA - Same Attribute (ShareAlike)<br>
NC - No Commercial Use<br>
ND - No Derivative Works<br>
<br>

- **CC0** <br> Most permissive for copyright holders who want to assign their work to the public domain. Maximum Open Science (usually used for image and photo collections)<br>
<br>

- **CC-BY** <br>(Creative Commons Attribution) - others distribute,remix, tweak, and build upon your work,even commercially, as long as they credit you for the original creation.<br>
<br>

- **CC-BY-NC** <br> requires attribution, but only allows non-commercial use.<br>
<br>

- **CC-BY-ND** <br> requires attribution, blocks derivative works - no changing, adapting, or transforming a work.<br>
<br>

- **CC-BY-SA** <br>(ShareAlike) - requires attribution, and people can use and adapt the material for any purpose, even commercially.  must give appropriate credits and indicate if changes were made.The new material produced must be distributed under the same licenses as the original.<br>
<br>

- **CC-BY-SA-NC** <br>- you can use the original work in your own publication, as long as you:* Attribute the original author (BY); * Publish your work with the same license as the original author (SA); * Do not use the work for commercial purposes (NC).<br>
<br>

- **CC-BY-NC-ND** <br> Most restrictive; only distribution for non-commercial use of the unmodified original work is allowed.<br>

## Open Meetings
_more information needed here_
- Meeting Notice
- Meeting Notes
- Meeting Outcomes
- Document Hosting

## Algorithm Theoretical Basis Documents (ATBD)
_More information needed here. Pontus to advise._

