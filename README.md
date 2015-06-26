MW-OMIA: MICCAI Workshop - Ophthalmic Medical Image Analysis; Paper
===================================================================

Classification of SD-OCT volumes with LBP: application to DME detection
------------------------------------------------------------------------

What ?
------
This repository contains the latex files to generate the paper entitled
`Classification of SD-OCT volumes with LBP: application to DME detection`
which was summited to the MW-OMIA in 2015.

The results reported in this article can be replicated based on this
[repo-tag](https://github.com/I2Cvb/retinopathy/tree/0.0.1).

### Call for Papers


MICCAI attracts scientists, engineers, and clinicians from a wide range of
disciplines associated with medical imaging and computer assisted
interventions.

Topics discussed at MW-OMIA include, but are not limited to:
* [x] Computer-aided detection and diagnosis of disease
* [ ] Image analysis of novel ophthalmic imaging modalities
* [ ] Multimodal ophthalmic image analysis
* [ ] Ophthalmic image atlases
* [ ] Ophthalmic image analysis in animals
* [ ] Registration of ophthalmic images, including multimodal
* [ ] Segmentation of structures (e.g., vasculature, lesions, landmarks)
* [ ] Combined analysis of images of the eye and other organs
* [ ] Validation and evaluation of software tools
* [ ] Crowd sourcing
* [ ] Retinal biomarkers studies for various conditions, eg, diabetes, cardiovascular, neurodegenerative

### Important dates

* [x] **2015-05-19** Full paper submission deadline
* [ ] **2015-06-17** Acceptance/rejection notification
* [ ] **2015-08-03** final version of acepted papers
* [ ] **2015-09-10** MW-OMIA workshop

### Submission Guidelines
* [x] Papers should be formatted in Lecture Notes in Computer Science style.
* [x] 8 pages maximum.
* [ ] The review process is double blind:
  * [x] Remove author and institutional information by replacing the information using * .
  * [x] Remove author information from all paper headers.
  * [ ] Remove clues from:
    * [x] Acknowledgment
    * [x] collaborating partners (hospitals, companies)
    * [x] Your own published work (including online publications) must be cited in the third person.
    * [x] Your own work that is in press or accepted for publication and thus not available for the reviewers should be listed as "Anonymous" (with no other information) in the bibliography. For example: "In [5], Muller and Doe have proposed ..." is not acceptable if [5] is listed as "Anonymous".
    * [x] You may reveal anonymized citations to the primary PC member (the one assigning the external reviewers) using the submission form. This information will not be known to external reviewers or secondary PC members (the ones making accept/reject recommendations for your paper). You may upload anonymized reprints of such papers as supplementary material.
    * [ ] Anonymize your PDF file. Note that PDF creator programs may accidentally leave Author information in the file header.

How ?
-----

### Structure
The primary file is called master.tex, and contains the bare essential and the abstract to get an idea of the content at a glance. The content is imported using include and input. Latex packages, acronyms, etc.. are called using input directly meanwhile the chapters (or sections) are called using include. If a chapter source requires from an external file, this is imported using input (in the further included chapter file).

The document structure is as follows

    .
    ├── .gitattributes      % indicates git how to treat pdf and latex files
    ├── .gitignore          % indicates git which files to ignore
    ├── .git/               % Contains all the info regarding the repository
    │
    ├── master.pdf          % document output
    ├── master.tex          % document source
    ├── README.md           % this document you are reading.
    |
    ├── content/
    │   │   % This folder contains any file related with the content of the
    │   │   % document. Each capter (or section) are stored in separated
    │   │   % folders, which contain a figures subdirectory. Other content
    │   │   % refering to the whole document such as frontmatter, acronyms
    │   │   % and bibliography can be found directly in this content folder.
    │   │
    │   ├── acronym_definition.tex
    │   ├── frontmatter.tex
    │   ├── literature_review.bib
    │   │
    │   ├── experiment/
    │   │   └── experiment.tex
    │   ├── intro/
    │   │   └── intro.tex
    │   ├── method/
    │   │   ├── figures/
    │   │   ├── BoFFramework.tex
    │   │   └── method.tex
    │   └── results
    │       └── results.tex
    │
    ├── latex
    │   │   % This folder contains all the files regarding the behaviour of
    │   │   % the document. Filesystem contains packages, styles, etc..
    │   │   % If fonts or other resources are needed they must be found here
    │   │
    │   └── filesystem/
    │       ├── package.tex
    │       └── fileSetup.tex
    │
    ├── aliascnt.sty              % MICCAI template file
    ├── llncs.cls                 % MICCAI template file
    ├── llncs.dem                 % MICCAI template file
    ├── llncsdoc.sty              % MICCAI template file
    ├── remreset.sty              % MICCAI template file
    ├── splncs03.bst              % MICCAI template file
    └── sprmindx.sty              % MICCAI template file

### Procedure
The master branch should be stay clean. Every conceptual increment (or todo item) should generate an issue. In order to address the issue a branch should be created and worked out. Once the issue is finished the master is checked out and the branch merged. If a issue needs to be reopen the issue is checked out, merged to master and reworked. Consider to open a new issue instead of reopening a previous one when possible.

### Important Note:
Keeping this file updated is important, it can help in further projects.

TODO
----
* [x] Branch properly
* [x] Add authors and replace information by *
* [ ]
* [ ]
