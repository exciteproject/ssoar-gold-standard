# SSOAR Gold Standard
This repository contains manually inspected datasets for evaluating the different steps during the reference extraction process. 
All datasets consist of research papers in German and come from the [SSOAR repository](http://www.ssoar.info/). 
We will constantly grow this corpus. 
For now, the PDF files of this corpus can be downloaded [here](http://excite-compute.west.uni-koblenz.de/ssoar-gold/).

## Content
* [reference-extraction](reference-extraction)
	* [ref-tags](reference-extraction/ref-tags)
        Currently contains 100 randomly picked German SSOAR publications with annotated reference strings (see [Paper Selection](#paper-selection)).
 	* [ref-strings](reference-extraction/ref-strings)
 		The reference strings (only in reference section) of papers are extracted from <ref></ref> tags and saved in text files. Each text file contains references of a paper and each reference string is saved in a separated line.
 
 * [reference-segmentation](reference-segmentation)
 	* [cermine/xml](reference-segmentation/cermine/xml)
 
 ## Paper Selection
We randomly select our papers from the 33,954 available publications that were available on [SSOAR repository](http://www.ssoar.info/).
 The random order of SSOAR publications that we used can be found at [random-ssoar-ids.csv](corpus/de/random-ssoar-ids.csv).
 For easier referencing we introduce a second ID, the EXCITEID, which refers to the position of a SSOAR ID in the above list.
 For example, ``109-12826.pdf`` refers to SSOAR ID 12826 which appears in line 109 in [corpus/de/random-ssoar-ids.csv](corpus/de/random-ssoar-ids.csv).
We excluded the following publications from our gold standard:
 
 * Non-German publications
 * Publications that were scanned
 * Publications that were scanned (images)
 * Publications that do not contain a reference section
 
 A list of excluded papers can be found at [corpus/de/sorted-out.csv](corpus/de/sorted-out.csv). All other papers that were excluded are scanned publications.