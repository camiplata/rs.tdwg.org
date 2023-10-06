# Plinian Core List of Terms

**Title**  
Plinian Core List of Terms

**Date version issued:**  
2023-10-06

**Date created:**  
2023-10-06

**Part of TDWG Standard:**  
http://www.tdwg.org/standards/643

**This version:**  
http://rs.tdwg.org/plic/doc/list/2023-10-06

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
### 3.1 Index By Term Name

(See also [3.2 Index By Label](#32-index-by-label))

**Classes**

[plic:References](#plic_References) 

**Dataset Metadata**

[plic:Dataset_ID](#plic_Dataset_ID) |
[plic:References](#plic_References) 

**Record Metadata**

[plic:Audience](#plic_Audience) |
[plic:Revision](#plic_Revision) |
[plic:abstract](#plic_abstract) 

**Nomenclature And Classification**

[plic:CommonName](#plic_CommonName) |
[plic:UsedBy](#plic_UsedBy) |
[plic:commonNamesUnstructured](#plic_commonNamesUnstructured) |
[plic:detailAtomized](#plic_detailAtomized) 

**Taxonomic Description**

**Life Form**

**Life Cycle**

**Reproduction**

**Annual Cycles**

[plic:AnnualCycleUnstructured](#plic_AnnualCycleUnstructured) |
[plic:EndTimeInterval](#plic_EndTimeInterval) |
[plic:Event](#plic_Event) |
[plic:StartTimeInterval](#plic_StartTimeInterval) 

**Feeding**

[plic:FeedingType](#plic_FeedingType) |
[plic:TrophicStrategy](#plic_TrophicStrategy) |
[plic:TrophicStrategyRemarks](#plic_TrophicStrategyRemarks) |
[plic:feedingUnstructured](#plic_feedingUnstructured) 

**Dispersal**

[plic:DispersalMeans](#plic_DispersalMeans) |
[plic:DispersalUnstructured](#plic_DispersalUnstructured) |
[plic:Distance](#plic_Distance) |
[plic:StructureDispersed](#plic_StructureDispersed) 

**Behavior**

**Interactions**

[plic:SpeciesInteractionType](#plic_SpeciesInteractionType) 

**Molecular Data**

**Migratory**

**Ecological Significance**

[plic:ecologicalSignificanceAtomized](#plic_ecologicalSignificanceAtomized) |
[plic:ecologicalSignificanceUnstructured](#plic_ecologicalSignificanceUnstructured) 

**Environmental Envelope**

[plic:environmentalEnvelopeAtomized](#plic_environmentalEnvelopeAtomized) |
[plic:environmentalEnvelopeUnstructured](#plic_environmentalEnvelopeUnstructured) 

**Natural History**

**Invasiveness**

[plic:Route](#plic_Route) |
[plic:WhatImpact](#plic_WhatImpact) |
[plic:impactMechanism](#plic_impactMechanism) |
[plic:impactTarget](#plic_impactTarget) |
[plic:invasivenessUnstructured](#plic_invasivenessUnstructured) |
[plic:vector](#plic_vector) 

**Habitat And Distribution**

[plic:DistributionScope](#plic_DistributionScope) |
[plic:DistributionUnstructured](#plic_DistributionUnstructured) |
[plic:EndemicIn](#plic_EndemicIn) |
[plic:EndemicTo](#plic_EndemicTo) |
[plic:GeographicEntity](#plic_GeographicEntity) |
[plic:endemicUnstructured](#plic_endemicUnstructured) |
[plic:habitatAndDistributionUnstructured](#plic_habitatAndDistributionUnstructured) |
[plic:habitatAtomized](#plic_habitatAtomized) |
[plic:habitatUnstructured](#plic_habitatUnstructured) 

**Demography And Threat**

[plic:AbundanceData](#plic_AbundanceData) |
[plic:AreaOfOccupancy](#plic_AreaOfOccupancy) |
[plic:AverageDensity](#plic_AverageDensity) |
[plic:BirthRate](#plic_BirthRate) |
[plic:CarryingCapacity](#plic_CarryingCapacity) |
[plic:DensityData](#plic_DensityData) |
[plic:DescriptionLifeStages](#plic_DescriptionLifeStages) |
[plic:DirectThreatAtomized](#plic_DirectThreatAtomized) |
[plic:Emigration](#plic_Emigration) |
[plic:ExtentOfOccurrence](#plic_ExtentOfOccurrence) |
[plic:Fecundity](#plic_Fecundity) |
[plic:Immigration](#plic_Immigration) |
[plic:LegislationName](#plic_LegislationName) |
[plic:LegislationRead](#plic_LegislationRead) |
[plic:MortalityRate](#plic_MortalityRate) |
[plic:NumberIndividualsPerObservation](#plic_NumberIndividualsPerObservation) |
[plic:PatternDistribution](#plic_PatternDistribution) |
[plic:PopulationGrowthRate](#plic_PopulationGrowthRate) |
[plic:PopulationTrend](#plic_PopulationTrend) |
[plic:ProportionIndividualsPerStageLife](#plic_ProportionIndividualsPerStageLife) |
[plic:ProtectionLegalStatus](#plic_ProtectionLegalStatus) |
[plic:Recruitment](#plic_Recruitment) |
[plic:SexRatio](#plic_SexRatio) |
[plic:Size](#plic_Size) |
[plic:demographyAndThreatUnstructured](#plic_demographyAndThreatUnstructured) |
[plic:legalNorm](#plic_legalNorm) |
[plic:legislationStatus](#plic_legislationStatus) |
[plic:legislationType](#plic_legislationType) |
[plic:legislationUnstructured](#plic_legislationUnstructured) 

**Uses Management And Conservation**

[plic:Actions](#plic_Actions) |
[plic:ActionsType](#plic_ActionsType) |
[plic:Conservation-ExplotationData](#plic_Conservation-ExplotationData) |
[plic:Economics](#plic_Economics) |
[plic:HumanAndEnvironmentalrelevance](#plic_HumanAndEnvironmentalrelevance) |
[plic:ManagementPlan](#plic_ManagementPlan) |
[plic:MeansOfApplication-Administration](#plic_MeansOfApplication-Administration) |
[plic:Objectives](#plic_Objectives) |
[plic:Organisms](#plic_Organisms) |
[plic:PartUsed](#plic_PartUsed) |
[plic:Potential](#plic_Potential) |
[plic:ProductionDetails](#plic_ProductionDetails) |
[plic:Properties](#plic_Properties) |
[plic:RatingPopularity](#plic_RatingPopularity) |
[plic:SeasonOfAvailability-Use](#plic_SeasonOfAvailability-Use) |
[plic:Use-Value](#plic_Use-Value) |
[plic:UseNotes](#plic_UseNotes) |
[plic:UseType](#plic_UseType) |
[plic:Users](#plic_Users) |
[plic:UsesManagementAndConservationUnstructured](#plic_UsesManagementAndConservationUnstructured) |
[plic:UsesUnstructured](#plic_UsesUnstructured) |
[plic:VernacularNameUseAnnotations](#plic_VernacularNameUseAnnotations) 

**Associated Party**

**Ancillary Data**

### 3.2 Index By Label

(See also [3.1 Index By Term Name](#31-index-by-term-name))

**Classes**

[References](#plic_References) 

**Dataset Metadata**

[Dataset ID](#plic_Dataset_ID) |
[References](#plic_References) 

**Record Metadata**

[Abstract](#plic_abstract) |
[Audience](#plic_Audience) |
[Revision](#plic_Revision) 

**Nomenclature And Classification**

[Atomized Detail](#plic_detailAtomized) |
[Common Name](#plic_CommonName) |
[Used By](#plic_UsedBy) |
[unstructured common names](#plic_commonNamesUnstructured) 

**Taxonomic Description**

**Life Form**

**Life Cycle**

**Reproduction**

**Annual Cycles**

[End Time Interval](#plic_EndTimeInterval) |
[Event](#plic_Event) |
[Start Time Interval](#plic_StartTimeInterval) |
[Unstructured Annual Cycle](#plic_AnnualCycleUnstructured) 

**Feeding**

[Feeding Type](#plic_FeedingType) |
[Trophic Strategy](#plic_TrophicStrategy) |
[Trophic Strategy Remarks](#plic_TrophicStrategyRemarks) |
[Unstructured Feeding](#plic_feedingUnstructured) 

**Dispersal**

[Dispersal Means](#plic_DispersalMeans) |
[Distance](#plic_Distance) |
[Structure Dispersed ](#plic_StructureDispersed) |
[Unstructured Dispersal](#plic_DispersalUnstructured) 

**Behavior**

**Interactions**

[Species Interaction Type](#plic_SpeciesInteractionType) 

**Molecular Data**

**Migratory**

**Ecological Significance**

[Atomized Ecological Significance](#plic_ecologicalSignificanceAtomized) |
[Unstructured Ecological Significance](#plic_ecologicalSignificanceUnstructured) 

**Environmental Envelope**

[Atomized Environmental Envelope](#plic_environmentalEnvelopeAtomized) |
[Unstructured Environmental Envelope](#plic_environmentalEnvelopeUnstructured) 

**Natural History**

**Invasiveness**

[Impact Mechanism](#plic_impactMechanism) |
[Impact Target](#plic_impactTarget) |
[Route](#plic_Route) |
[Unstructured Invasiveness](#plic_invasivenessUnstructured) |
[Vector](#plic_vector) |
[What Impact](#plic_WhatImpact) 

**Habitat And Distribution**

[Atomized Habitat](#plic_habitatAtomized) |
[Distribution Scope](#plic_DistributionScope) |
[Endemic In](#plic_EndemicIn) |
[Endemic To](#plic_EndemicTo) |
[Geographic Entity](#plic_GeographicEntity) |
[Unstructured Distribution](#plic_DistributionUnstructured) |
[Unstructured Endemic](#plic_endemicUnstructured) |
[Unstructured Habitat](#plic_habitatUnstructured) |
[Unstructured Habitat And Distribution](#plic_habitatAndDistributionUnstructured) 

**Demography And Threat**

[AbundanceData](#plic_AbundanceData) |
[Area of occupancy](#plic_AreaOfOccupancy) |
[Atomized Direct Threat](#plic_DirectThreatAtomized) |
[Average density](#plic_AverageDensity) |
[Birth rate](#plic_BirthRate) |
[Carrying capacity](#plic_CarryingCapacity) |
[DensityData](#plic_DensityData) |
[Description life stages](#plic_DescriptionLifeStages) |
[Emigration](#plic_Emigration) |
[Extent of occurrence](#plic_ExtentOfOccurrence) |
[Fecundity](#plic_Fecundity) |
[Immigration](#plic_Immigration) |
[Legal Norm](#plic_legalNorm) |
[Legislation Name](#plic_LegislationName) |
[Legislation Read](#plic_LegislationRead) |
[Legislation Status](#plic_legislationStatus) |
[Legislation Type](#plic_legislationType) |
[Mortality rate](#plic_MortalityRate) |
[Number individuals per observation](#plic_NumberIndividualsPerObservation) |
[Pattern distribution](#plic_PatternDistribution) |
[Population growth rate](#plic_PopulationGrowthRate) |
[Population trend](#plic_PopulationTrend) |
[ProportionIndividuals per stage life](#plic_ProportionIndividualsPerStageLife) |
[Protection Legal Status](#plic_ProtectionLegalStatus) |
[Recruitment](#plic_Recruitment) |
[SexRatio](#plic_SexRatio) |
[Size](#plic_Size) |
[Unstructured Demography And Threat](#plic_demographyAndThreatUnstructured) |
[Unstructured Legislation](#plic_legislationUnstructured) 

**Uses Management And Conservation**

[Actions](#plic_Actions) |
[Actions Type](#plic_ActionsType) |
[Conservation-Explotation Data](#plic_Conservation-ExplotationData) |
[Economics](#plic_Economics) |
[Human and Environmental Relevance](#plic_HumanAndEnvironmentalrelevance) |
[Management Plan](#plic_ManagementPlan) |
[Means of Application-Administration](#plic_MeansOfApplication-Administration) |
[Objectives](#plic_Objectives) |
[Organisms](#plic_Organisms) |
[Part Used](#plic_PartUsed) |
[Potential](#plic_Potential) |
[Production Details](#plic_ProductionDetails) |
[Properties](#plic_Properties) |
[Rating Popularity](#plic_RatingPopularity) |
[Season of Availability-Use](#plic_SeasonOfAvailability-Use) |
[Unstructured Uses](#plic_UsesUnstructured) |
[Use Notes](#plic_UseNotes) |
[Use Type](#plic_UseType) |
[Use-Value](#plic_Use-Value) |
[Users](#plic_Users) |
[Uses Management and Conservation Unstructured ](#plic_UsesManagementAndConservationUnstructured) |
[Vernacular Name Use Annotations](#plic_VernacularNameUseAnnotations) 

**Associated Party**

**Ancillary Data**

## 4 Vocabulary
### 4.1 Dataset Metadata

Information about the collections of records.<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_Dataset_ID"></a>Term Name  plic:Dataset_ID</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/Dataset_ID">http://rs.tdwg.org/plic/terms/Dataset_ID</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/Dataset_ID-2023-10-06">http://rs.tdwg.org/plic/terms/version/Dataset_ID-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Dataset ID</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>An identifier for the dataset.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/Metadata/Dataset_ID</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_References"></a>Term Name  plic:References</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/References">http://rs.tdwg.org/plic/terms/References</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/References-2023-10-06">http://rs.tdwg.org/plic/terms/version/References-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>References</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>It represents the references that an element could have, in one or more of the different format and schemas: BICI, CODEN,DOI, EISSN, HANDLE, ISBN, ISSN, LSID, OCLC, SICI, URL, URN</td>
		</tr>
		<tr>
			<td>Notes</td>
			<td>Definition borrowed from EOL: referenceType.</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Class</td>
		</tr>
	</tbody>
</table>


### 4.2 Record Metadata

Information about the Version, Revision, the language and target audiences of the Taxon Record.<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_Audience"></a>Term Name  plic:Audience</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/Audience">http://rs.tdwg.org/plic/terms/Audience</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/Audience-2023-10-06">http://rs.tdwg.org/plic/terms/version/Audience-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Audience</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Repetitive concept where the target audiences are written one by one.</td>
		</tr>
		<tr>
			<td>Notes</td>
			<td>Predetermined list: 01. Expert (High). 02. Knowledgeable (Medium). 03. General (Low).</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>
				<details>
					<summary>Show all 89 XPaths</summary>
/Dataset/AncillaryData/audience<br/>/Dataset/TaxonRecord/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/DirectThreats/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/DirectThreats/DirectThreatAtomized/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/Legislation/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/Legislation/LegislationAtomized/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/Legislation/LegislationAtomized/AppliesTo/DistributionScope/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/AbundanceData/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/AverageDensity/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/BirthRate/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/CarryingCapacity/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/DensityData/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/DescriptionLifeStages/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/Emigration/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/Fecundity/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/Immigration/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/MortalityRate/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/NumberIndividualsPerObservation/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/PatternDistribution/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/PopulationGrowthRate/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/PopulationTrend/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/ProportionIndividualsPerStageLife/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/Recruitment/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/SexRatio/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/Size/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/Territory/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/Territory/TerritoryAtomized/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/Territory/TerritoryAtomized/AreaOfOccupancy/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/Territory/TerritoryAtomized/ExtentOfOccurrence/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/ThreatStatus/AncillaryData/audience<br/>/Dataset/TaxonRecord/DemographyAndThreat/ThreatStatus/ThreatStatusAtomized/AppliesTo/DistributionScope/AncillaryData/audience<br/>/Dataset/TaxonRecord/HabitatAndDistribution/AncillaryData/audience<br/>/Dataset/TaxonRecord/HabitatAndDistribution/Distribution/DistributionScope/AncillaryData/audience<br/>/Dataset/TaxonRecord/HabitatAndDistribution/Endemic/AncillaryData/audience<br/>/Dataset/TaxonRecord/HabitatAndDistribution/Endemic/EndemicAtomized/AncillaryData/audience<br/>/Dataset/TaxonRecord/HabitatAndDistribution/Habitats/AncillaryData/audience<br/>/Dataset/TaxonRecord/HabitatAndDistribution/Habitats/HabitatAtomized/AncillaryData/audience<br/>/Dataset/TaxonRecord/Invasiveness/AncillaryData/audience<br/>/Dataset/TaxonRecord/Invasiveness/InvasivenessAtomized/AncillaryData/audience<br/>/Dataset/TaxonRecord/NaturalHistory/AncillaryData/audience<br/>/Dataset/TaxonRecord/NaturalHistory/AnnualCycles/AncillaryData/audience<br/>/Dataset/TaxonRecord/NaturalHistory/AnnualCycles/AnnualCycleAtomized/AncillaryData/audience<br/>/Dataset/TaxonRecord/NaturalHistory/Behavior/AncillaryData/audience<br/>/Dataset/TaxonRecord/NaturalHistory/Behavior/BehaviorAtomized/AncillaryData/audience<br/>/Dataset/TaxonRecord/NaturalHistory/Dispersal/AncillaryData/audience<br/>/Dataset/TaxonRecord/NaturalHistory/Dispersal/DispersalAtomized/AncillaryData/audience<br/>/Dataset/TaxonRecord/NaturalHistory/EcologicalSignificance/AncillaryData/audience<br/>/Dataset/TaxonRecord/NaturalHistory/EcologicalSignificance/EcologicalSignificanceAtomized/AncillaryData/audience<br/>/Dataset/TaxonRecord/NaturalHistory/EnvironmentalEnvelope/AncillaryData/audience<br/>/Dataset/TaxonRecord/NaturalHistory/EnvironmentalEnvelope/EnvironmentalEnvelopeAtomized/AncillaryData/audience<br/>/Dataset/TaxonRecord/NaturalHistory/Feeding/AncillaryData/audience<br/>/Dataset/TaxonRecord/NaturalHistory/Feeding/FeedingAtomized/AncillaryData/audience<br/>/Dataset/TaxonRecord/NaturalHistory/Interactions/AncillaryData/audience<br/>/Dataset/TaxonRecord/NaturalHistory/Interactions/InteractionAtomized/AncillaryData/audience<br/>/Dataset/TaxonRecord/NaturalHistory/LifeCycle/AncillaryData/audience<br/>/Dataset/TaxonRecord/NaturalHistory/LifeCycle/LifeCycleAtomized/AncillaryData/audience<br/>/Dataset/TaxonRecord/NaturalHistory/LifeForm/AncillaryData/audience<br/>/Dataset/TaxonRecord/NaturalHistory/LifeForm/LifeFormAtomized/AncillaryData/audience<br/>/Dataset/TaxonRecord/NaturalHistory/Migratory/AncillaryData/audience<br/>/Dataset/TaxonRecord/NaturalHistory/Migratory/MigratoryAtomized/AncillaryData/audience<br/>/Dataset/TaxonRecord/NaturalHistory/MiscDetails/AncillaryData/audience<br/>/Dataset/TaxonRecord/NaturalHistory/MiscDetails/DetailAtomized/AncillaryData/audience<br/>/Dataset/TaxonRecord/NaturalHistory/MolecularData/AncillaryData/audience<br/>/Dataset/TaxonRecord/NaturalHistory/MolecularData/MolecularDataAtomized/AncillaryData/audience<br/>/Dataset/TaxonRecord/NaturalHistory/Reproduction/AncillaryData/audience<br/>/Dataset/TaxonRecord/NaturalHistory/Reproduction/ReproductionAtomized/AncillaryData/audience<br/>/Dataset/TaxonRecord/NomenclatureAndClassification/AncillaryData/audience<br/>/Dataset/TaxonRecord/NomenclatureAndClassification/CommonNames/AncillaryData/audience<br/>/Dataset/TaxonRecord/NomenclatureAndClassification/CommonNames/CommonNamesAtomized/AncillaryData/audience<br/>/Dataset/TaxonRecord/NomenclatureAndClassification/CommonNames/CommonNamesAtomized/UsedIn/DistributionScope/AncillaryData/audience<br/>/Dataset/TaxonRecord/NomenclatureAndClassification/Hierarchy/AncillaryData/audience<br/>/Dataset/TaxonRecord/NomenclatureAndClassification/MiscDetails/AncillaryData/audience<br/>/Dataset/TaxonRecord/NomenclatureAndClassification/MiscDetails/DetailAtomized/AncillaryData/audience<br/>/Dataset/TaxonRecord/NomenclatureAndClassification/Synonyms/AncillaryData/audience<br/>/Dataset/TaxonRecord/NomenclatureAndClassification/Synonyms/SynonymsAtomized/AncillaryData/audience<br/>/Dataset/TaxonRecord/NomenclatureAndClassification/TaxonRecordName/AncillaryData/audience<br/>/Dataset/TaxonRecord/RecordMetadata/TargetAudiences/Audience<br/>/Dataset/TaxonRecord/TaxonomicDescription/AncillaryData/audience<br/>/Dataset/TaxonRecord/TaxonomicDescription/FullDescription/AncillaryData/audience<br/>/Dataset/TaxonRecord/TaxonomicDescription/FullDescription/FullDescriptionAtomized/AncillaryData/audience<br/>/Dataset/TaxonRecord/TaxonomicDescription/IdentificationKeys/AncillaryData/audience<br/>/Dataset/TaxonRecord/UsesManagementAndConservation/AncillaryData/audience<br/>/Dataset/TaxonRecord/UsesManagementAndConservation/ManagementAndConservation/AncillaryData/audience<br/>/Dataset/TaxonRecord/UsesManagementAndConservation/ManagementAndConservation/ManagementAndConservationAtomized/AncillaryData/audience<br/>/Dataset/TaxonRecord/UsesManagementAndConservation/Uses/AncillaryData/audience<br/>/Dataset/TaxonRecord/UsesManagementAndConservation/Uses/UsesAtomized/AncillaryData/audience
</details>
</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>http://www.w3.org/2004/02/skos/core#ConceptScheme</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_Revision"></a>Term Name  plic:Revision</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/Revision">http://rs.tdwg.org/plic/terms/Revision</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/Revision-2023-10-06">http://rs.tdwg.org/plic/terms/version/Revision-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Revision</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Creators, revision status and dates of the record.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/RecordMetadata/Revision</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_abstract"></a>Term Name  plic:abstract</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/abstract">http://rs.tdwg.org/plic/terms/abstract</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/abstract-2023-10-06">http://rs.tdwg.org/plic/terms/version/abstract-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Abstract</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>A brief summary of the most relevant or attractive features of this taxon to the general public. Could point to any kind of information. </td>
		</tr>
		<tr>
			<td>Notes</td>
			<td>Example: Blue whale is the largest mammal in the world. </td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/Metadata/dataset/abstract<br/>/Dataset/TaxonRecord/BaseElements/Abstract</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>


### 4.3 Nomenclature And Classification

Information on the taxon's name, synomyms, nomenclatural status, common names, and taxonomic hierarchy; plus misc. details and ancillary data<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_CommonName"></a>Term Name  plic:CommonName</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/CommonName">http://rs.tdwg.org/plic/terms/CommonName</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/CommonName-2023-10-06">http://rs.tdwg.org/plic/terms/version/CommonName-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Common Name</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>The name of the common name. </td>
		</tr>
		<tr>
			<td>Notes</td>
			<td>From GBIF EML profile</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/NomenclatureAndClassification/CommonNames/CommonNamesAtomized/CommonName</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_UsedBy"></a>Term Name  plic:UsedBy</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/UsedBy">http://rs.tdwg.org/plic/terms/UsedBy</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/UsedBy-2023-10-06">http://rs.tdwg.org/plic/terms/version/UsedBy-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Used By</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Sometimes names used by one group of people are adopted by another. </td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/NomenclatureAndClassification/CommonNames/CommonNamesAtomized/UsedBy</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>http://www.w3.org/1999/02/22-rdf-syntax-ns#Property </td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_commonNamesUnstructured"></a>Term Name  plic:commonNamesUnstructured</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/commonNamesUnstructured">http://rs.tdwg.org/plic/terms/commonNamesUnstructured</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/commonNamesUnstructured-2023-10-06">http://rs.tdwg.org/plic/terms/version/commonNamesUnstructured-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>unstructured common names</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>CommonNames element in text block format.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/NomenclatureAndClassification/CommonNames/CommonNamesUnstructured</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_detailAtomized"></a>Term Name  plic:detailAtomized</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/detailAtomized">http://rs.tdwg.org/plic/terms/detailAtomized</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/detailAtomized-2023-10-06">http://rs.tdwg.org/plic/terms/version/detailAtomized-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Atomized Detail</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>MiscDetail element in structured format.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/NaturalHistory/MiscDetails/DetailAtomized<br/>/Dataset/TaxonRecord/NomenclatureAndClassification/MiscDetails/DetailAtomized</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>


### 4.4 Taxonomic Description

Description of Taxon: Brief description, Full description, Identification keys and Ancillary Data
### 4.5 Life Form

General appearance. Characteristic mode of growth or occurrence associated to the environment, particularly for plants. Comprising the size, shape, texture and orientation
### 4.6 Life Cycle

Life history of a living organism: The course of developmental changes in an organism from fertilized zygote to maturity or stages through which an organism passes.
### 4.7 Reproduction

All data related to the generation of offspring
### 4.8 Annual Cycles

Set of changes or events that recurrently take place at the same time of year and are influenced by seasonal and interannual climate variations. For example: reproduction, flowering, fruiting, emergence of insects, etc. Also called phenology, mainly in plants. In the case of migration, it only makes reference to the timing; other data about this are gathered in MigratoryData.<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_AnnualCycleUnstructured"></a>Term Name  plic:AnnualCycleUnstructured</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/AnnualCycleUnstructured">http://rs.tdwg.org/plic/terms/AnnualCycleUnstructured</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/AnnualCycleUnstructured-2023-10-06">http://rs.tdwg.org/plic/terms/version/AnnualCycleUnstructured-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Unstructured Annual Cycle</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>AnnualCyles element in text block format. </td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/NaturalHistory/AnnualCycles/AnnualCycleUnstructured</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_EndTimeInterval"></a>Term Name  plic:EndTimeInterval</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/EndTimeInterval">http://rs.tdwg.org/plic/terms/EndTimeInterval</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/EndTimeInterval-2023-10-06">http://rs.tdwg.org/plic/terms/version/EndTimeInterval-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>End Time Interval</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>The date-time or interval at which an event ends. Recommended best practice is to use an encoding scheme, such as ISO 8601:2004(E). A controlled vocabulary is recommended.</td>
		</tr>
		<tr>
			<td>Notes</td>
			<td>e.g. "1963-03-08T14:07-0600" is 8 Mar 1963 2:07pm in the time zone six hours earlier than UTC, "2009-02-20T08:40Z" is 20 Feb 2009 8:40am UTC, "1809-02-12" is 12 Feb 1809, "1906-06" is Jun 1906, "1971" is just that year, "2007-03-01T13:00:00Z/2008-05-11T15:30:00Z" is the interval between 1 Mar 2007 1pm UTC and 11 May 2008 3:30pm UTC, "2007-11-13/15" is the interval between 13 Nov 2007 and 15 Nov 2007.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/NaturalHistory/AnnualCycles/AnnualCycleAtomized/endTimeInterval</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_Event"></a>Term Name  plic:Event</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/Event">http://rs.tdwg.org/plic/terms/Event</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/Event-2023-10-06">http://rs.tdwg.org/plic/terms/version/Event-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Event</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>An action that occurs at some location during some time. A controlled vocabulary is recommended.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/NaturalHistory/AnnualCycles/AnnualCycleAtomized/Event</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_StartTimeInterval"></a>Term Name  plic:StartTimeInterval</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/StartTimeInterval">http://rs.tdwg.org/plic/terms/StartTimeInterval</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/StartTimeInterval-2023-10-06">http://rs.tdwg.org/plic/terms/version/StartTimeInterval-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Start Time Interval</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>The date-time or interval at which an event starts. Recommended best practice is to use an encoding scheme, such as ISO 8601:2004(E). A controlled vocabulary is recommended.</td>
		</tr>
		<tr>
			<td>Notes</td>
			<td>e.g. "1963-03-08T14:07-0600" is 8 Mar 1963 2:07pm in the time zone six hours earlier than UTC, "2009-02-20T08:40Z" is 20 Feb 2009 8:40am UTC, "1809-02-12" is 12 Feb 1809, "1906-06" is Jun 1906, "1971" is just that year, "2007-03-01T13:00:00Z/2008-05-11T15:30:00Z" is the interval between 1 Mar 2007 1pm UTC and 11 May 2008 3:30pm UTC, "2007-11-13/15" is the interval between 13 Nov 2007 and 15 Nov 2007.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/NaturalHistory/AnnualCycles/AnnualCycleAtomized/startTimeInterval</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>


### 4.9 Feeding

Information related to the food supply for the development and sustenance of the individual and/or its offspring<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_FeedingType"></a>Term Name  plic:FeedingType</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/FeedingType">http://rs.tdwg.org/plic/terms/FeedingType</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/FeedingType-2023-10-06">http://rs.tdwg.org/plic/terms/version/FeedingType-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Feeding Type</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Primary diet source. A controlled vocabulary is recommended.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/NaturalHistory/Feeding/FeedingAtomized/FeedingType</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_TrophicStrategy"></a>Term Name  plic:TrophicStrategy</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/TrophicStrategy">http://rs.tdwg.org/plic/terms/TrophicStrategy</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/TrophicStrategy-2023-10-06">http://rs.tdwg.org/plic/terms/version/TrophicStrategy-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Trophic Strategy</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Tactic used to obtain energy or nutrients. A controlled vocabulary is recommended. e.g. Chemosynthetic organisms, Photosynthetic organisms, Parasites, Decomposers, Suspension feeders, Substrate feeders, Grazers, Fluid-feeders, Predators...</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/NaturalHistory/Feeding/FeedingAtomized/Thropic/TrophicStrategy</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>http://www.w3.org/2004/02/skos/core#ConceptScheme</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_TrophicStrategyRemarks"></a>Term Name  plic:TrophicStrategyRemarks</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/TrophicStrategyRemarks">http://rs.tdwg.org/plic/terms/TrophicStrategyRemarks</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/TrophicStrategyRemarks-2023-10-06">http://rs.tdwg.org/plic/terms/version/TrophicStrategyRemarks-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Trophic Strategy Remarks</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Information notes about specific feeding strategies.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/NaturalHistory/Feeding/FeedingAtomized/Thropic/TrophicStrategyRemarks</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>http://www.w3.org/2004/02/skos/core#ConceptScheme</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_feedingUnstructured"></a>Term Name  plic:feedingUnstructured</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/feedingUnstructured">http://rs.tdwg.org/plic/terms/feedingUnstructured</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/feedingUnstructured-2023-10-06">http://rs.tdwg.org/plic/terms/version/feedingUnstructured-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Unstructured Feeding</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>feeding element in text block format.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/NaturalHistory/Feeding/FeedingUnstructured</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>


### 4.10 Dispersal

The permanent spreading of individuals away from each other not including return. Dispersal determines the range over which genetic mixing occurs, and thus, the degree of homogeneity and inbreeding in a population.<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_DispersalMeans"></a>Term Name  plic:DispersalMeans</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/DispersalMeans">http://rs.tdwg.org/plic/terms/DispersalMeans</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/DispersalMeans-2023-10-06">http://rs.tdwg.org/plic/terms/version/DispersalMeans-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Dispersal Means</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>VCR. Zoochory, Anemochory, Hydrochory, Barochory, Autochory.</td>
		</tr>
		<tr>
			<td>Notes</td>
			<td>Type of dispersal, a controlled vocabulary is recommended.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/NaturalHistory/Dispersal/DispersalAtomized/DispersalMeans</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>http://www.w3.org/2004/02/skos/core#ConceptScheme </td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_DispersalUnstructured"></a>Term Name  plic:DispersalUnstructured</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/DispersalUnstructured">http://rs.tdwg.org/plic/terms/DispersalUnstructured</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/DispersalUnstructured-2023-10-06">http://rs.tdwg.org/plic/terms/version/DispersalUnstructured-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Unstructured Dispersal</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Dispersal element in text block format.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/NaturalHistory/Dispersal/DispersalUnstructured</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_Distance"></a>Term Name  plic:Distance</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/Distance">http://rs.tdwg.org/plic/terms/Distance</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/Distance-2023-10-06">http://rs.tdwg.org/plic/terms/version/Distance-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Distance</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>The distance reached by the structured dispersed.</td>
		</tr>
		<tr>
			<td>Notes</td>
			<td>It includes elements of type MeasurementOrFact</td>
		</tr>
		<tr>
			<td>Examples</td>
			<td>Dispersal distance. e.g. 450 m. </td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/NaturalHistory/Dispersal/DispersalAtomized/Distance</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>http://www.w3.org/1999/02/22-rdf-syntax-ns#Property </td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_StructureDispersed"></a>Term Name  plic:StructureDispersed</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/StructureDispersed">http://rs.tdwg.org/plic/terms/StructureDispersed</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/StructureDispersed-2023-10-06">http://rs.tdwg.org/plic/terms/version/StructureDispersed-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Structure Dispersed </td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>VCR: Seed, Fruit, Vegetative structure, Spores, Gametes, Eggs, Offspring and Individuals.</td>
		</tr>
		<tr>
			<td>Notes</td>
			<td>Structured that is dispersed for a given biologial propose, a controlled vocabulary is recommended.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/NaturalHistory/Dispersal/DispersalAtomized/StructureDispersed</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>http://www.w3.org/2004/02/skos/core#ConceptScheme </td>
		</tr>
	</tbody>
</table>


### 4.11 Behavior

Responses, reactions or movements made by an organism in a particular situation
### 4.12 Interactions

Mutual or reciprocal actions or influences. For example, predation, parasitism, mutualism, etc. Relations with products grown and stored by man (plagues) are also included.<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_SpeciesInteractionType"></a>Term Name  plic:SpeciesInteractionType</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/SpeciesInteractionType">http://rs.tdwg.org/plic/terms/SpeciesInteractionType</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/SpeciesInteractionType-2023-10-06">http://rs.tdwg.org/plic/terms/version/SpeciesInteractionType-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Species Interaction Type</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>String with the type of interaction. Each element is separated by comma and each list of elements by.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/NaturalHistory/Interactions/InteractionAtomized/SpeciesInteractionType</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>


### 4.13 Molecular Data

Information on the chemical structures and biological processes at the molecular level: DNA and proteins sequences, protein structures, expression profiles of genes protein domains, families of genes, mutations, polymorphisms, involvement in disease, ... Placeholder for connecting with standards developed by specialists, e.g. Standards for Data Exchange and Management from Scalalife (http://www.scalalife.eu/content/data.html).
### 4.14 Migratory

The regular, usually seasonal, movement of all or part of an animal population to and from a given area, which can occur in variable periods of time and even involve more than one generation.
### 4.15 Ecological Significance

Ecological importance of the taxon<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_ecologicalSignificanceAtomized"></a>Term Name  plic:ecologicalSignificanceAtomized</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/ecologicalSignificanceAtomized">http://rs.tdwg.org/plic/terms/ecologicalSignificanceAtomized</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/ecologicalSignificanceAtomized-2023-10-06">http://rs.tdwg.org/plic/terms/version/ecologicalSignificanceAtomized-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Atomized Ecological Significance</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Ecological Significance element in structured format.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/NaturalHistory/EcologicalSignificance/EcologicalSignificanceAtomized</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_ecologicalSignificanceUnstructured"></a>Term Name  plic:ecologicalSignificanceUnstructured</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/ecologicalSignificanceUnstructured">http://rs.tdwg.org/plic/terms/ecologicalSignificanceUnstructured</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/ecologicalSignificanceUnstructured-2023-10-06">http://rs.tdwg.org/plic/terms/version/ecologicalSignificanceUnstructured-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Unstructured Ecological Significance</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Ecological Significance element in text block format.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/NaturalHistory/EcologicalSignificance/EcologicalSignificanceUnstructured</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>


### 4.16 Environmental Envelope

Set of environmental conditions within which it is believed that the species can persist; i.e. where its environmental requirements can be satisfied.<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_environmentalEnvelopeAtomized"></a>Term Name  plic:environmentalEnvelopeAtomized</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/environmentalEnvelopeAtomized">http://rs.tdwg.org/plic/terms/environmentalEnvelopeAtomized</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/environmentalEnvelopeAtomized-2023-10-06">http://rs.tdwg.org/plic/terms/version/environmentalEnvelopeAtomized-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Atomized Environmental Envelope</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Environmental envelope of a species expressed as an enumeration of measures and parameters.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/NaturalHistory/EnvironmentalEnvelope/EnvironmentalEnvelopeAtomized</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_environmentalEnvelopeUnstructured"></a>Term Name  plic:environmentalEnvelopeUnstructured</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/environmentalEnvelopeUnstructured">http://rs.tdwg.org/plic/terms/environmentalEnvelopeUnstructured</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/environmentalEnvelopeUnstructured-2023-10-06">http://rs.tdwg.org/plic/terms/version/environmentalEnvelopeUnstructured-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Unstructured Environmental Envelope</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>environmentalEnvelope as a text block.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/NaturalHistory/EnvironmentalEnvelope/EnvironmentalEnvelopeUnstructured</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>


### 4.17 Natural History

Relevant descriptive information about the species: Life Form, Life Cycle, Reproduction, Annual Cycles, Feeding, Dispersal, Behavior, Interactions, Molecular Data, Migratory, Ecological Significance, Miscellaneous Details, Environmental Envelope and Ancillary Data.
### 4.18 Invasiveness

Information about invasive exotic species that could threaten ecosystems, habitats and species<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_Route"></a>Term Name  plic:Route</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/Route">http://rs.tdwg.org/plic/terms/Route</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/Route-2023-10-06">http://rs.tdwg.org/plic/terms/version/Route-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Route</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>This is equivalent and probably replaceable by gisin:route.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/Invasiveness/InvasivenessAtomized/Route</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_WhatImpact"></a>Term Name  plic:WhatImpact</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/WhatImpact">http://rs.tdwg.org/plic/terms/WhatImpact</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/WhatImpact-2023-10-06">http://rs.tdwg.org/plic/terms/version/WhatImpact-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>What Impact</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>An indication of the actual impact as a free text string. e.g. destroys riparian vegetation, destroys irrigation systems, displaces Arvicola sapidus.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/Invasiveness/InvasivenessAtomized/WhatImpact</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_impactMechanism"></a>Term Name  plic:impactMechanism</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/impactMechanism">http://rs.tdwg.org/plic/terms/impactMechanism</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/impactMechanism-2023-10-06">http://rs.tdwg.org/plic/terms/version/impactMechanism-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Impact Mechanism</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Mechanism of introduction or impact to a new location.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/Invasiveness/InvasivenessAtomized/impactMechanism</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>http://www.w3.org/2004/02/skos/core#ConceptScheme</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_impactTarget"></a>Term Name  plic:impactTarget</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/impactTarget">http://rs.tdwg.org/plic/terms/impactTarget</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/impactTarget-2023-10-06">http://rs.tdwg.org/plic/terms/version/impactTarget-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Impact Target</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>This is equivalent and probably replaceable by gisin:impactTarget.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/Invasiveness/InvasivenessAtomized/impactTarget</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>http://www.w3.org/2004/02/skos/core#ConceptScheme</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_invasivenessUnstructured"></a>Term Name  plic:invasivenessUnstructured</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/invasivenessUnstructured">http://rs.tdwg.org/plic/terms/invasivenessUnstructured</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/invasivenessUnstructured-2023-10-06">http://rs.tdwg.org/plic/terms/version/invasivenessUnstructured-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Unstructured Invasiveness</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>invasiveness element in text block format.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/Invasiveness/InvasivenessUnstructured</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_vector"></a>Term Name  plic:vector</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/vector">http://rs.tdwg.org/plic/terms/vector</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/vector-2023-10-06">http://rs.tdwg.org/plic/terms/version/vector-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Vector</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>By which means a species occupies a new territory. e.g. fishing boats; dirty boots, cars (Aedes albopictus).</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/Invasiveness/InvasivenessAtomized/vector</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>


### 4.19 Habitat And Distribution

Habitat and Distribution of the species<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_DistributionScope"></a>Term Name  plic:DistributionScope</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/DistributionScope">http://rs.tdwg.org/plic/terms/DistributionScope</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/DistributionScope-2023-10-06">http://rs.tdwg.org/plic/terms/version/DistributionScope-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Distribution Scope</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>List of regions structured and categorized.</td>
		</tr>
		<tr>
			<td>Notes</td>
			<td>A controlled vocabulary is recommended. e.g. Historical, Current, Restricted and Wide. </td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/Legislation/LegislationAtomized/AppliesTo/DistributionScope<br/>/Dataset/TaxonRecord/DemographyAndThreat/ThreatStatus/ThreatStatusAtomized/AppliesTo/DistributionScope<br/>/Dataset/TaxonRecord/HabitatAndDistribution/Distribution/DistributionScope<br/>/Dataset/TaxonRecord/NomenclatureAndClassification/CommonNames/CommonNamesAtomized/UsedIn/DistributionScope</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_DistributionUnstructured"></a>Term Name  plic:DistributionUnstructured</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/DistributionUnstructured">http://rs.tdwg.org/plic/terms/DistributionUnstructured</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/DistributionUnstructured-2023-10-06">http://rs.tdwg.org/plic/terms/version/DistributionUnstructured-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Unstructured Distribution</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Distribution element in text block format.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/Legislation/LegislationAtomized/AppliesTo/DistributionUnstructured<br/>/Dataset/TaxonRecord/DemographyAndThreat/ThreatStatus/ThreatStatusAtomized/AppliesTo/DistributionUnstructured<br/>/Dataset/TaxonRecord/HabitatAndDistribution/Distribution/DistributionUnstructured<br/>/Dataset/TaxonRecord/NomenclatureAndClassification/CommonNames/CommonNamesAtomized/UsedIn/DistributionUnstructured</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_EndemicIn"></a>Term Name  plic:EndemicIn</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/EndemicIn">http://rs.tdwg.org/plic/terms/EndemicIn</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/EndemicIn-2023-10-06">http://rs.tdwg.org/plic/terms/version/EndemicIn-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Endemic In</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>The area that works as a context for specifying endemic areas of a species. A controlled vocabulary is recommended. The term may go from local to above-country levels.</td>
		</tr>
		<tr>
			<td>Notes</td>
			<td>If not specified, the Earth as a whole is assumed as the geographical context. Examples: Vicuña (Vicugna vicugna Molina, 1782) endemic to the Andean region **in South America**. Manzanilla Real (Artemisia granatensis Boiss.) endemic in the peaks of Sierra Nevada (**in Spain**).</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/HabitatAndDistribution/Endemic/EndemicAtomized/EndemicIn</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_EndemicTo"></a>Term Name  plic:EndemicTo</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/EndemicTo">http://rs.tdwg.org/plic/terms/EndemicTo</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/EndemicTo-2023-10-06">http://rs.tdwg.org/plic/terms/version/EndemicTo-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Endemic To</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>A territory in which an endemic species appear. A controlled vocabulary is recommended. The term may go from local to above-country levels.</td>
		</tr>
		<tr>
			<td>Notes</td>
			<td>Examples: Giant panda (Ailuropoda melanoleuca (David, 1869) endemic to China. Quetzal Resplendent (Pharomachrus mocinno de la Llave, 1832) endemic to Mexico, Guatemala, Honduras, El Salvador, Nicaragua, Costa Rica and Panama.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/HabitatAndDistribution/Endemic/EndemicAtomized/EndemicTo</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_GeographicEntity"></a>Term Name  plic:GeographicEntity</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/GeographicEntity">http://rs.tdwg.org/plic/terms/GeographicEntity</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/GeographicEntity-2023-10-06">http://rs.tdwg.org/plic/terms/version/GeographicEntity-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Geographic Entity</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Name of the geographic entity. </td>
		</tr>
		<tr>
			<td>Notes</td>
			<td>A controlled vocabulary --as specified in the Catalogue element-- is recommended. e.g. Spain; Aguascalientas; Alabama; Ambon</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/Legislation/LegislationAtomized/AppliesTo/Distribution/DistributionAtomized/GeographicEntity<br/>/Dataset/TaxonRecord/DemographyAndThreat/ThreatStatus/ThreatStatusAtomized/AppliesTo/Distribution/DistributionAtomized/GeographicEntity<br/>/Dataset/TaxonRecord/NomenclatureAndClassification/CommonNames/CommonNamesAtomized/UsedIn/DistributionAtomized/GeographicEntity<br/>/Dataset/TaxonRecord/HabitatAndDistribution/Distribution/DistributionAtomized/GeographicEntity</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>http://www.w3.org/1999/02/22-rdf-syntax-ns#Property </td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_endemicUnstructured"></a>Term Name  plic:endemicUnstructured</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/endemicUnstructured">http://rs.tdwg.org/plic/terms/endemicUnstructured</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/endemicUnstructured-2023-10-06">http://rs.tdwg.org/plic/terms/version/endemicUnstructured-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Unstructured Endemic</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Information on the endemicity of a species as a text block.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/HabitatAndDistribution/Endemic/EndemicUnstructured</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_habitatAndDistributionUnstructured"></a>Term Name  plic:habitatAndDistributionUnstructured</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/habitatAndDistributionUnstructured">http://rs.tdwg.org/plic/terms/habitatAndDistributionUnstructured</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/habitatAndDistributionUnstructured-2023-10-06">http://rs.tdwg.org/plic/terms/version/habitatAndDistributionUnstructured-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Unstructured Habitat And Distribution</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>habitatAndDistribution element in text block format.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/HabitatAndDistribution/HabitatAndDistributionUnstructured</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_habitatAtomized"></a>Term Name  plic:habitatAtomized</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/habitatAtomized">http://rs.tdwg.org/plic/terms/habitatAtomized</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/habitatAtomized-2023-10-06">http://rs.tdwg.org/plic/terms/version/habitatAtomized-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Atomized Habitat</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>habitatAndDistribution element in structured format.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/HabitatAndDistribution/Habitats/HabitatAtomized</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_habitatUnstructured"></a>Term Name  plic:habitatUnstructured</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/habitatUnstructured">http://rs.tdwg.org/plic/terms/habitatUnstructured</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/habitatUnstructured-2023-10-06">http://rs.tdwg.org/plic/terms/version/habitatUnstructured-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Unstructured Habitat</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>habitat element in text block format.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/HabitatAndDistribution/Habitats/HabitatUnstructured</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>


### 4.20 Demography And Threat

Information concerning the demographic aspects of the species: Territory, Population Biology, Threat Status, Direct Threats, Legislation and Ancillary Data<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_AbundanceData"></a>Term Name  plic:AbundanceData</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/AbundanceData">http://rs.tdwg.org/plic/terms/AbundanceData</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/AbundanceData-2023-10-06">http://rs.tdwg.org/plic/terms/version/AbundanceData-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>AbundanceData</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>The relative representation of a species population in relation to other species or multiple species in a particular territory.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/AbundanceData</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_AreaOfOccupancy"></a>Term Name  plic:AreaOfOccupancy</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/AreaOfOccupancy">http://rs.tdwg.org/plic/terms/AreaOfOccupancy</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/AreaOfOccupancy-2023-10-06">http://rs.tdwg.org/plic/terms/version/AreaOfOccupancy-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Area of occupancy</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Area within its 'extent of occurrence' (see EOO) which is occupied by a taxon, excluding cases of vagrancy. The measure reflects the fact that a taxon will not usually occur throughout the area of its extent of occurrence, which may contain unsuitable or unoccupied habitats.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/Territory/TerritoryAtomized/AreaOfOccupancy</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_AverageDensity"></a>Term Name  plic:AverageDensity</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/AverageDensity">http://rs.tdwg.org/plic/terms/AverageDensity</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/AverageDensity-2023-10-06">http://rs.tdwg.org/plic/terms/version/AverageDensity-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Average density</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Average of the densities obtained for a population.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/AverageDensity</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_BirthRate"></a>Term Name  plic:BirthRate</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/BirthRate">http://rs.tdwg.org/plic/terms/BirthRate</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/BirthRate-2023-10-06">http://rs.tdwg.org/plic/terms/version/BirthRate-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Birth rate</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Ratio of births to the total number of individuals in a population in a time period.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/BirthRate</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_CarryingCapacity"></a>Term Name  plic:CarryingCapacity</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/CarryingCapacity">http://rs.tdwg.org/plic/terms/CarryingCapacity</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/CarryingCapacity-2023-10-06">http://rs.tdwg.org/plic/terms/version/CarryingCapacity-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Carrying capacity</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Maximum population density possible as limited by the resources available for the population in the absence of predators and parasites.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/CarryingCapacity</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_DensityData"></a>Term Name  plic:DensityData</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/DensityData">http://rs.tdwg.org/plic/terms/DensityData</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/DensityData-2023-10-06">http://rs.tdwg.org/plic/terms/version/DensityData-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>DensityData</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Population size in relation to a defined space unit.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/DensityData</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_DescriptionLifeStages"></a>Term Name  plic:DescriptionLifeStages</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/DescriptionLifeStages">http://rs.tdwg.org/plic/terms/DescriptionLifeStages</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/DescriptionLifeStages-2023-10-06">http://rs.tdwg.org/plic/terms/version/DescriptionLifeStages-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Description life stages</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Sex/age categories or life stages of a species; can be size in the case of plants.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/DescriptionLifeStages</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_DirectThreatAtomized"></a>Term Name  plic:DirectThreatAtomized</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/DirectThreatAtomized">http://rs.tdwg.org/plic/terms/DirectThreatAtomized</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/DirectThreatAtomized-2023-10-06">http://rs.tdwg.org/plic/terms/version/DirectThreatAtomized-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Atomized Direct Threat</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>directThreats element in structured format. </td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/DirectThreats/DirectThreatAtomized</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_Emigration"></a>Term Name  plic:Emigration</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/Emigration">http://rs.tdwg.org/plic/terms/Emigration</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/Emigration-2023-10-06">http://rs.tdwg.org/plic/terms/version/Emigration-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Emigration</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Information on individuals leaving a population.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/Emigration</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_ExtentOfOccurrence"></a>Term Name  plic:ExtentOfOccurrence</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/ExtentOfOccurrence">http://rs.tdwg.org/plic/terms/ExtentOfOccurrence</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/ExtentOfOccurrence-2023-10-06">http://rs.tdwg.org/plic/terms/version/ExtentOfOccurrence-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Extent of occurrence</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Area contained within the shortest continuous imaginary boundary which can be drawn to encompass all the known, inferred or projected sites of present occurrence of a taxon, excluding cases of vagrancy.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/Territory/TerritoryAtomized/ExtentOfOccurrence</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_Fecundity"></a>Term Name  plic:Fecundity</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/Fecundity">http://rs.tdwg.org/plic/terms/Fecundity</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/Fecundity-2023-10-06">http://rs.tdwg.org/plic/terms/version/Fecundity-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Fecundity</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>In the context of a population, is the combined maximum potential of its individuals to produce offspring.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/Fecundity</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_Immigration"></a>Term Name  plic:Immigration</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/Immigration">http://rs.tdwg.org/plic/terms/Immigration</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/Immigration-2023-10-06">http://rs.tdwg.org/plic/terms/version/Immigration-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Immigration</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Information on individuals entering a population.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/Immigration</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_LegislationName"></a>Term Name  plic:LegislationName</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/LegislationName">http://rs.tdwg.org/plic/terms/LegislationName</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/LegislationName-2023-10-06">http://rs.tdwg.org/plic/terms/version/LegislationName-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Legislation Name</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Word or phrase to designate the law or group of laws.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/Legislation/LegislationAtomized/LegislationName</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_LegislationRead"></a>Term Name  plic:LegislationRead</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/LegislationRead">http://rs.tdwg.org/plic/terms/LegislationRead</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/LegislationRead-2023-10-06">http://rs.tdwg.org/plic/terms/version/LegislationRead-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Legislation Read</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>The oficial document in which the user can read the legislation.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/Legislation/LegislationAtomized/LegislationRead</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_MortalityRate"></a>Term Name  plic:MortalityRate</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/MortalityRate">http://rs.tdwg.org/plic/terms/MortalityRate</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/MortalityRate-2023-10-06">http://rs.tdwg.org/plic/terms/version/MortalityRate-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Mortality rate</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Probability of dying; the ratio between the number of deaths in a given time interval to the number of subjects alive at the start of this interval.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/MortalityRate</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_NumberIndividualsPerObservation"></a>Term Name  plic:NumberIndividualsPerObservation</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/NumberIndividualsPerObservation">http://rs.tdwg.org/plic/terms/NumberIndividualsPerObservation</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/NumberIndividualsPerObservation-2023-10-06">http://rs.tdwg.org/plic/terms/version/NumberIndividualsPerObservation-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Number individuals per observation</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Mean number of individuals per observation event or unit.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/NumberIndividualsPerObservation</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_PatternDistribution"></a>Term Name  plic:PatternDistribution</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/PatternDistribution">http://rs.tdwg.org/plic/terms/PatternDistribution</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/PatternDistribution-2023-10-06">http://rs.tdwg.org/plic/terms/version/PatternDistribution-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Pattern distribution</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>The spatial arrangement of the individuals of a population in the territory it occupies.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/PatternDistribution</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_PopulationGrowthRate"></a>Term Name  plic:PopulationGrowthRate</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/PopulationGrowthRate">http://rs.tdwg.org/plic/terms/PopulationGrowthRate</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/PopulationGrowthRate-2023-10-06">http://rs.tdwg.org/plic/terms/version/PopulationGrowthRate-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Population growth rate</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Growth rate of a population in a given time period, based on births, deaths, emigration and immigration.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/PopulationGrowthRate</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_PopulationTrend"></a>Term Name  plic:PopulationTrend</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/PopulationTrend">http://rs.tdwg.org/plic/terms/PopulationTrend</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/PopulationTrend-2023-10-06">http://rs.tdwg.org/plic/terms/version/PopulationTrend-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Population trend</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Changes of a population over time and can include changes in distribution, biogeography (e.g., size of population), life-history (e.g., birth and death rates), etc.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/PopulationTrend</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_ProportionIndividualsPerStageLife"></a>Term Name  plic:ProportionIndividualsPerStageLife</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/ProportionIndividualsPerStageLife">http://rs.tdwg.org/plic/terms/ProportionIndividualsPerStageLife</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/ProportionIndividualsPerStageLife-2023-10-06">http://rs.tdwg.org/plic/terms/version/ProportionIndividualsPerStageLife-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>ProportionIndividuals per stage life</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Percentage of individuals that belong to each life stage in a population.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/ProportionIndividualsPerStageLife</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_ProtectionLegalStatus"></a>Term Name  plic:ProtectionLegalStatus</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/ProtectionLegalStatus">http://rs.tdwg.org/plic/terms/ProtectionLegalStatus</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/ProtectionLegalStatus-2023-10-06">http://rs.tdwg.org/plic/terms/version/ProtectionLegalStatus-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Protection Legal Status</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Description of the legal status.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/Legislation/LegislationAtomized/ProtectionLegalStatus</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_Recruitment"></a>Term Name  plic:Recruitment</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/Recruitment">http://rs.tdwg.org/plic/terms/Recruitment</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/Recruitment-2023-10-06">http://rs.tdwg.org/plic/terms/version/Recruitment-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Recruitment</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Information on the process by which young individuals (e.g., seedlings, larvae, propagules) become part of the adult population. It can be rate, scale, a description, etc.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/Recruitment</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_SexRatio"></a>Term Name  plic:SexRatio</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/SexRatio">http://rs.tdwg.org/plic/terms/SexRatio</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/SexRatio-2023-10-06">http://rs.tdwg.org/plic/terms/version/SexRatio-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>SexRatio</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Relative number of males to females in a population.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/SexRatio</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_Size"></a>Term Name  plic:Size</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/Size">http://rs.tdwg.org/plic/terms/Size</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/Size-2023-10-06">http://rs.tdwg.org/plic/terms/version/Size-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Size</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Number of individual organisms in a population.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/PopulationBiology/PopulationBiologyAtomized/Size</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_demographyAndThreatUnstructured"></a>Term Name  plic:demographyAndThreatUnstructured</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/demographyAndThreatUnstructured">http://rs.tdwg.org/plic/terms/demographyAndThreatUnstructured</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/demographyAndThreatUnstructured-2023-10-06">http://rs.tdwg.org/plic/terms/version/demographyAndThreatUnstructured-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Unstructured Demography And Threat</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>demographyAndThreat element in unstructured format. </td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/DemographyAndThreatUnstructured</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_legalNorm"></a>Term Name  plic:legalNorm</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/legalNorm">http://rs.tdwg.org/plic/terms/legalNorm</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/legalNorm-2023-10-06">http://rs.tdwg.org/plic/terms/version/legalNorm-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Legal Norm</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Norms are general legal principles that are widely accepted. This acceptance is evidenced in a number of ways, such as international agreements, national legislation, domestic and international judicial decisions, and scholarly writings.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/Legislation/LegislationAtomized/LegalNorm</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_legislationStatus"></a>Term Name  plic:legislationStatus</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/legislationStatus">http://rs.tdwg.org/plic/terms/legislationStatus</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/legislationStatus-2023-10-06">http://rs.tdwg.org/plic/terms/version/legislationStatus-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Legislation Status</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Whether a piece of legislation is in force, or superseded, etc.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/Legislation/LegislationAtomized/LegislationStatus</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_legislationType"></a>Term Name  plic:legislationType</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/legislationType">http://rs.tdwg.org/plic/terms/legislationType</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/legislationType-2023-10-06">http://rs.tdwg.org/plic/terms/version/legislationType-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Legislation Type</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Category of the piece of legislation.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/Legislation/LegislationAtomized/LegislationType</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_legislationUnstructured"></a>Term Name  plic:legislationUnstructured</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/legislationUnstructured">http://rs.tdwg.org/plic/terms/legislationUnstructured</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/legislationUnstructured-2023-10-06">http://rs.tdwg.org/plic/terms/version/legislationUnstructured-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Unstructured Legislation</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>legislation element in text block format.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/DemographyAndThreat/Legislation/LegislationUnstructured</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>


### 4.21 Uses Management And Conservation

Uses: Ways in which species are utilized by people, including Folklore. Management: actions aimed at conserving or recovering species. Conservation status<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_Actions"></a>Term Name  plic:Actions</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/Actions">http://rs.tdwg.org/plic/terms/Actions</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/Actions-2023-10-06">http://rs.tdwg.org/plic/terms/version/Actions-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Actions</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Individual tasks in which a management project can be atomized. Each action must be separated by ;</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/UsesManagementAndConservation/ManagementAndConservation/ManagementAndConservationAtomized/Actions</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_ActionsType"></a>Term Name  plic:ActionsType</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/ActionsType">http://rs.tdwg.org/plic/terms/ActionsType</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/ActionsType-2023-10-06">http://rs.tdwg.org/plic/terms/version/ActionsType-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Actions Type</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Each action must have one type. In the case that one action doesn't have type then put blank.</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_Conservation-ExplotationData"></a>Term Name  plic:Conservation-ExplotationData</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/Conservation-ExplotationData">http://rs.tdwg.org/plic/terms/Conservation-ExplotationData</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/Conservation-ExplotationData-2023-10-06">http://rs.tdwg.org/plic/terms/version/Conservation-ExplotationData-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Conservation-Explotation Data</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Acc. TDWG Economic Botany. Frequency record of plants, details of regeneration, sustainability or over-exploitation and any locally imposed bans on felling or harvesting.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/UsesManagementAndConservation/Uses/UsesAtomized/Conservation-ExplotationData</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_Economics"></a>Term Name  plic:Economics</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/Economics">http://rs.tdwg.org/plic/terms/Economics</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/Economics-2023-10-06">http://rs.tdwg.org/plic/terms/version/Economics-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Economics</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Acc. TDWG Economic Botany. Real or potential existence of trade in live plants, plant parts or derivatives and, if so, the trade scale.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/UsesManagementAndConservation/Uses/UsesAtomized/Economics</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_HumanAndEnvironmentalrelevance"></a>Term Name  plic:HumanAndEnvironmentalrelevance</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/HumanAndEnvironmentalrelevance">http://rs.tdwg.org/plic/terms/HumanAndEnvironmentalrelevance</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/HumanAndEnvironmentalrelevance-2023-10-06">http://rs.tdwg.org/plic/terms/version/HumanAndEnvironmentalrelevance-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Human and Environmental Relevance</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Impact or value an species has either on the environment or on humans, and that justify management measures.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/UsesManagementAndConservation/ManagementAndConservation/ManagementAndConservationAtomized/HumanAndEnvironmentalRelevance</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_ManagementPlan"></a>Term Name  plic:ManagementPlan</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/ManagementPlan">http://rs.tdwg.org/plic/terms/ManagementPlan</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/ManagementPlan-2023-10-06">http://rs.tdwg.org/plic/terms/version/ManagementPlan-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Management Plan</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>plan guiding the overall management project.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/UsesManagementAndConservation/ManagementAndConservation/ManagementAndConservationAtomized/ManagementPlan</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_MeansOfApplication-Administration"></a>Term Name  plic:MeansOfApplication-Administration</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/MeansOfApplication-Administration">http://rs.tdwg.org/plic/terms/MeansOfApplication-Administration</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/MeansOfApplication-Administration-2023-10-06">http://rs.tdwg.org/plic/terms/version/MeansOfApplication-Administration-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Means of Application-Administration</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Acc. TDWG Economic Botany. This is specific relevant for medicines, poisons .</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/UsesManagementAndConservation/Uses/UsesAtomized/MeansOfApplication-Administration</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_Objectives"></a>Term Name  plic:Objectives</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/Objectives">http://rs.tdwg.org/plic/terms/Objectives</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/Objectives-2023-10-06">http://rs.tdwg.org/plic/terms/version/Objectives-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Objectives</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Specific purposes of the management actions. Each objective must be separated by ;</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/UsesManagementAndConservation/ManagementAndConservation/ManagementAndConservationAtomized/Objectives</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_Organisms"></a>Term Name  plic:Organisms</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/Organisms">http://rs.tdwg.org/plic/terms/Organisms</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/Organisms-2023-10-06">http://rs.tdwg.org/plic/terms/version/Organisms-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Organisms</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Acc. TDWG Economic Botany. Organisms which use the plant/plant parts.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/UsesManagementAndConservation/Uses/UsesAtomized/Organisms</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_PartUsed"></a>Term Name  plic:PartUsed</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/PartUsed">http://rs.tdwg.org/plic/terms/PartUsed</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/PartUsed-2023-10-06">http://rs.tdwg.org/plic/terms/version/PartUsed-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Part Used</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Acc. TDWG Economic Botany. Which plant parts are used, or have any negative values.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/UsesManagementAndConservation/Uses/UsesAtomized/PartUsed</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_Potential"></a>Term Name  plic:Potential</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/Potential">http://rs.tdwg.org/plic/terms/Potential</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/Potential-2023-10-06">http://rs.tdwg.org/plic/terms/version/Potential-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Potential</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Acc. TDWG Economic Botany. Could the use, cultivation, manufacture of products etc. be increased and /or introduced to other areas or social groups?</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/UsesManagementAndConservation/Uses/UsesAtomized/Potential</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_ProductionDetails"></a>Term Name  plic:ProductionDetails</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/ProductionDetails">http://rs.tdwg.org/plic/terms/ProductionDetails</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/ProductionDetails-2023-10-06">http://rs.tdwg.org/plic/terms/version/ProductionDetails-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Production Details</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Definition: Acc. TDWG Economic Botany. (where relevant). Give details of protection, cultivation, harvesting, yields, processing and storage methods used and take note of special tools, timing etc.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/UsesManagementAndConservation/Uses/UsesAtomized/ProductionDetails</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_Properties"></a>Term Name  plic:Properties</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/Properties">http://rs.tdwg.org/plic/terms/Properties</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/Properties-2023-10-06">http://rs.tdwg.org/plic/terms/version/Properties-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Properties</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Acc. TDWG Economic Botany. Details of properties which influence its value for a specified purpose.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/UsesManagementAndConservation/Uses/UsesAtomized/Properties</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_RatingPopularity"></a>Term Name  plic:RatingPopularity</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/RatingPopularity">http://rs.tdwg.org/plic/terms/RatingPopularity</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/RatingPopularity-2023-10-06">http://rs.tdwg.org/plic/terms/version/RatingPopularity-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Rating Popularity</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Acc. TDWG Economic Botany. Assessment of the plant for its use and possible preference to other species, pointing out, in this case, which species are they.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/UsesManagementAndConservation/Uses/UsesAtomized/RatingPopularity</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_SeasonOfAvailability-Use"></a>Term Name  plic:SeasonOfAvailability-Use</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/SeasonOfAvailability-Use">http://rs.tdwg.org/plic/terms/SeasonOfAvailability-Use</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/SeasonOfAvailability-Use-2023-10-06">http://rs.tdwg.org/plic/terms/version/SeasonOfAvailability-Use-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Season of Availability-Use</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Acc. TDWG Economic Botany. The season in which the plant is available/is used and, if relevant, the time of day.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/UsesManagementAndConservation/Uses/UsesAtomized/SeasonOfAvailability-Use</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_Use-Value"></a>Term Name  plic:Use-Value</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/Use-Value">http://rs.tdwg.org/plic/terms/Use-Value</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/Use-Value-2023-10-06">http://rs.tdwg.org/plic/terms/version/Use-Value-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Use-Value</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>What is the plant used for, or what negative values does it have.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/UsesManagementAndConservation/Uses/UsesAtomized/Use-Value</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_UseNotes"></a>Term Name  plic:UseNotes</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/UseNotes">http://rs.tdwg.org/plic/terms/UseNotes</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/UseNotes-2023-10-06">http://rs.tdwg.org/plic/terms/version/UseNotes-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Use Notes</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Notes about how species are utilized by people.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/UsesManagementAndConservation/Uses/UsesAtomized/UseNotes</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_UseType"></a>Term Name  plic:UseType</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/UseType">http://rs.tdwg.org/plic/terms/UseType</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/UseType-2023-10-06">http://rs.tdwg.org/plic/terms/version/UseType-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Use Type</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Acc. TDWG Economic Botany. Type of use: traditional, modern, industrial or just a possible use.</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_Users"></a>Term Name  plic:Users</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/Users">http://rs.tdwg.org/plic/terms/Users</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/Users-2023-10-06">http://rs.tdwg.org/plic/terms/version/Users-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Users</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Acc. TDWG Economic Botany. The user group who recognizes the value and/or use of the plant.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/UsesManagementAndConservation/Uses/UsesAtomized/Users</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_UsesManagementAndConservationUnstructured"></a>Term Name  plic:UsesManagementAndConservationUnstructured</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/UsesManagementAndConservationUnstructured">http://rs.tdwg.org/plic/terms/UsesManagementAndConservationUnstructured</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/UsesManagementAndConservationUnstructured-2023-10-06">http://rs.tdwg.org/plic/terms/version/UsesManagementAndConservationUnstructured-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Uses Management and Conservation Unstructured </td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>UsesManagementAndConservation element in text block format.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/UsesManagementAndConservation/UsesManagementAndConservationUnstructured</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_UsesUnstructured"></a>Term Name  plic:UsesUnstructured</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/UsesUnstructured">http://rs.tdwg.org/plic/terms/UsesUnstructured</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/UsesUnstructured-2023-10-06">http://rs.tdwg.org/plic/terms/version/UsesUnstructured-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Unstructured Uses</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Uses in a unstructured format.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/UsesManagementAndConservation/Uses/UsesUnstructured</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="2"><a id="plic_VernacularNameUseAnnotations"></a>Term Name  plic:VernacularNameUseAnnotations</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/VernacularNameUseAnnotations">http://rs.tdwg.org/plic/terms/VernacularNameUseAnnotations</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2023-10-06</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/plic/terms/version/VernacularNameUseAnnotations-2023-10-06">http://rs.tdwg.org/plic/terms/version/VernacularNameUseAnnotations-2023-10-06</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Vernacular Name Use Annotations</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>Acc. TDWG Economic Botany. The name of the taxon must be distinguished from the name of the plant parts, the names of any processing stages, and the final product name. Names used in trade should be identified. It should also be mentioned if any vernacular name refers to more than one taxon. The use of some names may be restricted to a time of year or occasion, or have sacred connotations. The language or dialect to which the names belong should be stated along with details of the ethnic group. Care should be taken with transliteration into the Roman alphabet; if a standard system exists, use it and note which one it is.</td>
		</tr>
		<tr>
			<td>Equivalent XPath</td>
			<td>/Dataset/TaxonRecord/UsesManagementAndConservation/Uses/UsesAtomized/VernacularNameUseAnnotations</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
	</tbody>
</table>


### 4.22 Associated Party

A party associated with the resource. Parties have particular role. (EML-RESOURCE)
### 4.23 Ancillary Data

The AncillaryData element contains information that could be an image, an audio, a list of references, a list of agents, rights, licenses...related with the element it belongs. Its definition is borrowed from the dataObjectBaseType element of the EOL scheme.
