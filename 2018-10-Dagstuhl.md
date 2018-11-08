# Interoperability of Metadata Standards in Cross-Domain Science, Health, and Social Science Applications

This is a report on the workshop on [Interoperability of Metadata Standards in Cross-Domain Science, Health, and Social Science Applications][1], held at **Schloss Dagstuhl** – Leibniz Center for Informatics, in Wadern, Saarland, Germany during 1-5 October 2018. The workshop was sponsored by the DDI Alliance, CODATA and Dagstuhl. I attended as part of the CODATA Commission for Standards project R-11749. The [official organizer’s report][2] is available from CODATA.

> _Note: In common with most technical work, there are a lot of acronyms, here exacerbated by the fact that the meeting brought together a highly cross-disciplinary group. The details of most of them are not important and are provided for reference only. The few that do matter are spelled out. In fact an [Acronym-buster][3] is available as one of the workshop outputs._

The workshop was conceived by Joachim Wackerow (GESIS-Leibniz Center, DDI Alliance) and me (CSIRO, W3C), and we were joined by Simon Hodson (CODATA) and Steve McEachern (ANU, DDI-Alliance) on the organizing team. It was positioned as the 12th member of a [series of annual workshops on DDI][4]. There were [24 participants][5].

## Workshop goals

The goal of the workshop was to examine opportunities for [alignment of (meta)data standards from a range of disciplines and application areas][6], ranging from social science and official statistics (DDI, SDMX), public health and clinical trials (FHIR, CDISC, DATS), ecology and environmental sciences (EML, ISO 19115), and some general purpose vocabularies (CERIF, DCAT, schema.org). To give a user-centric frame for the discussion, [three pilot projects from the CODATA Data Integration Initiative][7] provided requirements related to multi-disciplinary datasets concerning
1.	Infectious disease outbreaks (IDDO)
2.	Resilient cities and regions
3.	Disaster risk reduction (Sendai framework)
From a technical design point of view, these pilots provide archetypal scenarios requiring discovery and accessing datasets from a variety of sources across a spectrum of disciplines and domains.

## Metadata

Metadata about datasets is used to support a variety of functions in a research workflow, particularly discovery, assessment/selection, access, transformation. Metadata may also relate to attribution and data management. Cross-disciplinary indexes like [CSIRO’s Data Access Portal (DAP)][8], [Research Data Australia (RDA)][9], and Google’s recently announced [Dataset Search][10] use metadata to support discovery and some assessment/selection actions. There are also many more specialized indexes serving specific communities, such as remote sensing, clinical trials, energy use. Extracts from the specialist indexes may be harvested into the general purpose indexes, but there is some loss of precision as specialized aspects are dropped.

The hypothesis of the workshop is that
(a)	specialized, domain-specific repositories and indexes are key sources of data for the cross-disciplinary applications
(b)	it is difficult to search for datasets across discipline boundaries, because
-	the specialized data may not be listed in the general-purpose indexes,
-	even if they are, the information required to achieve accurate discovery and selection is not included in the general-purpose indexes
(c)	small enhancements to the general-purpose indexes can provide significant improvements in search and assessment functionality, and allow some specialist information to be represented, before a hand-off to specialist indexes.
A particular issue is the need to supplement general, study-level descriptions with more specific, variable-level information and summary statistics.

A platform for this is the [W3C DCAT (Dataset Catalogue) vocabulary][11].  DCAT is in [widespread use in Europe][12], is harvested by the [Google Dataset Search index][13], and is gaining momentum as a lingua-franca for data catalogs (e.g. CKAN, used in many data.gov initiatives, has a [standard DCAT interface][14]).

## Workshop structure
The first day of the workshop saw a series of introductions, first to the pilot scenarios, then to the various metadata standards, which produced an assessment of their scope.

The rest of the week saw the participants split into 4 or 5 work-groups: one for each of the three pilots, one to look at [enhancing DCAT for research data][15], which merged with a group looking at the details of variable definition.

The outlines of 5 papers were prepared during the workshop, and the outcomes will be presented at the upcoming [SciDataCon 2018][16].

## Relevance to CSIRO
Of particular interest for CSIRO are the following outcomes of the workshop:
### 1.	Enhancements to data search and sharing –

The current enhancements to DCAT [11] have been guided in part by the requirements of Research Data Australia (RDA) – a service provided by ANDS (now the Australian Research Data Commons – ARDC). The extensions for research data proposed as an outcome of the workshop [15] take DCAT even further into the research data world. ARDC was represented at the workshop by Dr Adrian Burton. We have been working with Adrian on plans for enhancing Research Data RDA. The intention is now to add DCAT support to RDA. Initially this will be alongside the current interface (which uses a local metadata standard called RIF-CS), but in due course is likely to replace it, providing a richer, standards-conformant API to the main Australian research data index. A reduced focus on RIF-CS from RDA would also lead to CSIRO’s DAP following a similar course.

### 2.	Better indexing of CSIRO outputs –

Google is harvesting dataset descriptions from RDA and DAP, so CSIRO’s data are now visible in the biggest global index. However, the precision of that index is compromised by the relatively shallow metadata provided for datasets, and in turn the relatively few tags that Google chooses to index. Google uses both DCAT and its own (schema.org) metadata tags (some of which were cloned from an early version of DCAT anyway). So designing an enhanced metadata set built on a base of schema.org and DCAT [15], and then getting the records exposed through RDA and DAP to use these, is a likely way to see enhanced descriptions of CSIRO data in the global indexes, and thus better exposure of CSIRO products.

### 3.	Opportunities for engagement with international cross-disciplinary projects –

The three CODATA pilots [7] are exemplars of cross-disciplinary applications. As Australia’s leading cross-disciplinary research organization, CSIRO is well placed to engage. In particular, the Resilient Cities project appears to correlate well with the recently announced DD project on Cities/Energy (I’ve already contacted the leads). I’m less familiar with CSIRO’s work in health, but there is likely to be an overlap with the IDDO project.

### 4.	Continued global leadership of international research data platforms by CSIRO –

CSIRO has had a longstanding engagement with information standardization initiatives, both generic and domain specific. We were the host for the Australian W3C office for about 10 years, and CSIRO officers have held leadership positions in the Dublin Core Metadata Initiative, the Open Geospatial Consortium, and various ISO committees. I am currently on the Steering Committee for the CODATA Data Integration Initiative and also on the Vocabularies and Standards working group. This workshop saw a new liaison with an important data community – official statistics and social sciences. Our engagement in leading this reinforces our global leadership role.


<!-- Footnotes and links-->
[1]: https://ddi-alliance.atlassian.net/wiki/spaces/DDI4/pages/433553433/Interoperability+of+Metadata+Standards+in+Cross-Domain+Science+Health+and+Social+Science+Applications
[2]: http://www.codata.org/news/289/62/Workshop-Report-Interoperability-of-Metadata-Standards-in-Cross-Domain-Science-Health-and-Social-Science-Applications
[3]: https://ddi-alliance.atlassian.net/wiki/spaces/DDI4/pages/578650215/Acronym-buster
[4]: https://www.dagstuhl.de/en/program/calendar/evhp/?semnr=18403
[5]: https://ddi-alliance.atlassian.net/wiki/download/attachments/433553433/DagstuhlEvent18403_Participants.pdf
[6]: https://ddi-alliance.atlassian.net/wiki/spaces/DDI4/pages/535494691/Background+Materials+for+Use+in+Workshop
[7]: https://ddi-alliance.atlassian.net/wiki/spaces/DDI4/pages/535363641/Pilot+Projects
[8]: https://data.csiro.au/dap/
[9]: https://researchdata.ands.org.au/
[10]: https://toolbox.google.com/datasetsearch
[11]: https://w3c.github.io/dxwg/dcat/#changes
[12]: https://ec.europa.eu/isa2/solutions/dcat-application-profile-data-portals-europe_en
[13]: https://toolbox.google.com/datasetsearch
[14]: https://github.com/ckan/ckanext-dcat
[15]: https://github.com/w3c/dxwg/wiki/Data-aspects-semantics
[16]: https://www.scidatacon.org/IDW2018/sessions/232/
