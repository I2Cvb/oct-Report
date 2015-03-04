MICCAI 2015 Breast segmentation Article based on my PhD thesis
==============================================================

What ? 
------
look at the damn title. This repo contains the latex for the article.


### Call for Papers

MICCAI attracts scientists, engineers, and clinicians from a wide range of disciplines associated with medical imaging and computer assisted interventions. Topics discussed at MICCAI include, but are not limited to:

* [x] Medical image computing
* [ ] Visualization and interaction
* [ ] Medical robotics
* [ ] Novel surgical devices and sensors
* [ ] Surgical and interventional systems
* [ ] Imaging and analysis methods for image guided therapies
* [ ] Physician-computer interfaces using virtual/mixed/augmented reality
* [ ] Computer-aided modeling and evaluation of surgical procedures
* [ ] Biological image computing
* [ ] Neuroscience image computing
* [ ] Computational anatomy
* [ ] Computational physiology
* [ ] Clinical and biological applications 

### Important dates
* [x] **2015-02-27 11:59 PM PST** Registration of paper with title, abstract and authors
* [ ] **2015-03-06 11:59 PM PST** Full paper submission deadline
* [ ] **2015-03-10 11:59 PM PST** Supplementary material deadline

### Submission Guidelines 
* [x] Papers should be formatted in Lecture Notes in Computer Science style.
* [ ] 8 pages maximum.
* [ ] The review process is double blind:
  * [x] Remove author and institutional information by replacing the information using * .
  * [x] Remove author information from all paper headers.
  * [ ] Remove clues from:
    * [x] Acknowledgment
    * [ ] collaborating partners (hospitals, companies)
    * [ ] Your own published work (including online publications) must be cited in the third person.
    * [ ] Your own work that is in press or accepted for publication and thus not available for the reviewers should be listed as "Anonymous" (with no other information) in the bibliography. For example: "In [5], Muller and Doe have proposed ..." is not acceptable if [5] is listed as "Anonymous".
    * [ ] You may reveal anonymized citations to the primary PC member (the one assigning the external reviewers) using the submission form. This information will not be known to external reviewers or secondary PC members (the ones making accept/reject recommendations for your paper). You may upload anonymized reprints of such papers as supplementary material.
    * [ ] Anonymize your PDF file. Note that PDF creator programs may accidentally leave Author information in the file header.

How ?
-----

### Structure
The primary file is called master.tex, and contains the bare essential and the abstract to get an idea of the content at a glance. The content is imported using include and input. Latex packages, acronyms, etc.. are called using input directly meanwhile the chapters (or sections) are called using include. If a chapter source requires from an external file, this is imported using input (in the further included chapter file).

The document structure is as follows

    .
    |____.gitattributes       % indicates git how to treat pdf and latex files
    |____.gitignore           % indicates git which files to ignore
    |____.git
    | |__ % Contains all the info regarding the repository
    |    
    |____master.pdf           % document output
    |____master.tex           % document source
    |____README.md            % this document you are reading.
    |
    |____content
    | |   % This folder contains any file related with the content of the 
    | |   % document. Each capter (or section) are stored in separated 
    | |   % folders, which contain a figures subdirectory. Other content
    | |   % refering to the whole document such as frontmatter, acronyms
    | |   % and bibliography can be found directly in this content folder.
    | |
    | |____acronym_definition.tex
    | |____frontmatter.tex
    | |____literature_review.bib
    | |
    | |____intro
    | | |____intro.tex
    | |____other
    | | |____figures
    | | | |____mcr3b.eps
    | | |____other_content.tex
    |
    |____latex
    | |   % This folder contains all the files regarding the behaviour of
    | |   % the document. Filesystem contains packages, styles, etc..
    | |   % If fonts or other resources are needed they must be found here
    | |
    | |____filesystem
    | | |____package.tex
    | | |____fileSetup.tex
    | |____fonts
    |

### Procedure
The master branch should be stay clean. Every conceptual increment (or todo item) should generate an issue. In order to address the issue a branch should be created and worked out. Once the issue is finished the master is checked out and the branch merged. If a issue needs to be reopen the issue is checked out, merged to master and reworked. Consider to open a new issue instead of reopening a previous one when possible.

### Important Note:
Keeping this file updated is important, it can help in further projects.

TODO
----
* [x] Branch properly
* [x] Reduce Abstract
* [ ] Reduce Introduction
* [ ] Kill comparison references (and refer to the PhD dissertation)
* [x] Add authors and replace information by *
* [ ] Evolve figures
* [ ] Tray a split strategy (1) Generic method, (2) for breast
* [ ] 
* [ ] 
* [ ] 
