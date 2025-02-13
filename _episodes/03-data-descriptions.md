---
title: "2. Speak the same language"
teaching: 10
exercises: 15
questions:
- "1 What are Data Descriptions?"
- "2 How to reuse Data Descriptions?"
- "3 Are there standard ways for doing Data Descriptions?"
- "4 What is the relation between Data Descriptions and Linked Data?"
objectives:
- "The participant will learn that Data Descriptions are named differently in various fields."
- "The participant will be able to create a machine-friendly Data Descriptions file."
keypoints:
- "'Codebook', 'data glossary', or 'data dictionary' are some other ways to name **Data Descriptions**."
- "**Ontologies** (in information science) are like public online vocabularies of community curated terms and their definitions."   
- "By reusing **Ontology terms** or community accepted vocabularies, we aim to create a culture of recycling terminology by default."
---

> ## FAIR principles used in Data Descriptions:  
> **Interoperable**   
> > FM-I1 (Use a Knowledge Representation Language) → [doi.org/10.25504/FAIRsharing.jLpL6i](https://doi.org/10.25504/FAIRsharing.jLpL6i)  
> > FM-I2 (Use FAIR Vocabularies) → [doi.org/10.25504/FAIRsharing.jLpL6i](https://doi.org/10.25504/FAIRsharing.0A9kNV)  
>
> **Reusable**  
> > FM-R1.3 (Meets Community Standards) → [doi.org/10.25504/FAIRsharing.cuyPH9](https://doi.org/10.25504/FAIRsharing.cuyPH9)  
>
{: .checklist}

### 1. What are Data Descriptions?

> Data descriptions are a detailed explanation and documentation of each data attribute or variable in a dataset.  
{: .objectives}

Depending on the use case and field of research, these data descriptions are also known as:  
- Codebooks (e.g., in Statistics or Social Sciences)
- Data Dictionaries (e.g., in Computer and Data Science)
- Labels or Data Tags (e.g., in Crowdsourcing or Humanities)
- Data Glossary (e.g., in Business Administration & Finance)
- Metadata (wrong use of this term in this context)

For example:  

|Variable Name | Description| Scale|
|---|---|---|
|Weight | Weight of a human | kilograms|
|Height | Height of a human | centimetres |
|Age | Age of a human | years|
|Blood Glucose Level |Blood glucose level of a human | mg/dl|

> ## "Data Descriptions" is sometimes named differently depending on the field
>
> No matter what terminology you use, "Data Descriptions" always refers to a detailed explanation and documentation of each data attribute or variable in a dataset.
{: .callout}

### 2. How to reuse Data Descriptions?

Documentation of any kind always takes time. However, we shall always aim to reuse existing data descriptions generally accepted in the community. i.e., the variable `Weight` is a concept that has been widely used in research; therefore, we don't need to redefine it every time.  

For example, in [BioPortal](https://bioportal.bioontology.org/), we can find existing descriptions of `Weight`. These descriptions belong to an [Ontology](https://en.wikipedia.org/wiki/Ontology_(information_science)), i.e., a community-accepted online dictionary for curated terms and definitions. Moreover, it provides a globally unique identifier to the description.  → [LINK TO EXAMPLE](https://bioportal.bioontology.org/)  

<br>
<img src="../fig/FAIRcoursebook-image2_1.png" alt="bioportal 1" style="max-width: 60%; height: auto;">
<br>
You will get several results when searching for a term and its definition. These results regard the different ontologies that define these terms. For example, think of the description of an apple. It might be defined differently in a British dictionary than in an American one.
<br>
<img src="../fig/FAIRcoursebook-image2_2.png" alt="bioportal 2" style="max-width: 60%; height: auto;">
<br>
Finally, using this Ontology, you can get a standard definition that community experts curate has a global identifier.  
<br>
<img src="../fig/FAIRcoursebook-image2_3.png" alt="bioportal 3" style="max-width: 60%; height: auto;">
<br>

> ## Describe your data by reusing Ontology terms  
>
> By reusing Ontology terms or community-accepted vocabularies, we aim to create a culture of recycling definitions by default.  
> > **Advantages**  
> > - We don't have to redefine the terms every time
> > - We get a permanent link to the resource
> > - Since it uses a global identifier becomes easier for others to integrate with different data sources  
> > **Disadvantages**  
> > - Sometimes, you might not find an Ontology or vocabulary that fits your variable.  
{: .callout}

### 3. Are there standard ways for doing Data Descriptions?

There are no standard ways of doing Data Descriptions.  
The minimum elements you need to describe your dataset are the **Variable Name** and the **Link to Description**. You can do that in a tabular format. However, following the FAIR principles of Interoperability and Reusability, we must ensure that the data is described using community standard FAIR vocabularies. Here are some Ontologies for general use that can cover a wide variety of data attributes

|Ontology | Link | About what?|
| ---| ---|
|Schema.org | [LINK](https://schema.org/)| Definitions of generic things e.g., "Computer"|
|DBpedia | [LINK](https://www.dbpedia.org/resources/lookup/)| Definitions from Wikipedia |
|Data Catalog Vocabulary (DCAT) | [LINK](https://www.w3.org/TR/vocab-dcat-2/)| Definitions about data things e.g., "accessURL"|
|Dublin Core | [LINK](https://www.dublincore.org/specifications/dublin-core/dcmi-terms/)| Definitions about Metadata|

> ## There are also public registries where you can find Ontologies
> **Linked Open Vocabularies**  → [lov.linkeddata.es/dataset/lov/](https://lov.linkeddata.es/dataset/lov/)  
> **EU Vocabularies:**  → [op.europa.eu/en/web/eu-vocabularies](https://op.europa.eu/en/web/eu-vocabularies)  
> **BioPortal:**  → [bioportal.bioontology.org/](https://bioportal.bioontology.org/)  
> **AgroPortal:**  → [agroportal.lirmm.fr/](http://agroportal.lirmm.fr/)  
> **EcoPortal** → [ecoportal.lifewatchitaly.eu/](http://ecoportal.lifewatchitaly.eu/)  
> **Ontology Lookup Service by the EBI** → [ebi.ac.uk/ols/index](https://www.ebi.ac.uk/ols/index)  
> **Bioschemas** → [bioschemas.org/](https://bioschemas.org/)  
{: .prereq}

----

> ## Exercise - Level Easy 🌶
>
> 1. Visit [BioPortal](https://bioportal.bioontology.org/). BioPortal is the most known repository for biomedical ontologies  
> 2. Search for an Ontology term for `blood glucose level` In the "Search for a class" search box.  
> 3. Select one result related to a clinical measurement that is sound to you.   
> 4. What are the definition and ID?  
> 
> {: .source}
>
> > ## Solution
> >
> > Definition: Measurement of the amount of glucose, the monosaccharide sugar, C6H12O6, occurring widely in plant and animal tissues which is one of the three dietary monosaccharides that are absorbed directly into the bloodstream during digestion, is the end product of carbohydrate metabolism, and is the chief source of energy for living organisms, in a specified volume of blood, the fluid that circulates through the heart, arteries, capillaries and veins carrying nutrients and oxygen to the body tissues and metabolites away from them.  
> > ID: [http://purl.obolibrary.org/obo/CMO_0000046](http://purl.obolibrary.org/obo/CMO_0000046)
> > {: .output}
> {: .solution}
{: .challenge}

The **Data Descriptions** (or data dictionaries in some domains) are usually manually written in a tabular format. This document has the length and depth that the data owner sees fit. The general rule of thumb is to describe the dataset related to a publication. Any accessible format like `.csv`, `.xls`, or similar is acceptable.  

<img src="https://dataedo.com/asset/img/kb/glossary/data_vs_data_dictionary.png" alt="tabular">

In case it is a database, a data model must be included in machine-readable format (e.g., `.sql`) and a human-friendly diagram (e.g., ER model on `.pdf`).

There are examples where data descriptions are made available in a human-relatable manner, such as the *dataset nutrition labels* style [(Holland et al., 2018)](https://arxiv.org/abs/1805.03677).   
An example is **A Statutory Article Retrieval Dataset**   → [LINK TO EXAMPLE](https://github.com/maastrichtlawtech/bsard/blob/master/docs/img/nutrition.png)   
Moreover, there are tools and software packages to generate automated "Codebooks" by only looking at the dataset  
An example is **Automatic Codebooks from Metadata Encoded in Dataset Attributes**   → [LINK TO EXAMPLE](https://rubenarslan.github.io/codebook/).  

These initiatives are helping us standardize data descriptions and are "Human Friendly", which works perfectly. However, the FAIR principles FM-I1, FM-I2 and FM-R1.3 explicitly mention the need for [Linked Data](https://en.wikipedia.org/wiki/Linked_data) formats in order to gain the maximum level of **Interoperability**.

### 4. What is the relation between Data Descriptions and Linked Data?

When we create comprehensive Data Descriptions reusing terminologies of existing Ontologies, we could make available our dataset in a [Linked Data](https://lod-cloud.net/#) format which makes it **Interoperable** with other datasets out there.

Imagine your dataset can be helpful to another researcher in the future. The future researcher can reuse your dataset and combine both by matching variable names with the Ontology identifiers. 

There are several tools that help you to convert your dataset from a conventional format into a Linked Data format (e.g., [RDF format](https://en.wikipedia.org/wiki/Resource_Description_Framework)).

|Tool | Source | GUI | Note|
| ---| ---|---|---|
|Open Refine | [LINK](https://openrefine.org/)| ✅| Installation can be a hassle and takes a lot of memory|
|RMLmapper | [LINK](https://github.com/RMLio/rmlmapper-java/releases)| ❌| Highly technical you need to know command line tools, preferred option of data engineers   |
|SDM-RDFizer | [LINK](https://github.com/SDM-TIB/SDM-RDFizer)| ❌ | You need to be familiar with programming languages |
|SPARQL-Generate | [LINK](https://ci.mines-stetienne.fr/sparql-generate/)| ✅|It is a good option if you are going to invest time in it since you can learn SPARQL language
|Virtuoso Universal Serve | [LINK](https://virtuoso.openlinksw.com/)| ✅|It's nice but you have to pay for a license|
|UM LDWizard | [LINK](https://humanities.wizard.semanticscience.org)| ✅|It's free, gets the job done quickly, and you can publish data if you have a [TriplyDB](https://triplydb.com/) account → **RECOMMENDED**|

> ## Exercise - Level Hard 🌶🌶🌶
>
> 1. Transform a dataset from XLSX format to RDF format using [UM LDWizard](https://humanities.wizard.semanticscience.org)  
>
> 2. Download the following mock dataset: [MOCK DATA](../fig/MOCK_DATA_BOOTCAMP.xlsx)  
> 
> 3. What ontology terms did you reuse to describe the data attributes?  
> {: .source}
>
> > ## Solution
> >
> > There is no one single answer 🤓
> > {: .output}
> {: .solution}
{: .challenge}

> ## Discussion  
> Scenario:  
You are a marine biology researcher, your group has discovered new organisms, and it's time to create data descriptions. However, there are no available Ontologies to describe the data records, given that they are new scientific discoveries.
> 
> Discuss with your team what the researcher should do given that apparently there are no available Ontologies to describe their data.
{: .discussion}

<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-1JS8K9J9GE"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'G-1JS8K9J9GE');
</script>

<script type="application/ld+json">
{
    "@context": "https://schema.org",
    "@type": "Course",
    "name": "Circular Research Data Bootcamp",
    "description": "This is the coursebook of the Circular Research Data Bootcamp. This coursebook is an Open Educational Resources following the FAIR and Open Science recommendations. A week-long summer camp training looking at real-world examples to achieve data sustainability following the FAIR principles of research data management. ",
    "version": "v1.0",
    "url": "https://doi.org/10.5281/zenodo.6974103",
    "license": "https://creativecommons.org/licenses/by/4.0/legalcode",
    "dateCreated": {
        "@type": "Date",
        "@value": "2022-08-01"
    },
    "datePublished": {
        "@type": "Date",
        "@value": "2022-08-08"
    },
    "inLanguage": {
        "@type": "Language",
        "name": "EN",
        "alternateName": "EN"
    },
    "keywords": [
        "Research Data Management",
        "Research Data Reuse",
        "Bootcamp",
        "Online Summer Camp",
        "FAIR",
        "FAIR Digital Objects"
    ],
    "creator": {
        "@type": "Person",
        "name": "Pedro Hernandez Serrano",
        "givenName": "Pedro",
        "familyName": "Hernandez Serrano",
        "image": "https://avatars.githubusercontent.com/u/12054964?v=4",
        "jobTitle": "Data Steward",
        "email": "p.hernandezserrano@maastrichtuniversity.nl",
        "affiliation": {
            "@type": "Organization",
            "name": "Maastricht University Library",
            "url": {
                "@type": "URL",
                "@value": "https://library.maastrichtuniversity.nl/research/rdm/"
            }
        }
    },
    "contributor": [
        {
            "@type": "Person",
            "givenName": "Maria",
            "familyName": "Vivas Romero",
            "jobTitle": "Data Steward",
            "email": "m.vivasromero@maastrichtuniversity.nl",
            "affiliation": {
                "@type": "Organization",
                "name": "Maastricht University Library",
                "url": {
                    "@type": "URL",
                    "@value": "https://library.maastrichtuniversity.nl/research/rdm/"
                }
            }
        }
    ],
    "publisher": {
        "@type": "Person",
        "name": "Pedro Hernandez Serrano",
        "givenName": "Pedro",
        "familyName": "Hernandez Serrano",
        "jobTitle": "Data Steward",
        "email": "p.hernandezserrano@maastrichtuniversity.nl"
    },
    "citation": {
        "@type": "CreativeWork",
        "name": "Circular Research Data Coursebook",
        "creator": [
            {
                "@type": "Person",
                "name": "Pedro Hernandez Serrano"
            },
            {
                "@type": "Person",
                "name": "Maria Vivas Romero"
            }
        ]
    },
    "learningResourceType": "Coursebook",
    "provider": {
        "@type": "Organization",
        "name": "Maastricht University"
    }
}
</script>