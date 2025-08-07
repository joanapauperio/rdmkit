---
title: Biodiversity
search_exclude: true
description: Data management solutions for biodiversity data.
contributors: [Josephine Burgin, Joana Pauperio, Anne-Françoise Adam-Blondon, Patrick Ruch, Robert Waterhouse, Valeria Di Cola, Erwan Corre, Yvan Le Bras, Peter Woollard, Bachir Balech, Matteo Montagna, Angela P. Fuentes Pardo, Solenne Correard]
page_id: biodiversity
related_pages: 
  your_tasks: [dmp, data_organisation, metadata, data_brokering, machine_actionability, compliance]
  tool_assembly: [galaxy, fairtracks]
# More information on which page id you can use can be found at https://rdmkit.elixir-europe.org/website_overview
training:
  - name: Training about Biodiversity data
    registry: TeSS
    url: https://tess.elixir-europe.org/search?q=biodiversity+data

  - name: TeSS Collection of biodiversity-relevant training resources
    registry: TeSS
    url: https://tess.elixir-europe.org/collections/elixir-biodiversity-community

  - name: Galaxy Training Network
    registry: other
    url: https://training.galaxyproject.org/

  - name: ERGA Knowledge Hub
    registry: other
    url: https://knowledge.erga-biodiversity.eu/

  - name: Glittr
    registry: other
    url: https://glittr.org/

# More information on how to fill in this metadata section can be found here https://rdmkit.elixir-europe.org/page_metadata
---

<!-- Please take in mind our style guide https://rdmkit.elixir-europe.org/style_guide when writing the content of this page. -->

<!--- Domain pages should detail the particular data management challenges of the domain, typically by complementing and extending one or more existing Problem pages.
In the event that no adequate Problem page exists for a problem that can be generalized across domains, consider first contributing to create one or raising a GitHub issue. However, if a problem is entirely domain specific, then it should be fully detailed within the respective Domain page. --->

## Introduction

<!--- In this section you should provide a brief overview of the domain from the data management perspective, mentioning and putting into context the challenges that are particular to the domain, which will be the object of sections below. --->
While there is significant literature around biodiversity loss, there is a limited effort in reviewing biodiversity using high-throughput data acquisition technologies. Today, scientists recognise the important roles that genetic and genomic data (e.g. reference genomes, DNA/RNA barcoding approaches, metagenomics and metabarcoding), can play in biodiversity discovery, assessment, monitoring, conservation, and restoration, and its impact in policy and decision making processes. 

These research activities present unique data management challenges, especially in terms of complexity, data integration, and the need for interoperability across diverse datasets. Some of challenges include:

* Managing biological resources (samples, associated specimens or genetic resources): this requires compliance with the national and international frameworks and adherence to data sharing principles ([FAIR](https://www.nature.com/articles/sdata201618) principles, [Wilkinson 2016](https://doi.org/10.1038/sdata.2016.18)) and ethical principles (CARE Principles, [Carroll 2020](https://doi.org/10.5334/dsj-2020-043)).   
* Metadata in biodiversity research: metadata must go beyond basic descriptions to include detailed context, such as geographical locations, temporal data, methods, and environmental conditions, ideally using standard vocabularies (terminology) and ontology terms. Together, these aid ensuring that the data can be more easily discovered and effectively reused by both humans and machines.  
* Data management and integration systems: current systems still fail often to maintain critical links between the data, the metadata, the physical specimens, and the taxonomic information (e.g., correct scientific names) from which the data originates. Moreover, integrating molecular data (e.g., genomic sequences) with ecological, behavioral, or morphological datasets can be complex due to differences in formats, scales, and metadata structures.  
* Taxonomic harmonisation: taxonomy is an evolving field and linking data to and through taxonomy is challenging due to the spread of available resources and often unharmonised practices.   
* Handling and processing large-scale biodiversity data: molecular data (e.g., genomics or transcriptomics data) handling requires bioinformatics pipelines that are computationally intensive and can scale with large datasets.  
* Tracking provenance: ensuring proper tracking of the provenance, updates, and transformations of datasets is crucial, especially in collaborative biodiversity projects involving multiple stakeholders.

Addressing these challenges requires collaborative solutions involving better metadata practices, advanced bioinformatics tools, improved data integration platforms, and standardization efforts across the global biodiversity research community.

In addition to the specific data management challenges faced in biodiversity research, there is the need to move towards [Open Link Data](https://www.ontotext.com/knowledgehub/fundamentals/linked-data-linked-open-data/) in Biodiversity and a linked **Biodiversity Knowledge Graph** (see [machine actionability](https://rdmkit.elixir-europe.org/machine_actionability) for further information on knowledge graph)**.**   
This shift could fundamentally transform the landscape of biodiversity research by enabling more efficient data integration, discovery, and re-use. Moving towards a **Biodiversity Knowledge Graph** represents an ambitious but essential step in modernizing biodiversity research. While significant challenges remain, the potential for improved data integration, accessibility, and re-use across multiple disciplines could transform the field and open up new avenues for understanding and conserving biodiversity.

## Biological resource management and compliance
 
### Description
<!--- Sections within Domain pages (aside from "Introduction" at the start and "Tools and resources on this page" at the end) should focus on particular data management problems, which should be described in this first sub-section.
For problems that are fully domain-specific, a detailed description is merited.
For detailing the domain-specific challenges of a problem that is generic, please link to the corresponding generic Problem page before going into the domain-specific challenges. --->

Before starting your data collection, you need to plan how you will manage the biological resources (samples, associated specimens or genetic resources) and the data related to your experiment. However, managing biological resources \- such as samples, associated specimens, and genetic materials \- requires strict compliance with national and international frameworks like the Nagoya Protocol and adherence to ethical principles such as the CARE (Collective Benefit, Authority to Control, Responsibility, and Ethics) Principles ([Carroll 2020](https://doi.org/10.5334/dsj-2020-043)). While these frameworks are essential for promoting equitable benefit-sharing and responsible stewardship, they introduce significant data management challenges. Tracking the origin, consent, ownership, and permitted use of biological materials demands accurate and well-maintained metadata, persistent identifiers, and clear documentation of legal and ethical constraints. These requirements often vary across jurisdictions and can evolve over time, making it difficult to standardize processes across institutions and platforms. 

Here, we highlight key considerations to keep in mind when managing biological resource data, and we suggest relevant documents, standards, and frameworks to guide compliance and responsible data stewardship.

### Considerations
<!---  Direct and concise considerations, structured in bullet points and typically framed as questions RDMkit reader should ask themselves in order to arrive at the best solution among those listed below. One level of nesting of bullet points within considerations is fine, but more levels should be avoided. --->

* Do you have the required national and international permits for sample collection?  
* Will your sampling include Indigenous locations and/or be associated with traditional knowledge?  
* What biological material should be biobanked and where (samples, specimens, genetic resources)?  
* How will the data be preserved and shared?

### Solutions
<!--- Detail, either in normal text or in bullet points, the domain-specific solutions to the problem. Do not merely list tools or resources, as they will be automatically listed in the bottom section, but you can and should mention tools and resources listed below if you detail their usage to solve the problem. --->

* Ensure that due diligence was made regarding Nagoya treaty compliance, possibly with the help of your national focal point or institutional help desk. [The Global Genome Biodiversity Network (GGBN)](https://www.ggbn.org/ggbn_portal/) has developed a [ABS FactSheet and answer page](https://wiki.ggbn.org/ggbn/ABS_Fact_Sheet_and_Answers_to_Frequently_Asked_Questions) to help their network of biobanks to comply with the Nagoya protocol. More information is available on the [Compliance monitoring & measurement](https://rdmkit.elixir-europe.org/compliance_monitoring#how-can-you-ethically-access-genetic-resources-of-another-country) page. The main steps are summarised below:  
  * Check whether the countries where the samples are to be collected have signed the protocol, and identify the national entities that are issuing the permits for sample collection through the Access and Benefit Sharing Clearing House ([ABSCH](https://absch.cbd.int/en/?_gl=1*1taqnzf*_ga*NTEwOTEwMTYyLjE3Mjc2ODQwOTQ.*_ga_7S1TPRE7F5*MTcyNzY4NDA5My4xLjEuMTcyNzY4NDE5My42MC4wLjA.))  
  * If required, obtain the Prior Informed Consent (PIC) and Mutually Agreed Terms (MAT) and the final national permit of collection from the relevant(s) national focal point(s).  
  * Submit a Due Diligence declaration to the European Web-portal DECLARE (for European researchers) or to the ABSCH to get your Internationally Recognized Certificate of Compliance (IRCC).   
* Ensure that CARE principals are taken into account. If the samples are related to Indigenous Peoples and/or Local Communities, engage with the relevant communities during the planning phase of the experiment ([Mc Cartney *et al.,* 2023](https://www.nature.com/articles/s44185-023-00013-7)). Mc Cartney *et al* offer a framework, grounded in environmental justice and the CARE principles, for biodiversity genomic researchers, projects, and initiatives to support and promote the building of trustworthy and sustainable partnerships with Indigenous Peoples & Local Communities. Among other topics, engagement should consider:  
  * How the community will possibly access the specimens/samples collected and data generated.  
  * How the data will be labelled, accessed, and reused, including by the Indigenous communities for their own purposes, using, for example, [Local Contexts Labels and Notices](https://localcontexts.org/fr/).  
* Ensure that your Data Management Plan includes a section on specimen or biomaterial management or develop a specific Specimen management plan (see [Bentley et al. 2024](https://academic.oup.com/bioscience/article/74/7/435/7687409) for a proposal of guidelines). According to these guidelines this should include:  
  * The definition of the collections repository/biobank where the biomaterial will be stored.  
  * The type and anticipated number of specimens and/or samples, metadata collection and associated data.  
  * Plans for collection and preservation of the biomaterial that should be in line with established best practices for the relevant organisms (including the expectations of specimen curation and care).  
  * Plans for making the specimens/biomaterial available to the research community and for metadata publication and linkage to the data (also see recommendations for the digital extended specimen, [Hardisty et al. 2022](https://doi.org/10.1093/biosci/biac060)).  
* You can find more information on Biobanking and data management in [Alkhatib and Gaede, 2024](https://doi.org/10.3390/biotech13030034).

<!--- ## Section 2 Title --->
<!--- Add more sections as needed, with the same subsections as above. --->

## Biological material: metadata collection and publication
 
### Description
<!--- Sections within Domain pages (aside from "Introduction" at the start and "Tools and resources on this page" at the end) should focus on particular data management problems, which should be described in this first sub-section.
For problems that are fully domain-specific, a detailed description is merited.
For detailing the domain-specific challenges of a problem that is generic, please link to the corresponding generic Problem page before going into the domain-specific challenges. --->

Collecting and organizing rich metadata for biological materials, such as those stored in biobanks or specimen collections, is essential for enabling data interpretation, reuse, and integration across biodiversity studies. These materials are often linked to other types of data, including genomic sequences, images, phenotypic traits, and environmental context, making consistent metadata especially critical. However, a major challenge lies in identifying and applying suitable metadata standards, as multiple frameworks exist with varying levels of compatibility, coverage, and specificity. This complexity can hinder the accurate and interoperable description of samples, their origin, and associated information. In addition, managing persistent identifiers and maintaining consistent metadata across biological materials and their associated data is crucial for ensuring long-term traceability and interoperability. 

Here, we suggest commonly used metadata standards, as well as repositories and registries for (meta)data publication, to support effective and FAIR-compliant biobanking and biodiversity data management.

### Considerations
<!---  Direct and concise considerations, structured in bullet points and typically framed as questions RDMkit reader should ask themselves in order to arrive at the best solution among those listed below. One level of nesting of bullet points within considerations is fine, but more levels should be avoided. --->

Certain core metadata—such as collection date, biome, and geographical location—should always be collected to ensure basic contextualization and future usability. Beyond these essentials, the specific research context and use case will determine which additional metadata are most valuable. Key considerations include:

* Type of biological material: What kind of sample is being collected and analyzed (e.g., tissue, DNA, environmental sample)?  
* Type and intended use of data: What kind of data will be generated (e.g., genomic, phenotypic, environmental), and how is it expected to be used or reused?  
* Storage context: Will the biological material be preserved in a biobank, museum, or other long-term repository?  
* Data submission destination: Which database, repository, or registry will host the resulting data and metadata?

Collecting extensive (or "long-tail") metadata can greatly enhance data reuse and interoperability, but it also requires time and expertise. Therefore, metadata collection should be prioritized based on its anticipated value to future research and balanced against available human and technical resources.

### Solutions
<!--- Detail, either in normal text or in bullet points, the domain-specific solutions to the problem. Do not merely list tools or resources, as they will be automatically listed in the bottom section, but you can and should mention tools and resources listed below if you detail their usage to solve the problem. --->

* Consult your institution or project Data Management Plan to obtain information around the standard metadata that should be collected (also see [Documentation and metadata](https://rdmkit.elixir-europe.org/metadata_management#how-do-you-find-appropriate-standard-metadata-for-datasets-or-samples)), the procedures that should be used and the best practices for storing and sharing your data and metadata. Alternatively you can develop a Data Management Plan specific for your study following the guidelines available [here](https://rdmkit.elixir-europe.org/data_management_plan).  
* The metadata collected should be made available following community widespread standards to promote interoperability. The most relevant standards include the [Genomics Standards Consortium Minimal Information About (X) Any Sequence](https://www.gensc.org/pages/standards/checklists.html) (GSC MIxS, [Field et al. 2011](https://doi.org/10.1371/journal.pbio.1001088)) for genomics data, [Ecological Metadata Language](https://eml.ecoinformatics.org/) (EML, [Michener et al. 1997](https://doi.org/10.1890/1051-0761\(1997\)007[0330:NMFTES]2.0.CO;2)) for general biodiversity data, and [Darwin Core](http://www.tdwg.org/standards/450) (DwC, [Wieczorek et al. 2012](https://doi.org/10.1371/journal.pone.0029715)) mainly for taxa and their occurrences. For DNA/RNA barcoding data, BOLD (Barcode of Life Database, [Ratnasingham & Hebert 2007](https://doi.org/10.1111/j.1471-8286.2007.01678.x)) is developing the Barcoding Data Model ([BCDM](https://github.com/DNAdiversity/BCDM)). The core DwC terms have been aligned with the GSC MIxS ([Meyer et al 2023](https://doi.org/10.3897/BDJ.11.e112420)) terms, with further work underway to align many DwC extension terms to increase the interoperability.

**Sample metadata and checklists**

* Assess the type of sample/organism being analysed and the type of data being produced to identify the relevant metadata to collect. Take into consideration that richer metadata collection enables greater reuse of biodiversity information.  
* Identify the appropriate sample metadata checklist for submission to a public repository. There are several checklists available for different types of samples and analyses:  
  * The [European Nucleotide Archive](https://www.ebi.ac.uk/ena/browser/home) (ENA) has several [sample metadata checklists](https://www.ebi.ac.uk/ena/browser/checklists) for various sequence data types, part of these associated with biodiversity related data, that are adequate for different types of samples and research purposes.   
  * For reference barcodes, BOLD is using the Barcoding Data Model ([BCDM](https://github.com/DNAdiversity/BCDM)).  
  * For reference genomes there are specific guidelines regarding sample metadata collection. For example, the [ERGA](https://www.erga-biodiversity.eu/) (European Reference Genomes Atlas) initiative developed the [ERGA sample manifest](https://github.com/ERGA-consortium/ERGA-sample-manifest) that aligns with current standards and the [Tree of Life Checklist](https://www.ebi.ac.uk/ena/browser/view/ERC000053) at ENA.  
* When referencing in the sample metadata to information held in other repositories, as for example taxonomic information (also see Biological material: Taxonomic information), specimen collections or sampling protocols, always use persistent identifiers.  
* Also see this page on [documentation and metadata](https://rdmkit.elixir-europe.org/metadata_management).

**Biobanking and specimen linking**

* If possible keep vouchers and your tissues and DNA samples in a biobank/collection with relevant metadata (see Biological resource management and compliance)  
* The [Global Genome Biodiversity Network](https://www.ggbn.org/ggbn_portal/) (GGBN) is a global network of curated collections of genomic samples, working together to make DNA and tissue collections discoverable for biodiversity research. GGBN is actively developing resources and recommendations for data management in relation to biobanking and specimen collections with their networks of repositories \- GGBN data standard: [https://wiki.ggbn.org/ggbn/GGBN\_Data\_Standard](https://wiki.ggbn.org/ggbn/GGBN_Data_Standard).   
* [CETAF](https://cetaf.org/) (Consortium of European Taxonomic Facilities), an European Network of biological and geological collections, generates specimen identifiers for specimens in CETAF collections.  
* The European research infrastructure [DISSCO](https://www.dissco.eu/) (Distributed System of Scientific Collections) is working on developing a Digital Specimen Repository where DOIs will be provided for digital specimens.  
* In the sample metadata in Biosamples, reference the specimen or tissue/DNA samples using persistent identifiers available or using the DwC standard (‘triplet’ that includes the institution and collection codes, and specimen catalogue number), see also recommendations in [Agosti et al. 2002](https://doi.org/10.3897/rio.8.e97374).  
* In relation with collections of genetic resources that also encompass the intraspecific diversity, part of the recommendations are developed in the frame of FAO’s activities and completed through consortia of researchers supported by initiatives such as the Research Data Alliance.  
* You can also find relevant information by consulting other domain pages related to Biodiversity:  
  * link to Plant genetic resources: [https://rdmkit.elixir-europe.org/plant\_sciences](https://rdmkit.elixir-europe.org/plant_sciences)  
  * Link to Domestic animals: [https://data.faang.org/home](https://data.faang.org/home)   
  * Link to Microbial genetic resources: [https://www.mirri.org/microbial-resources-data/](https://www.mirri.org/microbial-resources-data/) 

**Sample metadata sharing and publication**

* Identify the repository where the sample metadata will be stored:  
  * For samples associated with genomic data, [Biosamples](https://www.ebi.ac.uk/biosamples/) database is recommended, as a persistent identifier will be assigned that will be linked with the data.   
* You can also reach out to data brokers or use brokering tools, that can help manage metadata and data submission to public repositories, as for example:   
  * [COPO](https://copo-project.org/) (Collaborative OPen Omics) is a data broker that is involved in metadata and data submission for the ERGA initiative  
  * [MADBOT](https://gitlab.com/ifb-elixirfr/madbot) (Metadata And Data Brokering Online Tool) is a web application that provides a dashboard for managing research data and metadata.  
  * [Galaxy Ecology](https://ecology.usegalaxy.eu/), a Biodiversity oriented Galaxy instance, proposing data brokers functionalities in a common platform. Some examples of the tools available:  
    * “ENA Upload tool” to publish in European Nucleotide Archive (ENA),   
    * Ecological Metadata Language (EML) oriented tools allowing to create EML metadata,  
    * data packages that can be used to share data through international repositories as DataONE, accepting raw datafiles related to earth observation or GBIF, OBIS, Emodnet accepting Darwin core Archives related mainly to taxon occurrences.  
* Modern technology such as mobile phone apps can streamline registration and collection of standardised metadata and field measurements. Automation such as this can reduce the burden on the sample collectors and increase the metadata quality. A great example is the NMDC Field Notes mobile app functionality [https://microbiomedata.org/field-notes/](https://microbiomedata.org/field-notes/)

## Biological material: Taxonomic information
 
### Description
<!--- Sections within Domain pages (aside from "Introduction" at the start and "Tools and resources on this page" at the end) should focus on particular data management problems, which should be described in this first sub-section.
For problems that are fully domain-specific, a detailed description is merited.
For detailing the domain-specific challenges of a problem that is generic, please link to the corresponding generic Problem page before going into the domain-specific challenges. --->

Taxonomy is an evolving field and harmonisation is challenging. Multiple classifications exist for the same group of organisms and these are reported in many taxonomy databases with varying taxonomic and geographic coverage, and quality. For example, [WoRMS](https://www.marinespecies.org/), the World Registry of Marine Species, holds an extensive record for marine species and [AlgaeBase](https://www.algaebase.org/) is a global database of algae including taxonomy, nomenclature and distributional information.   
The data repositories may be associated with or link to different taxonomic databases, so it is not always straightforward to understand what classification should be used in which situation. In addition, the advances in reference library production and in environmental DNA analysis lead to the discovery and identification of new taxa; submitting data for undescribed taxa or from environmental samples may also be challenging.   
This complex taxonomic foundation makes the reporting and linking of data to taxonomy challenging. The different public databases are used by researchers, but the taxonomic references in publications do not usually include persistent identifiers for taxon names or information regarding the taxonomy database used. Moreover, in some national biodiversity studies it is sometimes necessary to use other taxonomic reference systems that are more widely used by public monitoring agencies and that may not have persistent identifiers.

Here we present some considerations regarding ongoing initiatives to facilitate taxonomy mapping, clustering and linking, and provide some guidance for the submission and reporting of taxonomic information.  

### Considerations
<!---  Direct and concise considerations, structured in bullet points and typically framed as questions RDMkit reader should ask themselves in order to arrive at the best solution among those listed below. One level of nesting of bullet points within considerations is fine, but more levels should be avoided. --->

There are multiple taxonomic checklists covering different geographic and taxonomic ranges that are included in multiple databases. These checklists follow rules in taxonomic naming that are guided by nomenclature codes according to the type of organism. Most taxon names are published in scientific literature, with a description (taxonomic treatment).  
In addition to published taxonomy, some taxonomic databases also include placeholders for undescribed species and/or clustering mechanisms that identify novel taxonomic units. A classification for environmental samples is also available in [NCBI Taxonomy](https://www.ncbi.nlm.nih.gov/taxonomy).   
Most of the main taxonomic databases and checklists services provide persistent identifiers in different forms for taxon names that should be used when referring to a species in a publication (see [Agosti et al. 2022](https://doi.org/10.3897/rio.8.e97374)).   
Therefore, key considerations include: 

* Does the work involve organisms or environmental samples?  
* Is the organism being analysed already published in a taxonomic journal?   
* Are there taxonomic treatments (descriptions of the taxa in publications) available for the species?  
* Which taxonomy checklist/backbone is being used?  
* Is there a persistent identifier available for the taxon name?

### Solutions
<!--- Detail, either in normal text or in bullet points, the domain-specific solutions to the problem. Do not merely list tools or resources, as they will be automatically listed in the bottom section, but you can and should mention tools and resources listed below if you detail their usage to solve the problem. --->

* If you have questions regarding taxonomic nomenclature you can consult the nomenclature codes, such as the [International Code of Zoological Nomenclature](https://www.iczn.org/) (ICZN) and the [International Code of Nomenclature for algae, fungi, and plants](https://www.iapt-taxon.org/nomen/main.php).   
* You can also find information on Taxonomic treatments, i.e. detailed descriptions of a specific group of organisms (a taxon) within a scientific publication, and taxonomic citations on [TreatmentBank](https://plazi.org/treatmentbank/), which also provides persistent identifiers for the taxonomic names annotated in nomenclature sections of publications.  
* Choose the reference taxonomic backbone and reference it in the publication including a version if available.   
  * For sequence data, the most used taxonomic databases are [NCBI taxonomy](https://www.ncbi.nlm.nih.gov/taxonomy) used by the [International Nucleotide Sequence Database Collaboration](https://www.insdc.org/) (INSDC) and [BOLD taxonomy](https://boldsystems.org/data/taxonomy-page/) used by the [International Barcode of Life](https://ibol.org/) (iBOL).  
* NCBI taxonomy, in addition to the published taxon names, also allows for placeholder names for undescribed or novel species. These can then be updated once the taxon is published.   
* If you are using an unpublished name, use available processes for requesting the databases to mint an identifier to a placeholder name (for sequence data and NCBI taxonomy see [Blaxter et al. 2024](https://doi.org/10.12688/wellcomeopenres.22949.1)).  
* If working with environmental samples, you can use NCBI taxonomy (environmental biome level taxonomy).  
* There are also sequence clustering frameworks, used in some databases and management systems that identify novel taxonomic units (Operational Taxonomic Units \- OTU) and assign them with identifiers:  
  *  BOLD processes barcode sequences through an online framework that clusters the sequences into units and generates Barcode Identification Numbers (BINs, [Ratnasingham and Hebert 2013](https://doi.org/10.1371/journal.pone.0066213)).   
  * [UNITE](https://unite.ut.ee/index.php), a database that targets the nuclear ribosomal internal transcribed spacer (ITS) region and is used for molecular identification primarily of fungi, holds a pipeline that clusters ITS sequences into units, the UNITE Species Hypotheses (SHs) to which a unique DOI is assigned ([Abarenkov et al. 2024](https://doi.org/10.1093/nar/gkad1039)).  
  * The [Catalogue of Life](https://www.catalogueoflife.org/) (COL) is a global collaboration between taxonomists and bioinformaticians aiming at gathering up-to-date listings of all the world’s known species. COL in collaboration with the [Global Biodiversity Information Facility](https://www.gbif.org/) (GBIF) provides a global list of accepted names by integrating existing checklists, both from large scale and national initiatives. The GBIF taxonomic backbone derives from COL and merges additional names from authoritative nomenclatural and taxonomic datasets including identifiers such as BINs from BOLD and SHs from UNITE.   
* Use mapping tools available to facilitate the discovery of taxon names and persistent identifiers, such as:   
  * [Taxize](https://cran.r-project.org/web/packages/taxize/index.html) and [TaxonomyCleanR](https://github.com/EDIorg/taxonomyCleanr) R packages  
  * [ChecklistBank](https://www.checklistbank.org/), a repository of taxonomic datasets, developed in collaboration between GBIF and COL, allows mapping of taxonomic names and identifiers between the different taxonomies/checklists in COL.  
* Use persistent identifiers for the taxon name in the data publication if available (e.g. COL, NCBI taxonomy, BOLD, UNITE).

## Reference libraries: meta(data) collection and publication
 
### Description
<!--- Sections within Domain pages (aside from "Introduction" at the start and "Tools and resources on this page" at the end) should focus on particular data management problems, which should be described in this first sub-section.
For problems that are fully domain-specific, a detailed description is merited.
For detailing the domain-specific challenges of a problem that is generic, please link to the corresponding generic Problem page before going into the domain-specific challenges. --->

Reference genomes (DNA sequences of an organism's genome) are crucial for scientists to study genetic diversity and evolutionary relationships within, and between populations and species. These also enable analysis of population and functional genomics that facilitate monitoring of ecosystems. [DNA barcoding](https://ibol.org/about/dna-barcoding/) instead consists of the analysis of short, standardised DNA sequences to identify organisms at the species level. This fast and cost-effective approach has helped revolutionise species detection in biodiversity using metabarcoding and eDNA methods. However, the accuracy of metabarcoding methods relies on well-curated DNA barcoding reference libraries, as they provide the essential benchmarks needed for correctly identifying and assigning DNA sequences to the right taxa.

The scaling up of both barcoding and reference genome production for documenting biodiversity raises some data management challenges. These include the application of sequencing, barcoding, and genome analysis standards, the availability and documentation of analysis tools and computing platforms, and the sharing of reference sequence libraries. Collecting rich metadata for reference libraries is essential for ensuring the utility, traceability, and interoperability of genomic data. Proper metadata facilitates comparisons, reproducibility, and downstream analyses.

Here, we highlight key considerations to keep in mind when annotating and sharing reference libraries, and we suggest relevant standards and tools.

### Considerations
<!---  Direct and concise considerations, structured in bullet points and typically framed as questions RDMkit reader should ask themselves in order to arrive at the best solution among those listed below. One level of nesting of bullet points within considerations is fine, but more levels should be avoided. --->

* Is the relevant metadata about the specimens being collected and following the recommendations in the ‘[Biological material: metadata collection and publication](#biological-material:-metadata-collection-and-publication)’?  
* Consider collecting additional data, as for example, specimen images, that can be linked to the specimen.  
* Are the current standards for barcoding or reference genome production and publication being followed?  
* Are public bioinformatic pipelines being used or the bioinformatic pipelines and workflows being recorded in public repositories?  
* Consider making the data produced publicly available in an appropriate repository.

### Solutions
<!--- Detail, either in normal text or in bullet points, the domain-specific solutions to the problem. Do not merely list tools or resources, as they will be automatically listed in the bottom section, but you can and should mention tools and resources listed below if you detail their usage to solve the problem. --->

**Reference barcodes meta(data) collection and publication**

* Standards for barcoding are being developed by BOLD, the Barcoding Data Model ([BCDM](https://github.com/DNAdiversity/BCDM)) \- these include metadata for sample collection and processing as well as on sequence information and primers.   
* When additional data is collected, as for example, specimen image data, this should also be made available in a public repository. Some museum collections store and make available this information. BOLD stores image data linked with the specimen information. There are also specific databases, such as the [BioImage Archive](https://www.ebi.ac.uk/bioimage-archive/), where these are linked with the sample metadata in Biosamples. For more information on bioimaging see the [BioImaging domain](https://rdmkit.elixir-europe.org/bioimaging_data).   
* The details of the laboratory processes and bioinformatic pipelines (including taxonomic assignment pipelines) and workflows used to produce the reference barcodes, should be captured and made available by registering them into [GitHub](https://github.com/) or [WorkflowHub](https://workflowhub.eu/) ([Gustafsson et al. 2024](https://doi.org/10.48550/arXiv.2410.06941)) and linking to them from the data.  
* Publish the samples, raw data (if high throughput sequencing is used) and barcode sequences in the relevant public repositories:  
  * Samples can be submitted to BOLD and to Biosamples  
  * Raw data and curated barcodes can be submitted to the INSDC (e.g. in Europe to ENA)  
  * Curated barcodes can be submitted to BOLD  
* Use the appropriate reference libraries for your taxonomic area(s) of interest.

**Reference genomes meta(data) collection and publication**

* Standards for reference genomes production are published by the [Earth Biogenome Project](https://www.earthbiogenome.org/) \- these include reports on standards for sample collection and processing to genome analysis and annotations.   
* Reference genomes and raw sequence data should be submitted to the INSDC, through the ENA (its European node) or [NCBI](https://www.ncbi.nlm.nih.gov/) or the [DDBJ](https://www.ddbj.nig.ac.jp/index-e.html), where all the data will be linked to the biosample and bioproject information.  
* When additional data is collected, as for example, specimen image data, this should also be made available in a public repository. Some museum collections also store and make available this information. There are also specific databases, such as the [BioImage Archive](https://www.ebi.ac.uk/bioimage-archive/), where these are linked with the sample metadata in Biosamples. For more information on bioimaging see the [BioImaging domain](https://rdmkit.elixir-europe.org/bioimaging_data).   
* Analysis tools and pipelines should be published and linked to the data. There are some repositories available for capturing information on bioinformatic tools and databases (e.g. [GitHub](https://github.com/), [bio.tools](https://bio.tools/)) and on pipelines and workflows as [WorkflowHub](https://workflowhub.eu/).  
* The [European Reference Genome Atlas](https://www.erga-biodiversity.eu) (ERGA) initiative has a [Workflow Hub space](https://workflowhub.eu/programmes/33) where genome assembly, annotation and curation pipelines are available.  
* [Genome on a Tree (GoaT)](https://www.sanger.ac.uk/tool/genome-on-a-tree-goat/) is a powerful data aggregator and portal for reference genomes.  
* You can also use data brokering services or brokering tools that can help manage metadata and data submission to the public repositories (see section on biological material: metadata collection and publication).  
* The bioproject accession should be included in the publication.


