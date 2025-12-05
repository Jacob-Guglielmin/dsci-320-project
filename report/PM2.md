# Project Milestone 2 Report

## Introduction

The Varieties of Democracy (V-Dem) Project is a global project working to collect comprehensive and high-quality data to study democracy and democratization of polities. The project is managed by 5 principle investigators but includes 23 project managers, 33 regional managers, 134 country coordinators, and more than 4200 country experts, which makes it one of the largest social science data collection projects on democracy. The main objective of this data collection project is to equip researchers with data that enables them to better study why some countries become and remain democratic, while others do not.

The name, Varieties of Democracy, reflects how this project approaches democracy as a complex and multifaceted concept beyond being a system of rule characterized by the simple presence of election.This comprehensive approach is systematised into five high-level indices of democracy, each representing one core principle of democracy: electoral, liberal, participatory, deliberative, and egalitarian democracy. Each core principle is broken down to its constituent components, called mid-level indices, which again are disaggregated into specific low-level indicators.

A special feature of the V-Dem Database is that it measures 600+ low-level indicators annually from 1789 for all countries of the world, which makes it possible to study the complexity of democratization on a global level, throughout the last two centuries. For the purpose of our project, we have chosen to study a subset of the columns available in the full dataset (while ensuring that the selected columns still meet the count and type requirements), as detailed below.

Our research team, Plot Twist, consists of three members: Jennifer Payne, Jacob Guglielmin and Sidsel Birkmose. Jennifer is interested in the different aspects of democracy, Jacob is interested in episodes of democratic change, and Sidsel is interested in geographical aspects of democracy.

Our intended audience is broad; it might include fellow students and curious members of the public, alongside more specialist viewers like policy-makers or researchers. We expect they might be able to answer some of our analytic questions, after viewing our representations. 

## Data Abstraction

| Attribute Name | Attribute Type | Data Semantics | Cardinality |
| --- | --- | --- | --- |
| country_name | Nominal | Country name | 202 unique values |
| year | Temporal | Year | 236 unique values |
| v2x_polyarchy | Quantitative (interval, continuous) | Electoral democracy index: represents the extent to which the ideal of electoral democracy is achieved, i.e. the core idea of free and fair electoral competition. | [0, 1] |
| v2x_libdem | Quantitative (interval, continuous) | Liberal democracy index: represents the extent to which the ideal of liberal democracy is achieved. The core idea being protecting individual and minority rights against tyranny. | [0, 1] |
| v2x_partipdem | Quantitative (interval, continuous) | Participatory democracy index: represents the extent to which the ideal of participatory democracy is achieved. The core idea being direct citizen participation in democracy: NGOs, referendums, local elections etc.. | [0, 1] |
| v2x_delibdem | Quantitative (interval, continuous) | Deliberative democracy index: represents the extent to which the ideal of deliberative democracy is achieved. The core idea being political decisions being made after public reasoning about the common good. | [0, 1] |
| v2x_egaldem | Quantitative (interval, continuous) | Egalitarian democracy index: represents the core idea of all social groups enjoying equal access to rights/resources/power. | [0, 1] |
| v2x_api | Quantitative (interval, continuous) | Additive polyarchy index: represents the extent to which the electoral principle of democracy achieved | [0, 1] |
| v2x_mpi | Quantitative (interval, continuous) | Multiplicative polyarchy index: represents the extent the electoral principle of democracy is achieved. | [0, 1] |
| v2x_freexp_altinf | Quantitative (interval, continuous) | Freedom of Expression and Alternative Sources of Information index: describes the extent to which government respect press and media freedom, the freedom of ordinary people to discuss political matters at home and in the public sphere, as well as the freedom of academic and cultural expression. | [0, 1] |
| v2x_frassoc_thick | Quantitative (interval, continuous) | Freedom of association thick index: represents the extent to which parties, including opposition parties, allowed to form and to participate in elections, and to what extent are civil society organizations able to form and to operate freely. | [0, 1] |
| v2x_suffr | Quantitative (interval, continuous) | Share of population with suffrage: represents the share of adult citizens as defined by statute has the legal right to vote in national elections. | [0, 1] |
| v2xel_frefair | Quantitative (interval, continuous) | Clean elections index: to what extent are elections free and fair? | [0, 1] |
| v2x_elecoff | Quantitative (interval, continuous) | Elected officials index: is the chief executive and legislature appointed through popular elections? | [0, 1] |
| v2x_liberal | Quantitative (interval, continuous) | Liberal component index: to what extent is the liberal principle of democracy achieved? | [0, 1] |
| v2xcl_rol | Quantitative (interval, continuous) | Equality before the law and individual liberty index: to what extent are laws transparent and rigorously enforced and public administration impartial, and to what extent do citizens enjoy access to justice, secure property rights, freedom from forced labor, freedom of movement, physical integrity rights, and freedom of religion? | [0, 1] |
| v2x_jucon | Quantitative (interval, continuous) | Judicial constraints on the executive index: to what extent does the executive respect the constitution and comply with court rulings, and to what extent is the judiciary able to act in an independent fashion? | [0, 1] |
| v2xlg_legcon | Quantitative (interval, continuous) | Legislative constraints on the executive index: to what extent are the legislature and government agencies e.g., comptroller general, general prosecutor, or ombudsman capable of questioning, investigating, and exercising oversight over the executive? | [0, 1] |
| v2x_partip | Quantitative (interval, continuous) | Participatory component index: to what extent is the participatory principle achieved | [0, 1] |
| v2x_cspart | Quantitative (interval, continuous) | Civil society participation index: are major CSOs routinely consulted by policymakers; how large is the involvement of people in CSOs; are women prevented from participating; and is legislative candidate nomination within party organization highly decentralized or made through party primaries | [0, 1] |
| v2xdd_dd | Quantitative (interval, continuous) | Direct popular vote index: to what extent is the direct popular vote utilized | [0, 1] |
| v2xel_locelec | Quantitative (interval, continuous) | Local government index: are there elected local governments, and — if so — to what extent can they operate without interference from unelected bodies at the local level? | [0, 1] |
| v2xel_regelec | Quantitative (interval, continuous) | Regional government index: are there elected regional governments, and — if so — to what extent can they operate without interference from unelected bodies at the regional level? | [0, 1] |
| v2xdl_delib | Quantitative (interval, continuous) | Deliberative component index: to what extent is the deliberative principle of democracy achieved? | [0, 1] |
| v2x_egal | Quantitative (interval, continuous) | Egalitarian component index: to what extent is the egalitarian principle achieved? | [0, 1] |
| v2xeg_eqprotec | Quantitative (interval, continuous) | Equal protection index: how equal is the protection of rights and freedoms across social groups by the state? | [0, 1] |
| v2xeg_eqaccess | Quantitative (interval, continuous) | Equal access index: how equal is access to power? | [0, 1] |
| v2xeg_eqdr | Quantitative (interval, continuous) | Equal distribution of resources index: how equal is the distribution of resources? | [0, 1] |
| v2elgvsuflvl | Nominal | Suffrage level: what is the level of suffrage practiced? | 17 unique values |
| v2expathhg | Nominal | HOG appointment in practice: how did the head of government gain access to office? | 10 unique values |
| v2elrstrct | Nominal (Dichotomous) | Candidate restriction by ethnicity, race, religion, or language: is the eligibility of candidates for national legislative office (when elected) formally restricted (by constitution or statute) by ethnicity, race, religion, or language? | 2 unique values |
| v2ddcredal | Nominal (Dichotomous) | Occurrence of any type of popular vote this year credible: if any direct democracy election occurred this year, was the official result of the vote, or votes (their success or failure) credible? | 2 unique values |
| v2exfemhog | Nominal (Dichotomous) | HOG female: what is the gender of the head of government? | 2 unique values |
| v2elcomvot | Ordinal | Compulsory voting: is voting compulsory (for those eligible to vote) in national elections? | 4 unique values |
| v2elfemrst | Ordinal | Female suffrage restricted: are women eligible to vote in national elections? | 3 unique values |
| v2ddlexci | Ordinal | Initiatives permitted: is there legal provision for initiatives? | 3 unique values |
| e_regionpol_7C | Nominal | Politico-geographical region: in which politico-geographic region is this country located? | 7 unique values |
| e_regiongeo | Nominal | Region: in which geographic region is this country located? | 19 unique values |

## Inquiry and Preliminary Analysis

Rather than include all three of our research focuses here, we have chosen to keep EDA and sketches in their own files to better segregate the different portions of our analysis.

### Geographical Analysis (Sidsel)

This analysis focuses on the spatial distribution of democracy, and how it has changed over time both within and between regions. Please see the [Geographical Analysis](../analysis/geographical_analysis/analysis1.ipynb) notebook.

### Episode Analysis (Jacob)

This analysis focuses on identifying and analyzing the nature of individual time-limited episodes of substantial democratic change. Please see the [Episode Analysis](../analysis/episode_analysis/analysis2.ipynb) notebook.

### Dimensional Analysis (Jennifer)

This analysis focuses on the relationships between the different dimensions of democracy identified in the dataset, and how they interact with each other over space and time. Please see the [Dimensional Analysis](../analysis/dimensions_analysis/analysis3.ipynb) notebook.

## Next Steps

| **Week** | **Goals** | **Milestone** |
| --- | --- | --- |
| **Week 1:** Begin Altair implementation | Each group member will work to develop Altair versions of their sketched representations. <br><br>By the end of this week we will come together as a team to structure how the final Altair views collectively will include:<br>• 3 UI widgets and 3 advanced interactions <br>• At least 1 bidirectional interaction <br>• At least 2 UI widgets and 2 advanced interactions used in concert within the same Altair view. | none |
| **Week 2:** Working Altair implementations | By the end of week 2, we aim to have working drafts of charts reflecting the analytic tasks described above. <br><br>Each team member will create one Altair view per analytic question, consisting of one or more visualizations. The aim is to include a variety of visualizations to illuminate different aspects of the question at hand. | none |
| **Week 3:** Review & implement feedback | Each team member will review teammate dashboards, and provide three or more pieces of actionable feedback for each teammate. Each team member will then revise based on both this peer feedback and TA feedback! | PM3: Dashboard due November 28th. |
| **Week 4:** Polish & record project video | Each team member will complete final edits to dashboards. <br><br>Each team member will draft a script for the portion of the video summarizing their dashboard. We’ll exchange these, and edit for coherency. Finally, we’ll meet to record the final video based on these scripts. | PM4: Feedback and video due December 5. |
