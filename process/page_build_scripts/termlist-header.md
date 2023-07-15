# Plinian Core List of Terms

**Title**  
Plinian Core List of Terms

**Date version issued:**  
2023-07-14

**Date created:**  
2023-07-14

**Part of TDWG Standard:**  
http://www.tdwg.org/standards/643

**This version:**  
http://rs.tdwg.org/plic/doc/list/2023-07-14

**Latest version:**  
http://rs.tdwg.org/plic/doc/list/

**Status**  
Current standard

**Category**  
Technical specification

**Permanent IRI**  
[http://www.tdwg.org/standards/777](http://www.tdwg.org/standards/777)

**Abstract**  
**Plinian Core (PliC)** is a standard for sharing information about species and higher taxa, covering biological and non-biological aspects of all taxonomic groups. It was conceived as a way to publish species information and to make it interoperable. The standard covers all properties and traits related to taxa (of any rank), including descriptions, nomenclature, conservation status, management, natural history, etc. Thus, Plinian Core coverage goes beyond taxonomic descriptions.

Plinian Core is designed to be easy to use, self-contained, supporting data integration from multiple databases, and handling different levels of granularity.

**Creator**  
Species Information Interest Group, [Biodiversity Information Standards (TDWG)](https://www.tdwg.org/)

**Bibliographic citation**  
Plinian Core Maintenance Group. 2022. Plinian Core List of Terms. Biodiversity Information Standards (TDWG). http://rs.tdwg.org/plic/doc/list/2023-07-14

**Institutions and persons**

| Institutions | Persons |
| :------------- | :----------- |
| GBIF Spain - CSIC | Francisco Pando |
| | Santiago Martínez de la Riva |
| | Ramón Pérez Pérez |
| | Gloria Martínez-Sagarra |
| INBIO & CRBIO | Maria Mora |
| | Manuel Vargas |
| | William Ulate |
| | Erick Mata |
| | Jose M. Cuadra |
| | Jaime Gutierrez |
| | Aurelio Sanabria |
| University of Granada | Carmen Quesada |
| Alexander von Humboldt Institute | Camila Plata |
| | Angela Suarez |
| | Danny Velez |
| | Valentina Grajales |
| CONABIO | Patricia Koleff |
| | Esther Quintero |
| | José Mendoza |
| University of São Paulo | Daniel Lins da Silva |
| University Carlos III | Mat Max Montalvo Martínez |

## 1. Introduction
The current version of Plinian Core includes the normative SDS documentation of the standar together with the non-normative [XSD documentation](https://github.com/tdwg/PlinianCore/tree/master/xsd) that establishes the hierarchy of classes and terms  to support species pages publication. For additional information to implement the standard refer to the [Plinian Core wiki](https://github.com/tdwg/PlinianCore/wiki/PlinianCore_Terms).

This SDS normative document contains definitions and XRIs of Plinian Core terms. That is, all terms borrowed from other standards are not included in the SDS document. non-normative documentation includes two sources:

The current abstract modes XML Schema (.XDS) available from the Plinian Core GITHUB repository at:
[https://github.com/tdwg/PlinianCore/tree/master/xsd/abstract models/stable version](https://github.com/tdwg/PlinianCore/tree/master/xsd/abstract%20models/stable%20version)

The documentation presented a the Plinian Core Wiki, available at:
[https://github.com/tdwg/PlinianCore/wiki](https://github.com/tdwg/PlinianCore/wiki)

Both sources contain Plinian Core native terms, and borrowed terms. They also contain a number of intermediate classes (complex terms) that group and provide semantic context to simple terms. These intermediate classes are not described in the SDS.

However, the SDS for each term, provides references to the location of the term in the  .XDS file as an additional way to provide context for the terms and facilitate its implementation (see section “1.4. Equivalent xPath ”).

These non-normative sources provide useful documentation to those aiming to implement Plinian Core.

## 1.1 Status of the content of this document

In Section 4, the values of the `Term IRI`,  `Definition` and `Type` are normative.  The values of `Term Name` are non-normative, although one can expect that the namespace abbreviation prefix is one commonly used for the term namespace, all other values such as  `Label`, `Notes`, and `Equivalent XPath` are non-normative. 

## 1.2 Categories of terms

A Plinian Core (PliC) record is a description of a species or higher taxa. Two kinds of terms are specified by this document: those terms which are part of the PliC vocabulary (e.g. `plic:FullDescription`, `plic:HabitatAndDistribution`, plic:Interactions, among others) and those borrowed from other standards or vocabularies (e.g. tcs:SynonymName and tcs:References are based on concepts described by the TCS vocabulary, see section 2 for details). 

## 1.3 Structured and unstructured properties

Within a class, both structured and unstructured properties can be found. Structured properties may contain other properties in a hierarchical manner or terms with a controlled vocabulary, for example: `plic:invasivenessAtomized` as defined by the XSD non-nomative document and by the XPaths.  Unstructured properties are terms for free text descriptions aimed to give ample details of the species information, for example: `plic:invasivenessUnstructured`.

## 1.4  Equivalent XPath

All the terms and classes include a series of XPaths that make references to the organization and hierarchy of the contents of the standar so the users know how to implement them, the organization of the standard is also refer on the [XSD](https://github.com/tdwg/PlinianCore/tree/master/xsd) as a non-normative part of the standar.

## 2. Borrowed terms
Plinian Core ,--following good practices-- re-uses a number of elements already defined by other data specifications. This is an important consideration in advancing towards robust semantic web architecture for biodiversity information. The following table presents the vocabularies from which terms have been borrowed:

Table 1. Vocabularies from which terms have been borrowed:

|Specifications|Abbreviation|Borrowed Terms|
|:----|:----|:----|
|[Darwin Core](https://dwc.tdwg.org/terms/)|DwC|[dwc:taxonConceptID](https://dwc.tdwg.org/terms/#dwc:taxonConceptID), [kingdom](https://dwc.tdwg.org/terms/#dwc:kingdom), [phylum](https://dwc.tdwg.org/terms/#dwc:phylum), [class](https://dwc.tdwg.org/terms/#dwc:class), [order](https://dwc.tdwg.org/terms/#dwc:order), [family](https://dwc.tdwg.org/terms/#dwc:family), [subfamily](https://dwc.tdwg.org/terms/#dwc:subfamily), [genus](https://dwc.tdwg.org/terms/#dwc:genus), [genericName](https://dwc.tdwg.org/terms/#dwc:genericName), [subgenus](https://dwc.tdwg.org/terms/#dwc:subgenus), [specificEpithet](https://dwc.tdwg.org/terms/#dwc:specificEpithet), [infragenericEpithet](https://dwc.tdwg.org/terms/#dwc:infragenericEpithet), [cultivarEpithet](https://dwc.tdwg.org/terms/#dwc:cultivarEpithet), [taxonRank](https://dwc.tdwg.org/terms/#dwc:taxonRank), [higherClassification](https://dwc.tdwg.org/terms/#dwc:higherClassification), [MeasurementOrFact](https://dwc.tdwg.org/terms/#measurementorfact), [ResourceRelationShip](https://dwc.tdwg.org/terms/#resourcerelationship)|
|[Dublin Core](http://dublincore.org/documents/dcmi-terms/)|DC|dc:created|
|[Encyclopedia of Life](https://eol.org/docs/what-is-eol/language-support)|EOL|eol:AncillaryData, eol:References|
|[Taxonomic Concept Transfer Schema](https://www.tdwg.org/standards/tcs/)|TCS|tcs:scientificName, tcs:ReferenceType|
|[Global Invasive Species Information Network](https://github.com/tdwg/gisin)|GISIN|gisin:origin, gisin:presence, gisin:persistence, gisin:distribution, gisin:harmful, gisin:modified, gisin:startValidDate, endValidDate, gisin:countryCode, gisin:stateProvince, gisin:county, gisin:localityName, gisin:county, gisin:language, gisin:citation, gisin:abundance, gisin:trend, gisin:rateOfSpread, gisin:regulatoryListing,gisin:memo, gisin:publicationDate, gisin:localityType, gisin:locationValue, gisin:publicationDatePrecision|
|[Ecological Metadata Language](https://eml.ecoinformatics.org/)|EML|GBIF EML profile|
