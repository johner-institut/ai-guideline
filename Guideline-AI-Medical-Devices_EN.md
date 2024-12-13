# Guideline for AI-based medical devices and IVD

## A) Meta information

### 1. Objective of the guideline

The objective of this guideline is to provide medical device and IVD manufacturers, authorities and notified bodies instructions and to provide them with a concrete checklist to

- understand what the expectations of the notified bodies and authorities are, resulting from 
  - medical device regulations such as [MDR](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:32017R0745) (regulation (EU) 2017/745 on medical devices) and 
  - [IVDR](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:32017R0746) (regulation (EU) 2017/746 on in vitro diagnostic medical devices) as well as from 
  - the [AI Act](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R1689) (regulation (EU) 2024/1689 on artificial intelligence),

- to promote step-by-step implementation of safety of medical devices and IVD, that implement artificial intelligence methods, in particular machine learning,
- to compensate for the lack of a harmonized standard (in the interim) to the greatest extent possible.

The guideline is **not** meant to serve as a training manual or guideline to achieve the safety of AI-based medical devices and IVD respectively. It is to be a guideline for its review.

The annex lists the recitals which led to the development of this guideline.

### 2. Scope of applicability and target group

This guideline is only applicable to medical devices and IVD that use AI methods, in particular machine learning. The requirements laid out by the AI Act, though, mostly do not affect medical devices of class I and IVD of class A.


The guideline applies in particular to
- Manufacturers of these products
- Their service providers (such as engineering providers)
- People and organizations that must assess the safety of these products, such as auditors, authorities and notified bodies.

The guideline only covers general safety and performance requirements with relation to AI. E.g., it does not address IT security aspects unless they are AI specific. IT security is scope of a [dedicated IT security guideline](https://github.com/johner-institut/it-security-guideline/).

### 3. Instructions for use

#### a) Structure of the guideline

This guideline follows the thought that the safety of AI based medical products can only be achieved through a process-oriented approach, whereby all relevant processes and phases of the life cycle must be considered such as:

1. Research and development
2. Data management
3. Post-market surveillance

Accordingly, the guideline does not set forth specific requirements for the products, but for the processes. It contains the following chapters:

1. General requirements
2. Requirements for product development
   1. Intended use
   2. Software requirement specification
   3. Data management
   4. Model development
   5. Product development
   6. Product release
3. Requirements for phases following development

#### b) Binding character of the guideline

This guideline is neither a legal requirement nor a harmonized standard. Accordingly, there is no differentiation between normative and informative elements.

Rather the guideline compiles best practices to reflect the required “state-of-the-art”.

Some of these best practices are not applicable in all situations, for all products or for all methods of machine learning. The manufacturers should at least justify non-obvious exclusions.

#### c) Use of the guideline

##### Creating and reviewing specifications

The manufacturers should first use the guideline to review the completeness of the specification documents (process and work instructions, checklists, etc.). These tasks are normally assumed by the following roles:

- Process-related persons, in particular heads of development, risk management and product management
- Quality manager and quality management deputy
- Regulatory affairs manager

##### Assessing products and QM system

Then the people responsible for the following tasks should use the guideline:

- Reviewing the conformity of products with the underlying safety and performance requirements
- Assessing the conformity of the technical documentation with the regulatory requirements
- Assessing the efficacy of the internal quality management system (e.g. for design reviews or audits)

The following roles are normally responsible for these tasks:

- Quality managers
- External and internal auditors (including notified bodies)
- Internal and external reviewers of technical documentation (including notified bodies and authorities)
- Testers
- Data scientists
- Clinical affairs specialists
- Regulatory affairs manager
- Risk manager

#### d) Structure of the guideline

The guideline is a grouped list of review criteria according to the aforementioned chapter. Each list element contains the following attributes:

- Unique ID
- Requirements / review criteria, that can be simply assessed as met or not met
- Comments
- Regulatory reference
- Reference to the ID of the [questionnaire of Team-NB](https://www.team-nb.org/wp-content/uploads/2024/11/Team-NB-PositionPaper-AI-in-MD-Questionnaire-V1-20241125.pdf) (that is based on this guideline)

The comments may contain:

- Examples
- Recommendations for implementation of reference to additional explanations
- Tips for auditors on how the fulfillment of the criteria can be assessed

### 4. Authors and rights of use

The following authors created this guideline:

- Prof. Dr. Christian Johner ([Johner Institute](https://www.johner-institut.de)) (Version 2019 and following)
- [Christoph Molnar](https://christophm.github.io/) ([LMU Munich](https://www.uni-muenchen.de/index.html)) (Version 2019)
- Dr. Andreas Purde, Dr. Abtin Rad ([TÜV SÜD](https://www.tuev-sued.de/)) (Version 2019)
- Prof. Dr. Dr. Christian Dierks ([Dierks + Company](https://www.dierks.company/)) (Version 2019)
- Stefan Bunk (CTO) and Sven Piechottka (Government & Regulatory Affairs) ([Merantix](https://www.merantix.com/healthcare/)) (Version 2019)

The guideline is published under the ([Creative Commons License](https://creativecommons.org/licenses/?lang=de)) of type [BY-NC-SA](https://creativecommons.org/licenses/by-nc-sa/4.0/). This requires a list of names of authors (“Christian Johner, Christoph Molnar et al.”) and allows third parties to build on this work, e.g. to correct it; however only for non-commercial purposes.

The license permits using the product for commercial consultancy purposes including audits and reviews. It is prohibited, however, to use this work itself in an unchanged or changed version for commercial purposes, e.g. in the form of sale as a brochure.

### 5. Document handling, document identification

This document is managed via the version management system git or the GitHub platform. Only the documents listed in this repository are valid.

The version history, including any authors may be found in the document history.

The released versions are on the main branch. Draft versions are to be found in other branches.

## B) General requirements

### 1. Process requirements

The manufacturers should cover all aspects listed below either in the standard operating procedures or in the relevant plans to ensure that the safety of the product is systematically guaranteed. Normally, the following standard operating procedures or plans are affected:

- Development
- Risk management
- Data management
- Verification and validation including testing of AI models (if not part of development)
- Labeling
- Collection and analysis of "automatically generated logs" according to 2024/1689/EU article 19
- Post-market surveillance and vigilance
- Service, installation, decommissioning
- Customer communication
- Management review (ISO 13485:2021 requires consideration of “applicable new or revised regulatory requirements”.)
- Data protection
- Identification of applicable regulatory requirements (regulations, directives laws, common specifications, harmonized standards)

If the manufacturer outsources processes, the requirements apply accordingly. Examples would be a (software) development service provider or contract research organization to be required to consider the relevant chapters of this guideline.

### 2. Plans

The manufacturer should compile all product specific plans as required by respective regulations.

- Development plan (incl. verification and validation planning)
- Post-market surveillance plan (s. 2017/745/EU Annex 1II, 2017/745/EU Annex IIII, 2024/1689 article 72 section 3.)
- Risk management plan
- Clinical evaluation plan

### 3. Competency requirements

The manufacturers must ensure and prove that they have sufficient competencies to ensure the relevant safety and performance of the products according to the state of the art. This proof is often gained most easily through internal or external training.

Manufacturers can use the competency of external resources.

|ID|Requirements|Comments|Regulatory references|Team-NB-ID|
|:--|:--|:--|---|:--|
|3.1|The manufacturer has created a list of all roles inside the scope of its QM system that are directly or indirectly concerned with AI.|Examples [^B2-01]|	ISO 13485 5.5.1 and 6.2., ISO 14971 3.3., IEC 62304 5.1, 2017/745/ EU Article 10.9, 21 CFR part 820.30 (b)| 5.1.1. |
|3.2|The manufacturer has identified and documented the competency requirements for each role inside the scope of its QM system that is directly or indirectly concerned with AI. [^B2-02]|Competencies are related to education, knowledge or skill. Examples of competencies: Machine learning, explainable AI, medicine (for relevant domains), clinical and usability validation.| ISO 13485 6.2., ISO 14971:2019 4.3, ISO 13485:2016 7.3.2, IEC 82304-1 6.1, 2024/1689/EU article 4 and 9 section 5. | 5.1.2. |
|3.3|The manufacturer has appropriate records for the training, further education and competencies that allow for the conclusion that the persons actually have these competencies.|| ISO 13485 6.2., ISO 14971 4.3 | 5.1.3 |
|3.4|The (software) development plans have defined the product-specific competencies (beyond or deviating).|| ISO 13485 7.3.2., IEC 82304-1 6.1. | 5.1.4 |
|3.5 |These competency requirements are met also for external resources (contractors, outsources processes) |||5.1.5|

[^B2-01]: Examples are: Data Scientists, Developers, Testers, Regulatory Affairs and Quality Mangers, Service and Support Employees, Product Managers, Medical Device Consultants, Physicians

[^B2-02]: Competencies levels such as understanding of capability to perform tasks should be listed, not just subjects

### 4. Documentation

The manufacturers should keep evidence that they have followed the relevant requirements of this guideline. There are no AI specific requirements for documentation and “objective evidence”.

In Europe at least, there is no obligation to create a specific document that summarizes the activities especially for AI. Manufacturers can integrate these aspects into existing documents such as QM documents (e.g. standard operating procedures, work instructions) and the technical documentation (e.g. software files, risk management files, clinical evaluation, summative evaluation of the usability).

Regulation 2024/1689/EU recommends to integrate the AI specific documentation into an existing technical documentation. It requires the documentation to be kept for 10 years after the AI system has been placed on the market (article 18.1).

## C) Requirements for product development

### 1. Intended use and stakeholder requirements

#### a) Intended medical use

|ID|Requirements|Comments| Regulatory references| Team-NB-ID |
|:--|:--|:--|---|:--|
|C1a1|The manufacturer has determined for which medical purpose (diagnosis, therapy, monitoring, predictions) the medical product should support.|The intended use / purpose should not be mistaken for the description of functionality (e.g. calculation of scores).| ISO 13485, 4.2.3. and 7.3.2. c., 2017/745/EU Annex II (1.1), 2924/1689/EC Annex IV section 1.(a), ISO 14971:2019, 5.2, 21 CFR 814.20 (b)(3)(i), 21 CFR part 820.30(c) | 6.1.1.1. |
|C1a2|The manufacturer has characterized the patients to be diagnosed, treated or monitored with the medical product. This characterization includes patient demographics, indications, contraindications and associated diseases.|This characterization is also included in IEC 62366-1. Patients may also simultaneously be users of the product.| 2017/745/EU, Annex I, 23.4 and Annex II, 1.1. c, 2017/746/EU, Annex II, 1.1. c, IEC 62366-1, 5.1. and 5.3., ISO 13485, 7.3.3 a., 21 CFR 814.20 (b)(3)(i)| 6.1.1.2 |
|C1a3|The manufacturer has stated whether there are patients under the age of 18 or other vulnerable groups,||2024/1689/EC article 9 section 10.||
|C1a4|The manufacturer has specified on which body locations the product will be used or from which body location the data originate.|Also called for in IEC 62366-1 clause 5.1.| 2017/745/EU, Annex II, 1.1., 2017/746/EU, Annex II, 1.1., IEC 62366-1, 5.1.3. | 6.1.1.3 |
|C1a5|The intended use also suggests what the goal of machine learning techniques is.|Classification and regression, clustering, similarity search and recommender systems are typical goals of machine learning methods. The description of the role of machine learning is necessary to fulfill the requirement for the description of the "physical principle".| IEC 62366-1, 5.1, 2017/745/EU Annex II, 1.1, 21 CFR part 814.20, XAVIER University "Building Explainability and Trust for AI in Healthcare"| 6.1.1.5 |
|C1a6|If applicable the manufacturer has described whether the device offers measuring functions.|This input is needed e.g., to determine the risk class of the device correctly.||6.1.1.4|
|C1a7|The manufacturer has determined the intended lifetime of the medical device respectively IVD.|This lifetime is determined, for example, by the state of the art (e.g., medical advances, new ML-methods, competitive products) and the speed at which the technical environment and libraries evolve.|||


#### b) Intended users and context of use

| ID                                               | Requirements                                                 | Comments                                                     |Regulatory references|Team-NB-ID|
| :----------------------------------------------------------- | :----------------------------------------------------------- |:--|---|:--|
| C1b1 | The manufacturer has characterized the intended users, e.g. using demographic features (age, gender), regarding the training, experience in medical domains, regarding technical knowledge, physical and mental limitations, linguistic skills and cultural background. | If the manufacturer does not foresee any limitations regarding these attributes, it must document this. | 2017/745/EU, Annex I, 5 and Annex II, 1.1, IEC 62366-1, 5.1., XAVIER University "Building Explainability and Trust for AI in Healthcare"| 6.1.2.1 |
|C1b2|The manufacturer has stated whether the device is intended to be used by lay persons.|This decision has regulatory implications such as the applicability of requirements of Regulations 2017/745/EU and 2017/746/EU in Annex I and 2024/1689/EU.|2017/745/EU Annex I section 22 and 2017/746/EU Annex I section 19|6.1.2.3|
| C1b3 | The manufacturer has characterized the intended use environment (also social environment such as stress, shift work, frequently changing colleagues)| This characterization is also required by IEC 62366-1. It is also relevant in the context of the explainability of AI, as AI can change the use environment e.g., tasks and workload. | 2017/745/EU, Annex I, 5, IEC 62366-1, 5, XAVIER University "Building Explainability and Trust for AI in Healthcare", UK 811.4 Position Paper | 6.1.2.2 |
|C1b4 |The manufacturer has described the core tasks that the medical device is to support. | The use scenarios that manufacturers must specify according to IEC 62366-1 can also be derived from these core tasks.| IEC 62366-1 |  |

#### c) Stakeholder requirements

| ID                                               | Requirements                                                 | Comments                                                     |Regulatory references|Team-NB-ID|
| :----------------------------------------------------------- | :----------------------------------------------------------- |:--|---|:--|
| C1c1 | The manufacturer has operationalized the goals listed in the intended use with quantitative values [^C.1.c.1]. | It is not unusual that these values are supplemented and revised during the course of development. | 2017/745/EU, Annex I, 23.4 and Annex III, 1.1, FDA SW validation guidance 5.2.2, FDA Guidance for the Content of Premarket Submissions for Software Contained in Medical Devices (s. "Software Requirements Specification")| |
| C1c2 | The manufacturer has set forth the runtime environment of the product regarding hardware (screen size, screen resolution, storage, network connection etc.) and software (e.g. operating system, browser, runtime environments such as Java runtime environment or .NET). | For some mobile apps, this characterization must be done for the app and for the server part. | 2024/1689/EU annex IV section 1.(b), ISO 13485, 7.3.3, 2017/745/EU, Annex I, 17.3 and 17.4, IEC 62304, 5.2, XAVIER University "Building Explainability and Trust for AI in Healthcare", FDA SW validation guidance 5.2.2, FDA Guidance for the Content of Premarket Submissions for Software Contained in Medical Devices (s. "Software Requirements Specification")| |
| C1c3 | The manufacturer has specified the data interfaces using the levels of the [interoperability model](https://www.johner-institut.de/blog/tag/interoperabilitat/) and set forth the formats and for images, their specific properties (size, resolution, color coding). | This is required pursuant to IEC 62304 chapter 5.2.2. | 2024/1689/EU annex IV section 1.(b), IEC 62304, 5.2.2, FDA Guidance for the Content of Premarket Submissions for Software Contained in Medical Devices (s. "Software Requirements Specification")| 6.2.3.1. |
|C1c4 |The manufacturer has specified the requirements for the input data. | The input data may also depend on the generation of the data, e.g. on the recording method, on technical parameters (magnetic field strengths, number of conductive electrodes, direction), on environmental conditions during the recordings, on the manufacturer, on the medical device, etc. | IEC 62304, 5.2, ISO 14971:2019, 5.3, FDA Guidance for the Content of Premarket Submissions for Software Contained in Medical Devices (s. "Software Requirements Specification") | 6.2.3.2. |
| C1c5 | The manufacturer has set forth all markets and documented the list of applicable regulatory requirements and the process how to identify these requirements. | Regulatory requirements include regulations, directives, laws, common specifications and harmonized standards. Show this list. | 2017/745/EU, Annex IX, 2.2, ISO 13485, 5.2 and 7.2.1, EN ISO 13485 4.1.1, 2024/1689/EU articles 17 section 1.(e), 41 section 5. and Annex IV 7. | 6.1.3.2 |
| C1c6 | The manufacturer has specified whether the system should continue to learn after it has been placed on the market. |If this is the case, the manufacturer has specified whether this continuous training will be global/centralized or decentralized (e.g., per product or per hospital) and online or offline.|||

[^C.1.c.1]: **Example**: Purpose: The software supports radiologists in diagnosing cancers using CT images of the head. Quantitative value: 95% of radiologists working with software detect the cancer.


#### d) Input for risk management and clinical evaluation

| ID                                               | Requirements                                                 | Comments                                                     | Regulatory References| Team-NB-ID |
| :------------------------------------------------------------ | :------------------------------------------------------------ |:--|---|:--|
| C1d1 | The manufacturer has listed alternative procedures and evaluated them in terms of benefit, safety, and performance. | The discussion of the state-of-the-art is a requirement of MEDDEV 2.7/1 and the MDR/IVDR. | 2017/745/EU, Annex I, 1., 2017/746/EU, Annex I, 1.,  MEDDEV 2.7/1, ISO 14971:2019, 4.2 and 10.9, FDA guidance on "Factors to Consider When Making Benefit-Risk Determinations in Medical Device Premarket Approval" (e.g. Part C)| 6.1.5.1 |
| C1d2 | The manufacturer has compared the aforementioned quantitative values with the relevant values of alternative methods. | Manufacturers should create a tabular overview.  ||(6.4.4.9.)|
| C1d3 | The manufacturer has justified why machine learning is superior to the other methods and thus justified the associated risks. | | 2017/745/EU, Annex I, 1., 2017/746/EU, Annex I, 1., MEDDEV 2.7/1 | (6.1.4.2) |
| C1d4 | The manufacturer has drawn up a list of risks specifically arising from the application of machine learning methods. | E.g., self-learning systems and LLMs can reveal a different output despite unchanged input data. | ISO 14971, 5.4. and 5.5., 2017/745/EU, Annex I, 3., DIN SPECT 2, ISO/TR 31004:2013 - Risk management - Guidance for the implementation of ISO 31000, UK 811.4 Position Paper | (6.1.2.5), 6.1.4.3 |
| C1d5 | The manufacturer has analyzed the risks arising if persons other than the specified users, use the product. |                                                              | ISO 14971, 5. | 6.1.4.5 |
| C1d6 | The manufacturer has analyzed the risks caused by a change of the use environment by the deployment of an AI-based system. |E.g. these systems can change, add or eliminate tasks or increase the workload. Working remotely instead of in a hospital is another example.  |UK 811.4 Position Paper||
| C1d7 | The manufacturer has analyzed the risks arising through use in an environment different than that specified. | e.g., the product is unexpectedly used in a home office. |  2017/745/EU, Annex I, 14.2.(d), 2017/746/EU, Annex I, 13.2.(d), ISO 14971, 5., IEC 82304-1, 4.1. (b)  |  6.1.4.9  |
| C1d8 | The manufacturer has analyzed the risks arising from inputs not meeting the specified prerequisites (e.g., quality, value range, format and unit). | | ISO 14971, 5., IEC 82304-1, 4.1. (c)| 6.1.4.6 |
| C1d9 | Manufacturers have analyzed risks arising from data not generated according to the specified prerequisites. | Examples: new type of CT scanner, MRT with new sequences ||(6.1.4.11)|
| C1d10 | The manufacturer has assessed the risks when the system is used for patients or patient populations other than that specified. | This could be part of a foreseeable misuse. | ISO 14971, 4.2., 4.3., 5., IEC 82304-1, 4.1., 2024/1689/EU article 9 section 2.(b) | 6.1.2.6, 6.1.4.8 |
| C1d11 | The manufacturer has analyzed the risk for fundamental rights.|Examples are the right to informational self-determination (data protection) and the right to the access of adequate healthcare.|2024/1689/EU article 9 section 2.(a)||


### 2. Software requirements

#### a) Functionality and performance

|ID|Requirements|Comments|Regulatory references|Team-NB-ID|
|:--|:--|:--|---|:--|
|C2a1|The manufacturer has comprehensibly derived quantitative quality criteria or requirements for the software or/and the algorithm from the intended use and stakeholder requirements [^C.2.a.1].|This comprehensibility can be represented particularly well with a traceability matrix.| 2024/1689/EU annex IV, ISO 13485, 7.3.3., IEC 62304, 5.2, XAVIER University "Building Explainability and Trust for AI in Healthcare", FDA guidance on "Software Validation", chapter 5.2.2| (6.1.3.1.), 6.2.1.1. |
|C2a2|The manufacturer considered for example the following quantitative quality criteria or requirements: for classification problems, accuracy (mean or balanced accuracy), positive predictive value (precision), specificity and sensitivity; for regression problems, mean absolute error and mean square error.| For unbalanced data, i.e. when labels occur with very different frequencies, balanced instead of mean accuracy should be used. However, the choice of quality criteria depends strongly on the intended use. | ISO 13485, 7.3.3., 7.3.4., IEC 62304, 5.2. | 6.2.1.2. |
| C2a3 | The manufacturer has specified the expected value ranges of the outputs.| | ISO 13485, 7.3.3., 7.3.4., IEC 62304, 5.2. | 6.2.1.4. |
|C2a4|The manufacturer has specified the requirements regarding repeatability and reproducibility of requirements.|This is particularly relevant with "Continuous Learning Systems".| 2017/745/EU, Annex I, 17.1. , 2017/746/EU, Annex I, 16.1., ISO 13485, 7.3.3., 7.3.4 | 6.2.1.5. |
|C2a5|The manufacturer has specified how the system will behave if the inputs do not meet the specified conditions [^C.2.a.2].|This is an aspect of robustness to be specified according to ISO 25010 and IEC 62304 Chapter 5.2. | ISO 25010,, IEC 62304, 5.2., ISO 14971:2019, 5.4, FDA guidance on "Software Validation" chapter 5.2.2, FDA digital health criteria| 6.2.1.6. |
|C2a6|The manufacturer has determined which self-tests the system must perform and how it behaves if this is not successful.|This is particularly relevant for "Continuous Learning Systems".| ISO 13485, 7.3.3. | (6.2.1.7.) |
|C2a7|The manufacturer has determined how fast the system must create the outputs.|This determination may be done depending on the size and amount of data.| 2017/745/EU, Annex I, 17.1., 2017/746/EU, Annex I, 16.1., ISO 13485, 7.3.3. | 6.2.1.8. |
|C2a8|The manufacturer has specified the availability of the medical device.|This is an aspect of robustness and must be specified pursuant to ISO 25010 and IEC 62304 chapter 5.2.| ISO 25010, IEC 62304, 5.2., ISO 14971, 4.3., ISO 13485, 7.3.3. | 6.2.1.9. |
|C2a9 |The manufacturer has specified the requirements related to audit logs. |AI Act speaks of "record keeping".|2024/1689/EU article 12||

[^C.2.a.1]: Examples:  **Example 1**: The stakeholder requirement (user requirement) states that 95% of radiologists must be able to detect a cancer with the product. The requirement of the algorithm states that it must display a sensitivity of 97%. **Example 2**: The stakeholder requirements state that arterial calcification must be able to be detected at a sensitivity of 92%. The requirements of the algorithm state that it must be able to exactly predict the strength of the plaques in the blood to 0.2 mm.

[^C.2.a.2]:  Examples: incomplete data sets, lack of data sets, wrong data format, excessive data quantities, data outside of specified value ranges, wrong temporal sequence of data.

#### b) User interface

| ID                                               | Requirements                                                 | Comments                                                     | Regulatory references| Team-NB-ID |
| :----------------------------------------------------------- | :----------------------------------------------------------- | :--| ---| :--|
|C2b1 |The manufacturer has specified the user interface (requirements). |IEC TR 62366-2 provides examples.| 2024/1689/EU annex IV section 1.(g), IEC 62304 5.2.2 f), IEC 62366-1 5.6 | |
| C2b2 | The manufacturer has specified what the user interface must display when the preconditions are not met[^C.2.a.2] or in case of internal errors in order to operate the system safely (e.g., inputs not valid or not expected). | AI Act requires "human oversight" which itself may lead to product / UI requirements such as monitoring information, warning of anomalies and dysfunctions as well as a kill switch. | 2017/745/EU, Annex I, 5., 2017/746/EU, Annex 1, 5., 2024/1689/EU article 14 section 4., IEC 62366-1, 5.2., FDA HFE guidance, FDA guidance on software validation e.g. chapter 5.2.3 | 6.2.2.1. |
| C2b3 | The manufacturer has specified what the user interface must display if the output does not meet the specified quality criteria. |    |  | 6.2.2.2. |
|C2b4|The manufacturer has specified the information the UI must provide to explain the system output (results)|Alternatively a rationale must be given that there is no need for "explainability". The target of this information is to reduce risks and to allow the "human oversight". | 2024/1689/EU article 14 section 4.(c) |  |
| C2b5 | The manufacturer has determined whether instructions for use and training materials are required. | The MDR / IVDR allow exceptions to the obligation. | 2017/745/EU, Annex I, 23., 2017/746/EU, Annex I, 20., ISO 13485, 4.2.3., FD&C, 21 CFR parts 801 and 820.120| 6.2.2.3. |


#### c) Additional software requirements

| ID                                               | Requirements                                                 | Comments                                    | Regulatory references| Team-NB-ID |
| :----------------------------------------------------------- | :------------------------------------------ |:--|---|:--|
| C2c1 | The manufacturer has set forth which requirements the system must fulfill to detect internal system errors. | Could be an audit log or a monitoring port. | 2017/745/EU, Annex I, 17, 18, 23.4, IEC 62304, 5.2, 5.3 and 7.1, ISO 149781:2019, 5.4, FDA guidance on software validation e.g. chapter 5.2.2, 5.2.3 and 5.2.4, GMLP Guiding Principles (by FDA et al) #2 (data integrity)  | 6.2.3.3. |
| C2c2 | According to the GDPR, the specified system must not expose patients to decisions based exclusively on automatic data processing. Manufacturers should address the corresponding requirement and be able to justify the chosen legal basis. |   | Art. 22 of the GDPR. |  |
| C2c3 | The manufacturer has determined the requirements that the software must meet in order to ensure the IT security of the product. | IT security is not the subject of this guideline, but the [IT-Security Guideline](https://github.com/johner-institut/it-security-guideline/). | 2024/1689/EU article 15 section 5. | 6.2.4.x |



#### d) Special requirements for continuous learning systems

| ID                                               | Requirements                                                 | Comments                                                     | Regulatory references | Team-NB-ID |
| :----------------------------------------------------------- | :----------------------------------------------------------- |:--|:--|---|
| C2d1 | The manufacturer has defined when and how often the model is updated. | For this purpose, the manufacturer should define the "triggers" of these updates. He must also describe whether these updates take place per individual medical device or for all medical devices of the type.  |                                                              |                                                              |
| C2d2 | The manufacturer has specified how the additional data will be quality assured and how incorrect, missing or implausible data will be dealt with. ||||
| C2d3 | The manufacturer has defined in which range the output data may change. | This requires a description of how the algorithms change.  |||
| C2d4 | The manufacturer has described how it continues to ensure the correctness and accuracy of the output data and what happens if this can no longer be guaranteed. | Self-checks, the possibility of roll-backs, limiting outputs are possible approaches. |||
|C2d5 |The manufacturer has described whether and how users are informed about changes to the algorithm and whether they can decide about them. | |||
|C2d6 |The manufacturer has identified and managed the specific risks arising from continuous learning. | To this end, the manufacturer must justify that it achieves a better risk-benefit ratio through continuous learning. |||

[^C.2.d.1]: The state-of-the-art of technology is not necessarily consistent with the state of science and thus the gold standard nor with the “Ground Truth”. This means that the system requirements are lower than with a gold standard respectively the "Ground Truth". This would be the case in particular if the latter require an invasive or very cost-intensive procedure.

### 3. Data Management

Data generally have to be understood as training, validation and test data as well as labels. Each type has to fulfill specific requirements. If not specified differently, however, the usage of the term "data" relates in the following to all types.

#### a) Data collection

| ID                                               | Requirements                                                 | Comments                                                     | Regulatory references| Team-NB-ID [^6.3.a.7]|
| :------------------------------------------------------------| :------------------------------------------------------------|:--|---|:--|
|C3a1|The manufacturer has defined a procedure that defines the data management including data collection, data processing, data analysis||2024/1689/EU articles 10 section 2 and 17 section 1.(f), ISO 13485 4.1||
| C3a2 | The manufacturer has specified the number of data sets and given a justification why this is sufficient [^C.3.a.1]. | This concerns the data sets for training, validation and test. | ISO 13485, 7.3.7, 2024/1689/EU article 10 section 2.(b) and (e) | 6.3.1.9. |
|C3a3 |The manufacturer has characterized the inclusion and exclusion criteria of data by relevant attributes [^C.3.a.2]. | This includes documentation of data types, units and value range. | ISO 24028, XAVIER University "Building Explainability and Trust for AI in Healthcare" | 6.3.1.10. |
|C3a4 |The manufacturer has specified inclusion and exclusion criteria for data [^C.3.a.3]. ||2024/1689/EU article 10 section 2.(f)|6.3.1.11.|
| C3a5 | The manufacturer has described the procedure by which it ensures that data sets that do not meet the inclusion criteria or should be excluded are actually excluded. | Procedure includes a software supported assessment. This software must be validated. |2024/1689/EU article 10 section 2.(f)|6.3.1.12.|
| C3a6 | The manufacturer has described the collected data using descriptive statistics[^C.3.a.4]. | The ["Dataset Nutrition Label"](https://ahmedhosny.github.io/datanutrition/) is a recommended option. | 2024/1689/EU article 10 section 2.(f) and Annex IV section 2.(d)| 6.3.1.13., 6.3.4.13. |
| C3a7 | The manufacturer has describe the origin of data (e.g. clinics, devices). |  | | 6.3.4.12. |
| C3a8 | The manufacturer has justified where the data are collected and why these are representative for the target population. As reasonable, these have been compared to scientific publications and to registers. | | 2024/1689/EU article 10 section 4. and 5.| 6.3.1.14. |
| C3a9 | The manufacturer has listed and discussed factors that could cause a bias in the data. |   | ISO 24028 e.g. 10.5, 2024/1689/EU article 9 sections 2.(d) and 5.(a), article 10 sections 2.(f), 2.(g), 4.| 6.3.1.16. |
| C3a10 | The manufacturer has analyzed which influences the type and location of data collection have on the data[^C.3.a.5]. |||6.3.1.17.|
|C3a11 |The manufacturer has established a procedure to ensure that data protection requirements are met. | For example, the data is anonymized or pseudonymized before testing and training. The data protection officer should be involved in this.  |2024/1689/EU article 10 section 5, 2016/679/EU|6.3.1.18.|
| C3a12 | The manufacturer has examined and excluded the possibility of a “label leakage”[^C.3.a.6]. | This depends on the applied ML model is not a general best practice. ||6.3.1.19., 6.3.1.20.|
| C3a13 | The manufacturer that uses surveys has justified the selection of the surveys, the time of survey and possibly the method for their assessment, in particular if no standardized survey exists. |                                                              |||

[^C.3.a.1]: A specification for the number of data is hardly possible. This depends on the “signal-noise-ratio” among other things. For example, for one data set, the percentage of relevant genes and the strength and frequency of the predicted effects affect the number. For data to be classified, the number of the data sets with the rare class (e.g. the prevalence of diseases) is decisive.

[^C.3.a.2]: e.g. demographic data (age, gender), physical parameters (height, weight), diseases, vital parameters, lab parameters, presence of additional tests, case history.

[^C.3.a.3]: Examples: **Example 1**: Patients who must be ruled out due to a heart pacemaker or lung surgery because the images cannot be analyzed or could lead to erroneous classification. **Example 2**: Formats and technical parameters such as image sizes, resolution, brightness and contrasts, color coding, compression, recording equipment, recording method (e.g. CT versus MRI), with or without contrast agent, zoom. **Example 3**: Completeness of meta-data.

[^C.3.a.4]: Usually, the calculation of distributions (histograms), mean / average values, quartiles, possibly “joint distribution of features". The correlation of data among that data should be examined. Additional examples are found in the [publication by Sarah Holland et al.](https://arxiv.org/pdf/1805.03677.pdf) (such as in table 1)

[^C.3.a.5]: Examples: Influence of various measurement devices, surveys, policies (such as a clinic only takes lab parameters only in emergencies, another routinely. Frequency and reason examined with the patient), type of clinic (e.g. small hospital, from which all serious cases must be referred versus university hospital > survivor basis), self-selection bias (e.g. patients with various pre-existing conditions usually go to a hospital rather than a medical practice), type of study (prospective versus retrospective)

[^C.3.a.6]: These are data in which non-causal information are found in the data via the label, e.g. in the sorting (e.g. first the data of healthy persons, then of ill persons), in the hospital (from one the severe cases originate), in images (e.g. for skin cancer, one must always see a ruler). An additional example would be multiple CT images of a patient, in which the model learns using the patient and not the disease. This could happen if a rib fracture can be seen in addition to the cancer on multiple images.

[^C.3.a.7]: The Team-NB document starts the numbering of this section with 9 instead of 1. I.e. there are no items 6.3.1.1. to 6.3.1.8.

#### b) Data labeling

| ID                                               | Requirements                                                 | Comments                                                     | Regulatory references| Team-NB-ID |
| :------------------------------------------------------------| :------------------------------------------------------------|:--|---|:--|
| C3b1 |  In the case of "Supervised Learning", the manufacturer has derived the labels from the intended use with which the training data are provided and justified this choice. | |2024/1689/EU article 10 section 3|6.3.2.1.|
| C3b2 | The manufacturer has defined a procedure for labeling in "Supervised Learning", if labels were not yet present in the data.   | | ISO 13485, 4.1, 2024/1689/EU article 10 section 2.(c) | 6.3.2.2. |
| C3b3 | This procedure specifies quantitative classification criteria for labeling. The selection of these criteria has been justified by the manufacturer[^C.3.b.1]. | If the "Ground Truth” is not chosen[^C.3.b.2], because it is too expensive or invasive, this must also be justified. |                                                            | 6.3.2.3. |
| C3b4 | This procedure specifies the requirements for the number, training and competency for the people responsible for labeling. |  | ISO 13485, 6.2 and 7.3.2, FDA 21 CFR part 820.25  | 6.3.2.4. |
| C3b5 | This procedure sets forth how the competencies of the persons responsible for labeling is tested. | This can be done by the labeling of selected data sets.      ||6.3.2.5.|
| C3b6 | This procedure sets forth how the persons responsible for labeling are trained and how the success of this training is evaluated. |                                                              ||6.3.2.6.|
| C3b7 | This procedure sets forth how the correctness of the label is systematically reviewed. The selection of this justification has been documented by the manufacturer. | The manufacturer can provide identical data sets of multiple persons and assess the consistency of the results. ||6.3.2.7.|
| C3b8 | This procedure sets forth, how the monitoring occurs, that the persons responsible for labeling are continually fit and willing to perform the labeling [^C.3.b.3]. | This can be done with datasets with already known labels that are inserted unnoticed by the person during labeling. ||6.3.2.8.|

[^C.3.b.1]: If, for example,  patients have to be classified as healthy and sick, the manufacturer must derive the criteria specifically for the intended use, when a patient is to be classified as healthy and when as sick.

[^C.3.b.2]: The “Ground Truth” is the most precise reference method (state of the art). For the determination of arterial hypertension, an invasive blood pressure measurement may provide the most exact results.

[^C.3.b.3]: The labeling of dozens of data sets is arduous. A payment per data set can cause an inappropriate motivation.

#### c) Procedure for (pre-)processing of data

| ID                                               | Requirements                                                 | Comments                                                     | Regulatory references| Team-NB-ID |
| :------------------------------------------------------------| :------------------------------------------------------------|:--|---|:--|
| C3c1 | The manufacturer has set a procedure that describes the pre-processing of the data. |   | ISO 13485:2016, 4.1.6, 7.3.6, XAVIER University "Building Explainability and Trust for AI in Healthcare", FDA 21 CFR part 820.70(i)   | 6.3.3.1. |
| C3c2 | This procedure describes the individual processing steps such as conversion, transformation, aggregation, normalization, format conversion, calculation of feature, conversion of numerical data into categories. | A graphic representation creates a rapid overview. The conversion of numerical to categorical values requires a justification. | | 6.3.3.2. |
| C3c3 | The procedure describes how the correctness of the interim steps and the final results are assessed[^C.3.c.0] through risk-based evaluations. | This is consistent with the requirements of ISO 13485:2016 chapter 4.1.6. The risk management file must contain these analyzes. | ISO 13485, 4.1.6., 7.3.2., 7.5.6. | 6.3.3.3. |
| C3c4 | This procedure specifies how values with various measurement scales or units are detected and processed. | This depends on the ML-method used (e.g. tabular data / image data) and cannot be demanded as a general best practice.  |                                                            | 6.3.3.4. |
| C3c5 | This procedure specifies how values are detected and processed that have been collected with various measurement methods. | This depends on the ML- method used (e.g. tabular data / image data) and cannot be demanded as a general best practice.       |                                                     | 6.3.3.5. |
| C3c6 | This procedure specifies how values or metadata with the same names (such as in column headers) are detected and processed. | This, however, depends on the ML-method used (e.g. tabular data / image data) and cannot be demanded as a general best practice. ||6.3.3.6.|
| C3c7 | This procedure specifies how missing values within data sets are detected and processed. The manufacturer gives a rationale for the decision[^C.3.c.1]. | Make sure that the rationale differentiates between “missing at random” and “missing not at random”[^C.3.c.2]. |                                                        | (6.3.3.7.) |
| C3c8 | This procedure specifies how outliers are detected and processed[^C.3.c.3]. The manufacturer gives a rationale for the decision[^C.3.c.4]. | Show example of a date / feature. This, however, depends on the ML-method used (e.g. tabular data / image data) and cannot be demanded as a general best practice. ||(6.3.3.7.)|
| C3c9 | This procedure specifies how unusable data sets are detected and handled[^C.3.c.5]. The determination was justified by the manufacturer. | Request example of a date / feature.                         ||(6.3.3.7.)|
| C3c10 | The manufacturer has identified, assessed, and managed the risks arising from data processing. | Risks can be caused, for example, by software errors, rounding errors, re-sampling and compression of data, and the sorting out of invalid data. |  AI4H-DAISAM |   |

[^C.3.c.0]: Options include software tests and redundant or alternative calculations such as with Excel.

[^C.3.c.1]: The options for processing include deleting the data set, replacement by the average value of other data sets, new value “missing” (for categorical values).

[^C.3.c.2]: An example for "missing not at random” is lab values that are too high that are cut off.

[^C.3.c.3]: The options for processing include deleting the data set, correcting the value, setting the value to a set value (min/max).

[^C.3.c.4]: This justification is more important in the regression method than with tree-based methods.

[^C.3.c.5]: Examples are x-rays of poor quality or patients who do not meet the inclusion criteria.

#### d) Documentation and version control

| ID                                               | Requirements                                                 | Comments                                                     | Regulatory references| Team-NB-ID [^C.3.d.1.] |
| :------------------------------------------------------------| :------------------------------------------------------------|:--|---|:--|
|  C3d1         |  The manufacturer has described the "funnel", which shows how much data originates from which data sources (e.g. clinics) and at which processing step how many data records were dropped and for what reason.              |                                                              |||
| C3d2 | The manufacturer has described which parts of the software are responsible for which processing step. | This should be part of the architecture of this software.  |||
| C3d3 | The manufacturer has described the processed data using descriptive statistics [^C.3.a.4]. | ["Dataset Nutrition Label"](https://ahmedhosny.github.io/datanutrition/) is recommended.|||
| C3d4 | The manufacturer has all software for data processing, including the libraries used in the process, documented and under version control. ||  ISO 13485, 4.1.6., 4.2.4., 7.5.6. | 6.3.4.10. |
| C3d5 | The manufacturer has all training, validation and test data under version control. ||  | 6.3.4.11. |
| C3d6 | The manufacturer has a procedure for data storage and retention according to applicable regulatory requirements. |These requirements specify on the one hand a minimum retention period such as 2017/745/EC, 2024/1689/EC, ISO 13485. On the other hand there are data protection requirements to minimized (time) of data storage.|  | 6.3.4.14. |


[^C.3.d.1.]: The numbering of the corresponding section 6.3.4 in Team-NB document starts with 9. I.e. the numbers 6.3.4.1. - 6.3.4.8. are missing.

### 4. Model development 

#### a) Preparation

| ID                                               | Requirements                                                 | Comments                                                     | Regulatory references| Team-NB-ID |
| :------------------------------------------------------------| :------------------------------------------------------------|:--|---|:--|
| C4a1 | The manufacturer has justified the selection of features that it considers during training. | This requires a list of all features.  | ISO 13485, 7.3.2., 7.3.3. | (6.4.1.1) |
| C4a2 | The manufacturer has described the dependency of the features among each other, especially for tabular data. | A Directed Acyclic Graph (DAG) helps with the visualization. This depends on the applied ML-method and cannot be demanded as a general best practice. | ISO 13485, 7.3.2., 7.3.3. | 6.4.1.3. |
| C4a3 | The manufacturer has documented and justified the ratio that it divides up the data into training, validation and test data. |                                                              ||6.4.1.4.|
| C4a4 | The manufacturer has documented the stratification it uses to divide up the data in to training, validation and test data[^C.4.a.1]. |    | ISO 24028 9.8.2.1, DAISAM | 6.4.1.5. |
| C4a5 | The manufacturer has documented how he ensures that multiple data sets for an object are in the same “bucket” (training, validation and test data). |                                                                                                  |                                                     |                                                     |
| C4a6 | The manufacturer has documented how he ensures that test data are not used for model training and validation. |                                                              |                                                            | 6.4.1.7. |
| C4a7 | The manufacturer has described when it recodes the data specifically for the model or specifically for the library[^C.4.a.2]. |                                                              ||6.4.1.8.|

[^C.4.a.1]: For data with rare features or labels, it may be necessary to distribute the data not just at random.

[^C.4.a.2]: Examples of this are normalization, selection of class labels (e.g. 0 or 1), selection of column names, distribution of categorical values over multiple columns.

#### b) Training

| ID                                               | Requirements                                                 | Comments                                                     | Regulatory references| Team-NB-ID |
| ------------------------------------------------------------ | ------------------------------------------------------------ | -- | -- | -- |
| C4b1 | The manufacturer performs model training, tuning of hyperparameters and model selection exclusively with the training and validation data (e.g. using cross-validation). |  The manufacturer should also show that the training actually improves the quality of the model.   |                                                         |                                                         |
| C4b2 | The manufacturer tried different sets of hyperparameters and documented his final choice.[^C.4.b.1]. | ISO 14971 requires risks to be minimized. |                                                           |                                                           |
| C4b3 | The manufacturer has documented the choice of epochs[^C.4.b.2].  |       |||
| C4b4 | The manufacturer has determined, documented and justified the quality parameters on the basis of the intended use for which he wants to optimize the model. | This means that the choice of these quality parameters is specific to the intended use. ||(6.4.2.1.)|
| C4b5 | The manufacturer has - as far as reasonable - trained and compared several model types (including simpler and interpretable model). |   ||6.4.2.2.|

[^C.4.b.1]: Examples: Loss function, optimizer, learning rate, number of epochs

[^C.4.b.2]: It can be useful to show the dependence of the quality of the model on the number of epochs by means of learning curves. These learning curves exist, for example, for neural networks and boosting methods, but not for models with numerical solution (e.g. linear regression) or with a single tree.	

#### c) Evaluation

| ID                                               | Requirements                                                 | Comments                                                     | Regulatory references| Team-NB-ID |
| ------------------------------------------------------------ | ------------------------------------------------------------ |--|--|--|
|C4c1|The manufacturer has planned the evaluation of the model.| This plan can be part of a development or V&V plan. | ISO 13485, 7.3.2, 7.3.6 and 7.3.7, ISO 14971:2019, 10., IEC 62304 5.1 |  |
|C4c2 |The manufacturer has documented the quality measures for the various models, e.g. in the case of a binary classification using a four-field table. | This documentation should not only include the values to which the manufacturer has optimized the model. | 2024/1689/EU article 9 section 8. and annex IV section 2.(g)| 6.4.3.1. |
|C4c3 |The manufacturer has not only evaluated and documented the quality metrics for the different models globally, but also separately for different features, if applicable. | ||6.4.3.2., 6.4.3.3., 6.4.4.9|
|C4c4 |The manufacturer has shown how to recognize and thus avoid overfitting. | | ISO 24028 9.8.2.23 | 6.4.3.4. |
|C4c5 |The manufacturer has examined the data sets that were predicted particularly well and those that were predicted particularly poorly. | A residuals analysis is recommended, in which the errors are plotted against the feature values, if applicable. ||6.4.3.5.|
|C4c6 |The manufacturer has examined the data sets for which the model is particularly safe and particularly unsafe[^C.4.c.1]. | This will help identifying limitations e.g., for certain patient groups | 2024/1689/EU annex IV section 3.| 6.4.3.6. |
|C4c7 |The manufacturer has justified the ultimate choice of model on the basis of the quality criteria and the intended use, and has explained in particular when simpler and more interpretable models were not used. |  | ISO 14971:2019, XAVIER University "Building Explainability and Trust for AI in Healthcare", DIN SPECT 2 | 6.4.3.7. |
|C4c8 |The manufacturer has considered, especially for tabular data for individual data sets, to have the model show the features that particularly influenced the decision [^C.4.c.2]. | This cannot be claimed as a general best practice. ||6.4.3.8.|
|C4c9 |The manufacturer has considered evaluating, especially for tabular data, how and how much individual features would have to change for the model to come to a different prediction. | This is referred to as ["counterfactuals"](https://christophm.github.io/interpretable-ml-book/counterfactual.html). This cannot generally be claimed as a best practice. ||6.4.3.9.|
|C4c10 |The manufacturer has considered analyzing/visualizing the dependence (strength, direction) of the predictions on the feature values, especially for tabular data [^C.4.c.3]. | This cannot be claimed as a best practice in general. ||6.4.3.10.|
|C4c11 |The manufacturer has considered synthesizing data sets that particularly activate the model[^C.4.c.4]. | This cannot be generally claimed as best practice. ||6.4.3.11.|
|C4c12 |The manufacturer has considered approximating the model with a simplified surrogate model such as a decision tree. | This cannot generally be claimed as best practice. |||

[^C.4.c.1]: Classification tasks must take into account the current state of research.

[^C.4.c.2]: Approaches include LIME (Local Interpretable Model-agnostic Explanations), Beta (Black Box Explanations through Transparent Approximations), LRP (Layer-wise Relevance Propagation) and Feature Summary Statistics (incl. Feature Importance and Feature Interaction).

[^C.4.c.3]: Examples of Shapley-Values, ICE-Plots, Partial Dependency Plots (PDP)

[^C.4.c.4]: For examples see http://yosinski.com/deepvis

#### d) Documentation

| ID                                               | Requirements                                                 | Comments                                                     |Regulatory references|Team-NB-ID|
| ------------------------------------------------------------ | ------------------------------------------------------------ |--|--|--|
| C4d1 | The manufacturer has the model[^C.4.d.1] and/or the training code under version and configuration control. | That includes scripts and build files.   | ISO 13485, 4.1.6., 4.2.4., 7.5.6. | 6.4.4.1. |
| C4d2 | The manufacturer has documented his code according to a policy. | Usually at least public class, methods with pass and return values as well as attributes are to be documented |||
| C4d3 | The manufacturer has described which data sets it used for training, validation and testing of the model. |  |ISO 24028 9.8.2.1, DAISAM||
| C4d4 | The manufacturer can reproduce the test and validation results. | For this purpose, it makes sense to use a version management system not only for the code, but also for data, test results and their evaluation. It is advisable to also document the infrastructure used in data processing and training (hardware, operating system, virtualization layers such as Docker). Any deviating results should be justified (e.g., hardware, random generators, rounding errors). Absolute paths and operating system specific commands are to be avoided. |   ISO 13485, 7.3.6., 7.3.3.                      |   6.4.4.2.              |
| C4d5 | The manufacturer has the SOUP (libraries and frameworks) under version and configuration control. | | IEC 62304, 8.1.2. | 6.4.4.3. |
| C4d6 | The manufacturer has documented the architecture of the model and the model itself including its algorithms and hyperparameters. | For example, in the case of a CNN, the number and type of layers, the linkage of the neurons or layers, the activation function, the optimizer and other parameters including their value ranges should be documented, among other things. The documentation of the model also includes the specification of the outputs such as the number of outputs, the respective data types, value ranges, units, etc.. | 2024/1689/EU annex IV section 2. (b) and (c), IEC 62304 5.3, ISO 13485, 4.2.3., 4.2.5. | 6.4.4.4. |
| C4d7 | The manufacturer has described how it selected the architectures, trained the models, and optimized the hyperparameters, and justified this procedure. | Auditors want to be able to understand how the manufacturer has proceeded and why the chosen solution is the best. IEC 62304 and the FDA do not want "ad hoc design decisions".  ||(6.4.4.9)|
| C4d8 | The manufacturer has described when it worked with a “pretrained model” and shown why this “pre-training” is suitable for the task. |                                                              ||6.4.4.5.|
| C4d9 | The manufacturer has documented the quality of the models based on the quality metrics. | These quality metrics relate to the testing with the test data. | ISO 13485, 4.2.3., 4.2.5. | 6.4.4.6. |
| C4d10 | The manufacturer has specified the confidence intervals for the quality metrics depending on the input data. | Especially at the edges of the allowed input data, the confidence often decreases strongly. This information should also be provided to the users in the accompanying materials. ||6.4.4.8.|
| C4d11 | The manufacturer has documented, especially for tabular data, within which limits (e.g. feature values) the model achieves the requirements for the quality measures. | This depends on the applied ML-model and cannot be generally claimed as best practice. |  ISO 13485, 4.2.3., 4.2.5. | 6.4.4.7. |
| C4d12 | The manufacturer has tried out several models and their hyperparameters and documented the aspects mentioned in this section for them. | This documentation serves the manufacturer to compare different models and to justify his choice of a model. This is necessary to fulfill the requirement of ISO 14971 to maximize the risk-benefit ratio. |||

[^C.4.d.1]: Trained models can be serialized.

### 5. Product development

#### a) Software development

| ID                                               | Requirements                                                 | Comments                        | Regulatory references| Team-NB-ID |
| ------------------------------------------------------------ | ------------------------------- |--| ------------------------------------------------------------ | ------------------------------------------------------------ |
| C5a1 | The manufacturer has performed the required activities pursuant to IEC 62304 and documented them. | Notes for auditors[^C.5.a.1] | IEC 62304, IEC 82304-1, XAVIER University "Building Explainability and Trust for AI in Healthcare", FDA guidance on software validation, FDA OTS guidance  | (6.5.1.1.) |
| C5a2 | If the manufacturer has implemented the model in another programming language or for another runtime environment, it has created a plan that repeats the activities pursuant to chapter 4. |  | IEC 62304, IEC 82304-1 | 6.5.1.2. |
| C5a3 | The manufacturer has verified the performance (response times, resource consumption) on the target hardware (e.g. browser, mobile device). | | 2017/745/EU, Annex I, 17.1., 17.3., 2017/746/EU, Annex I, 16.1., 16.3. | 6.5.1.3. |
| C5a4 | The manufacturer has specified the SOUP and OTS requirements. | ISO 25010 provides a list of quality aspects such as performance, IT security, portability and interoperability. | IEC 62304, 5.3, | 6.5.1.5. |
| C5a5 | The manufacturer has described how all SOUP and OTS components are to be verified and has also carried out and documented this verification. | | IEC 62304, 5.3, 8.1.2, FDA OTS Guidance | 6.5.1.4. |
| C5a6 | The manufacturer has attached the prescribed license conditions to the software and ensured the legality of the use of third-party software (e.g., open source software). | Manufacturers often use open source software, which may only be used within the scope of licenses and copy right statements. |||

[^C.5.a.1]: The manufacturers should adhere to the normal best practices such as adherence to coding guidelines, review of code by code reviews using defined criteria, testing to code with unit tests with a defined coverage, etc.  A description of the code (architecture) should make it easy to understand which code performs which task.


#### b) Accompanying materials

| ID                                               | Requirements                                                 | Comments                                                     | Regulatory references| Team-NB-ID |
| ------------------------------------------------------------ | ------------------------------------------------------------ |--|--|--|
| C5b1 | The instructions for use clearly identify the version of the product. | If possible, indicate the UDI. | 2017/745/EU, Annex I, chap. III, 23.1, 23.4., 2024/1689/EU article 13 section 3.(b)(i), FD&C, FDA 21 CFR parts801 and 820.120, ISO 24028 e.g. 10.11.3 | 6.5.2.1 |
| C5b2 | The instructions for use describe the intended use of the product including the expected medical benefit. |   | 2017/745/EU, Annex I, chap. III, 23.1, 23.4., 21 CFR part 801, 21 CFR part 814.20, XAVIER: "Perspectives and Good Practices for AI and Continuously Learning Systems in Healthcare", ISO 24028, XAVIER University "Building Explainability and Trust for AI in Healthcare", ISO 24028 e.g. 10.11.3| 6.5.2.3. |
| C5b3 | The instructions for use specify the intended patient population using indications, contraindications and if relevant using other additional parameters such as age, gender, accompanying diseases. | | 2017/745/EU, Annex I, chap. III, 23.1, 23.4. | 6.5.2.4. |
| C5b4 | The instructions for use explicitly list the patients / data / use case for which the product may **not** be used. |   | 2017/745/EU, Annex I, chap. III, 23.1, 23.4. | 6.5.2.6. |
| C5b5 | The instructions for use document the requirements of the input data (including formats, resolutions, value ranges, etc.). |                                                              |2024/1689/EU article 13 section 3.(b)(vi)|6.5.2.7.|
| C5b6 | The instruction for use specify the intended primary and secondary users pursuant to intended use. | Primary users use the system to achieve the intended medical purpose e.g. to diagnose patients. Secondary use includes installation, update, configuration and administration of the device. | 2024/1689/EU article 13 section 3.(b)(v)| 6.5.2.8. |
| C5b7 | The instructions for use describe the other preconditions applicable to the product (e.g. runtime environment, use environment). |  Runtime environment includes hardware and software prerequisites.  |2024/1689/EU article 13 section 3.(e) and annex IV sections 1.(b) and (e)|6.5.2.10.|
| C5b8 | The instructions for use describe how the product is to be used. | This includes behavior in the event of a problem (e.g. "human oversight") as well as the secondary use such as installation, update, upgrade and configuration as well as management of the audit-logs. |2024/1689/EU article 13 section 3.(d), (e) and (f)|6.5.2.2.|
| C5b9 | The instructions for use describe the possible outputs. | This also includes the explanations by the product ("Explainability"). |2024/1689/EU article 13 section 3.(b)(vii)||
| C5b10   | The instructions for use describe the residual risks.        | Also risk of foreseeable misuse  | 2017/745/EU, Annex I, 23.4, ISO 14971:2019, 8, 2024/1689/EU article 13 section 3.(b)(iii), ISO 24028 e.g. 10.11.3 | 6.5.2.11., 6.6.3. |
| C5b11 | The instructions for use indicate the data with which the model was trained. | This is related both to the patient population and to the features used. ||6.5.2.12.|
| C5b12 | The instructions for use describe the model and algorithms.  |                                                              ||6.5.2.13.|
| C5b13 | The instructions for use name the quality metrics.   |  Also specify confidence ranges here.                                                         | 2024/1689/EU article 13 section 3.(b)(ii)| 6.5.2.14. |
| C5b14 | The instructions for use list the factors that could have a negative effect on the product's performance. |                                                              |2024/1689/EU article 13 section 3.(b)(iii) |6.5.2.15. |
| C5b15 | The instructions for use specify whether the product is further trained during use. | Please observe notes in the chapter on continuous learning systems.  |                                                              |                                                              |
| C5b16 | The instructions for use contain references to additional literature. |                                                              |||
| C5b17 | The instructions for use contain references to licensing rights. |    | 2017/745/EU, Annex I, 23.4, EU-Regulation 207/2012| |
| C5b18 | The instructions for use identify the manufacturer and lists channels for posing questions. |  |  2017/745/EU, Annex I, 23.4, EU-Regulation 207/2012| 6.5.2.17. |
| C5b19 | The instructions for use list possible ethical problems.     | |||
| C5b20 | The instructions for use contain the URL under which the most current versions of the instruction of use can be found. | Different regulations allow, forbid or enforce electronic instructions for use. | 2017/745/EU, Annex I, 23.4, EU-Regulation 207/2012| 6.5.2.18. |


#### c) Usability validation

|ID                                                  |Requirements                                                  |Comments| Regulatory references| Team-NB-ID |
| ------------------------------------------------------------ | --------- |--|--|--|
| C5c1 | As part of the usability validation, the manufacturer assesses whether users understand the instructions for use. | This includes other accompanying materials.  | IEC 62366-1, FDA HFE guidance | 6.5.3.1. |
| C5c2 | As part of the usability validation, the manufacturer evaluates whether the users blindly trust the product or verify the results. | | IEC 62366-1 | 6.5.3.2. |
| C5c3 | As part of the usability validation, the manufacturer evaluates whether users correctly recognize and understand the results. | This also includes the display of errors and the explanations ("explainability"). Manufacturers should include all safety-related use scenarios in the validation and all risk-minimizing measures on the interface. | IEC 62366-1, 5.7-5.9 | 6.5.3.3. |


####  d) Risk management

| ID                                               | Requirements                                                 | Comments | Regulatory references| Team-NB-ID |
| ------------------------------------------------------------ | -------- |--| ------------------------------------------------------------ | ------------------------------------------------------------ |
| C5d1 | The manufacturer has evaluated the risks that arise if the inputs do not meet the specified requirements[^C.2.a.2]. |       |  ISO 14971:2019, 5.4,  IEC 62304, 7.1, DIN SPEC 2, IEC 82304-1 4.1.c) |   |
| C5d2 | The manufacturer has identified and mitigated risks that occur from adversarial attacks | These attacks (typically by subtle manipulations of the input data) are supposed to cause the AI system make wrong predictions such as misclassifications. |  | 6.2.4.6. |
| C5d3 | The manufacturer has derived the quantitative quality criteria based on the state of the art. | The manufacturer shall be able to name the quality criteria for alternative technologies and procedures and to argue if the medical device is not superior to the alternatives with respect to the quality criteria [^C.5.d.1]. | 2017/745/EU Annex 1 1., 2017/745/EU Annex 1 1., 2024/1689 article 8 section 1.| 6.1.4.10. |
| C5d4 | The manufacturer has defined the gold standard and justified its choice, which will be used to verify the quality criteria. |   | XAVIER University "Building Explainability and Trust for AI in Healthcare", FDA proposed regulatory framework for modifications to AI/ML based SaMD: "reference standard" |  |
| C5d5 | The manufacturer has identified, evaluated, and managed risks that arise when outputs do not meet the specified quality criteria. | In this analysis, the manufacturer also considers the specific properties of the selected model as well as the confidence intervals of the output values determined during testing. | ISO 14971:2019, 5.3, IEC 62304, 7.1, IEC 82304-1, 4.1.c), XAVIER University "Building Explainability and Trust for AI in Healthcare", FDA guidance on software validation, 5.2.2, 2024/1689/EU article 9 sections 2.(d) and 5.(a) | 6.1.4.7 |
| C5d6 | The manufacturer has evaluated the consequences if the system provides socially unacceptable outputs (e.g. discriminatory). | These "consequences" are not necessarily risks in the sense of ISO 14971. | Ethics guidelines for trustworthy AI,  2024/1689/EU article 9 2. sections 2.(d) and 5.(a)| |
| C5d7 | The manufacturer has identified, evaluated and managed the risks if the system is not available. |  | 2024/1689/EU article 9 section 2.| 6.1.4.12 |
| C5d8 | The manufacturer has identified, evaluated and managed the risks arising from software errors. | This includes errors in SOUP as well as in the software used for "pre-processing" the data and for training the model. | | |
| C5d9 | The manufacturer has identified, evaluated and managed the risks arising from the specific choice of model architecture. | In doing so, manufacturers should also analyze whether the models have been optimized to the right specifications. | ISO 14971:2019 |  |
| C5d10 | The manufacturer has identified, evaluated, and managed the risks posed by the specific choice of target platform. | For example, the target platform might not provide the required computing power or might cause the software to crash. | | 6.1.4.13 |
| C5d11 | The manufacturer has identified, evaluated and managed the risks arising from the selection of training, validation and test data. | This concerns both the sources of these data (such as patients, institutions) and the division of these data into training, validation and test data. For example, manufacturers should check that there is no overfitting or bias of the results. | 2024/1689/EU article 9 sections 2.(d) and 5.(a), article 10 sections 2.(f), 2.(g), 4. | (6.1.2.5), (6.1.4.11), (6.1.4.14) |
| C5d12 | The manufacturer has identified, evaluated and managed the risks of outputs (predictions, classifications, etc.) being correct only by chance. | Interpretability allows manufacturers to demonstrate why an ML-model has made a specific decision. |||
| C5d13 | The manufacturer has identified the risks posed by the fact that the predictions themselves change the predicted outcomes. | In this phenomenon, the model changes from observer to actor [^C.5.d.2]. It is called "performative prediction." Producers should investigate the possible effects on people or systems and describe them e.g. with a DAC ("directed acyclic graph"), observe a possible "distribution shift" and, if necessary, an unaffected control group, and take action if necessary such as choosing a different model or re-training the existing model. | 2024/1689/EU article 15 section 4.| 6.1.4.17 |
| C5d14 | If the manufacturer uses self-tests, he has explained which of the specified quality criteria are checked with them and which risks are thereby controlled. | These self-tests correspond to a mean of risk mitigation. |||
| C5d15 | The manufacturer has identified, evaluated and managed the risks from use errors caused by problems with perception. | These problems can be caused by complex user interfaces, new input modalities, new or additional information (leading to a cognitive overload).| IEC 62366-1, 5.3f, FDA HFE guidance, FDA guidance on software validation, 5.2.3, UK 811.4 Position Paper  | (6.1.4.17)  |
| C5d16 | The manufacturer has identified, evaluated and managed the risks from use errors caused by problems with cognition. | Examples are cognitive overload, a lack of situational awareness, a lack of awareness of limitations of the system, a confirmation bias, a mismatch of the mental model, overtrust and mistrust. | IEC 62366-1, 5.3f, FDA HFE guidance, FDA guidance on software validation, 5.2.3, UK 811.4 Position Paper | (6.1.4.17)  |
| C5d17 | The manufacturer has identified, evaluated and managed the risks from use errors caused by the explanations on the user interface or in the instructions for use. | "Explainability" can be a measure for risk mitigation, but can cause new use errors itself. | IEC 62366-1, 5.3f, FDA HFE guidance, FDA guidance on software validation, 5.2.3 | (6.1.4.17) |
| C5d18 | The manufacturer has identified, evaluated and managed the risks from wrong, delayed or missing actions by the user. | E.g., AI systems can cause fear / hesitation and thereby delayed actions or a lack of action due to overtust in the system. |UK 811.4 Position Paper||
| C5d19 | The manufacturer has identified, evaluated and controlled the other risks mentioned in chapter C.1.d). |   |||
|C5d20 |The manufacturer has evaluated "human oversight" as one risk mitigation measure and documented the decision. |Users can intervene e.g., press a kill-switch.| 2024/1689/EU article 14 and Annex IV section 2.(e)| |
|C5d21|The manufacturer has analyzed the records according to 2024/1689/EU for risks.| This is also a post-market surveillance duty. |2024/1689/EU article 9 section 2.||

[^C.5.d.1]: State-of-the-Art does not necessarily correspond to the Gold Standard, which in turn does not necessarily correspond to the Ground Truth. I.e., the system requirements may be lower than for a gold standard or ground truth, especially if the latter requires an invasive or very costly procedure.    
[^C.5.2.d]: Examples of this phenomenon can be found [here](https://mindfulmodeler.substack.com/p/correction-you-can-break-a-predictive).  

#### e) Clinical evaluation, performance evaluation

|ID                                                  |Requirements                                                  |Comments| Regulatory references| Team-NB-ID |
| ------------------------------------------------------------ | --------- |--| ------------------------------------------------------------ | ------------------------------------------------------------ |
| C5e1 | As part of the clinical / performance evaluation, the manufacturer has evaluated whether the promised medical benefit is achieved for the given quality parameters. || 2017/745/EU, Article 61, Annex XIV and Annex XV, 2017/746/EU, Annex XIII and Annex XIV, MEDDEV 2.7/1 rev.4, XAVIER University "Building Explainability and Trust for AI in Healthcare", FDA 21 CFR part 820.30(g)| 6.5.4.1. |
| C5e2 | As part of the clinical / performance evaluation, the manufacturer has evaluated whether the promised medical benefits and risks are in line with the state of the art. | | 2017/745/EU, Article 61, Annex XIV and Annex XV, 2017/746/EU, Annex XIII and Annex XIV, MEDDEV 2.7/1 rev 4, ISO 14971:2019, 4.2  | 6.5.4.2. |
| C5e3 | The manufacturer has specified the PMCF / PMPF requirements. | | 2017/745/EU, Article 61 (11), 2017/746/EU, Article 56 (6, | 6.5.4.4. |


### 6. Product release

|ID                                                  |Requirements                                                  |Comments| Regulatory references| Team-NB-ID |
| ------------------------------------------------------------ | --------- |--|--|--|
| C6.1 | The manufacturer has ensured that all the above documentation is available. | This concerns, among other things, the documentation required in chapters 3.d), 4.d and 5.b). | 2017/745/EU, Annexes I and II, ISO 13485 e.g. 7.3.5, FDA 21 CFR part 820.30(e) | (6.6.1) |
|C6.2|The manufacturer has identified the software version in the documentation.|| 2024/1689/EU annex IV section 1.(c)| |
| C6.3 | The manufacturer has assessed the risks as acceptable in risk management and documented that all activities specified in the risk management plan have been carried out. | Note for auditors [^C.6.1] ||6.6.2.|
|C6.4 |The manufacturer has outlined in the Software as a Medical Device Pre-Specifications (SPS) what types of changes it anticipates for systems that it wishes to market in the USA[^C.6.2]. | | 2024/1689/EU annex IV section 2.(f), FDA |  |
| C6.5 | The manufacturer has shown in Predetermined Change Control Plan (PCCP) how it will perform these changes for systems that it wishes to market [^C.6.3]. | |2024/1689/EU annex IV section 2.(f), [FDA PCCP Guidance](https://www.fda.gov/regulatory-information/search-fda-guidance-documents/marketing-submission-recommendations-predetermined-change-control-plan-artificial-intelligence)||
| C6.6 | The manufacturer has created a Post-Market Surveillance Plan, see below. |                            |||

[^C.6.1]: Using examples, check that the efficacy of risk management measures was tested so that there is a traceability of risks to risk control measures.

[^C.6.2]: Changes may affect the intended use, the input data and the clinical and analytical performance.

[^C.6.3]: The approach must, for example, address handling data, re-training, the performance and the updates.

## D) Requirements for the phases downstream of development

### 1. Production, Distribution, Installation

|ID|Requirement|Comments| Regulatory references| Team-NB-ID |
|:--|:--|:--|---|:--|
|D1.1|The manufacturer has described how it ensures that only exactly the intended artefacts (files) in exactly the intended version of the product or as a product are delivered.|This is configuration management. Also relevant to downloads or App <Stores.| IEC 62304, 5.8.8. | 7.1.1. |
|D1.2 |The manufacturer has described how the persons responsible for the installation know which is the latest version and how confusion during installation can be ruled out. |This is only relevant for stand-alone software. Here, a procedure or work instruction would be expected.| ISO 13485, 7.8.3., 8.3.,  IEC 62304, 5.8.4. | 7.1.2. |
|D1.3|The manufacturer has described how it will be ensured during installation that the requirements specified in the accompanying materials (see above) are actually met.|A SOP or work instruction would be expected here.| ISO 13485, 7.5.3. | 7.1.3. |
|D1.4|The manufacturer has established procedures that ensure that it can communicate with the operators and users of its product in a timely manner.|| ISO 13485, 7.2.3., 8.3.3., IEC 82304-1, 8.4. | 7.1.4. |


### 2. Post-Market Surveillance

|ID|Requirements|Comments| Regulatory references| Team-NB-ID |
|:--|:--|:--|---|:--|
|D2.1|The manufacturer has created a Post-Market Surveillance (PMS) Plan.|| 2017/745/EU, Chapter VII, 2017/746/EU, Chapter VII, 2024/1689/EC article 17 section 1.(h), article 72 | 6.6.4., 7.2.1. |
|D2.2|The manufacturer has specified the data it wishes to collect and analyze in this PMS plan.|| 2017/745/EU, Chapter VII, 2017/746/EU, Chapter VII | 7.2.2. |
|D2.3 |The manufacturer has specified in the PMS plan, that logging information is collected analyzed |This information are the "automatically generated logs" according to 2024/1689/EC|2024/1689/EC article 12 section 2.(b)||
|D2.4|The manufacturer has specified in the PMS plan the quality criteria and threshold values that it considers necessary for handling of in particular a re-evaluation of the risk-benefit analysis.|| 2017/745/EU, Chapter VII, 2017/746/EU, Chapter VII | 7.2.3. |
|D2.5|The manufacturer has analyzed when determining these threshold values which feedback loops the threshold values can influence[^D.2.1].|This analysis also serves as a measure against the above risk through "Performance Prediction".| 2017/745/EU, Chapter VII, 2017/746/EU, Chapter VII |  |
|D2.6|The manufacturer has analyzed when determining these threshold values which self-fulfilling prophecies the threshold values can influence[^D.2.2].|| 2017/745/EU, Chapter VII, 2017/746/EU, Chapter VII |  |
|D2.7|The manufacturer has described in the PMS-plan how it collects and analyzes information on adverse medical effects.|| 2017/745/EU, Chapter VII, 2017/746/EU, Chapter VII | 7.2.4. |
|D2.8|The manufacturer has described in the PMS-plan which information on (adverse) behavioral changes or (predictable) misuse is collected and analyzed[^D.2.3].|| 2017/745/EU, Chapter VII, 2017/746/EU, Chapter VII, 2024/1689/EC article 9 section 2.(b) | 7.2.5. |
|D2.9|The manufacturer has described in the PMS-plan how it collects and analyzes information on additional “adverse effects” [^D.2.4].|| 2017/745/EU, Chapter VII, 2017/746/EU, Chapter VII | 7.2.6. |
|D2.10|The manufacturer has described in the PMS-plan how it collects information to be able to analyze whether the data in the field is consistent with the expected data or training data[^D.2.5].|Note for auditors[^D.2.6]| 2017/745/EU, Chapter VII, 2017/746/EU, Chapter VII | 7.2.7. |
|D2.11|The manufacturer has described in the PMS-plan how and how often it wants to collect information on whether the product still meets the state of the art.|Note for auditors[^D.2.7]| 2017/745/EU, Chapter VII, 2017/746/EU, Chapter VII | 7.2.8. |
|D2.12|The manufacturer has described in the PMS-plan how and how often it wants to collect information on whether the “Ground Truth” or the gold standard are still up to date.|| 2017/745/EU, Chapter VII, 2017/746/EU, Chapter VII | 7.2.9. |
|D2.13|The manufacturer has described in the PMS-plan how and how often changes are made e.g. pursuant to the Pre-determined Change Protocol (PPRP).|| 2017/745/EU, Chapter VII, 2017/746/EU, Chapter VII, [FDA PCCP Guidance](https://www.fda.gov/regulatory-information/search-fda-guidance-documents/marketing-submission-recommendations-predetermined-change-control-plan-artificial-intelligence) |  |
|D2.14|The reports required by the plans are available at the times specified therein.|e.g. PSUR, SSCP|2017/745/EU article 85 f., 2017/747EU article 80 f.|7.2.10.|

[^D.2.1]: Examples for these feedback loops: **Example 1**: A travel recommendation app sends targeted advertising depending on feature (last trip). This influences travel behavior. **Example 2**: An algorithm provides prognoses. Therefore, the physician will treat the patients better or earlier...

[^D.2.2]: Example 1 (criminalistics)

[^D.2.3]: Example: Radiologists rely on the software and don't look at the images anymore, so they overlook findings.

[^D.2.4]: Examples would be ethical challenges such as the YouTube algorithm, which achieves the goal, maximizing the click count or use duration, but promoting violence and conspiracy videos.

[^D.2.5]: One speaks here of a distribution shift or data drift.

[^D.2.6:]: The manufacturer should set threshold values for features or for the variance / covariance over time. This allows visualization or quantification in particular for non-normally distributed data over the comparison of histograms or core density estimations.

[^D.2.7]: For example, have the manufacturer explain the process on how it is systematically informed of new developments in machine learning, and how it assesses these developments and reacts to them.



### 3. Decommissioning


|ID|Requirements|Comments| Regulatory references| Team-NB-ID |
|:--|:--|:--|---|:--|
|D3.1 |The manufacturer has created a decommissioning plan before withdrawing its product from the market. | Such a plan specifies, for example, whether and how the software must be uninstalled, whether data must be backed up or exported, how the confidentiality of the data remains guaranteed, who is responsible for these activities, how the progress of the decommissioning is monitored and ensured, and which organizations must be informed and how.| ISO 24028 | 7.3.1 |
|D3.2 |The manufacturer has identified, evaluated and controlled the risks arising from decommissioning. | This is to be evaluated in the risk management file. Risks from the unavailability of the product, from usage errors and from an influence on other products should be considered.|  2017/746/EU Annex I, 3., ISO 14971:2019 chapter 10 in combination with 3.8 and 3.12, ISO 24028 | 7.3.2. |


## E) Annexes

### 1. Additional literature

#### a) Laws

- [Medical Device Regulation](https://eur-lex.europa.eu/legal-content/DE/TXT/?uri=uriserv:OJ.L_.2017.117.01.0001.01.DEU&toc=OJ:L:2017:117:FULL) MDR
- [In-vitro Diagnostic Device Regulation](https://eur-lex.europa.eu/legal-content/DE/TXT/?uri=uriserv:OJ.L_.2017.117.01.0176.01.DEU&toc=OJ:L:2017:117:FULL) IVDR
- [Artificial Intelligence Act](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202401689) (AI Act)

#### b) Standards and Best Practice Guides

- **IEC 62304/AMD1**, Medical device software – Software life cycle processes
- **IEC 82304-1**, Health software – Part 1: General requirements for product safety
- [FDA Guidance Documents on Machine Learning](https://www.fda.gov/medical-devices/software-medical-device-samd/artificial-intelligence-and-machine-learning-software-medical-device)
- [FDA Guidance "Marketing Submission Recommendations for a Predetermined Change Control Plan for Artificial Intelligence-Enabled Device Software Functions"](https://www.fda.gov/regulatory-information/search-fda-guidance-documents/marketing-submission-recommendations-predetermined-change-control-plan-artificial-intelligence)
- [A Position Paper of DKE UK 811.4 "Usability Engineering for Medical Devices using Artificial Intelligence and Machine Learning Technology"](https://doi.org/10.5281/zenodo.14203190)

#### c) Industry literature, textbooks

- Christoph Molnar: [Interpretable Machine Learning](https://christophm.github.io/interpretable-ml-book/)
- Patrick Hall: [Machine Learning Interpretability
  with H2O Driverless AI](http://docs.h2o.ai/driverless-ai/latest-stable/docs/booklets/MLIBooklet.pdf)
- Patrick Hall: [On the Art and Science of Machine Learning Explanations](https://arxiv.org/pdf/1810.02909.pdf)
- Johner Institute: [Video training on machine learning for medical products](www.auditgarant.de)

#### d) Sources and checklists for reproducibility

- https://www.cs.mcgill.ca/~jpineau/ReproducibilityChecklist-v2.0.pdf
- https://epub.ub.uni-muenchen.de/92151/1/92151.pdf
- https://github.com/craig-willis/reproducibility-checklist/
- https://2020.emnlp.org/call-for-papers#new-reproducibility-criteria
- https://onlinelibrary.wiley.com/pb-assets/assets/15214036/RR_Guideline.pdf

### 2. Recitals

1. Manufacturers are increasingly developing medical products that use the process of artificial intelligence, in particular machine learning. Many of these procedures are still very new, and lack best practices. This creates new risks for patients, users and third parties.
2. The EU directives (MDR, IVDR) explicitly require the safety of the products in the relevant annexes I. Bu concrete requirements for these classes of products are completely lacking. Therefore, both the manufacturers and the notified bodies and authorities lack concrete guidelines on how to evaluate the safety of the products.
3. Contrary to most other fundamental requirements, no standards on the subject of AI are harmonized. Therefore, there is no canonical catalog of requirements that reflects the recognized state of the art of technology.
4. The FDA has started to formulate requirements on using Continuous Learning Systems, CLS. These specifications are unsuitable to sufficiently set requirements for the products and processes as early as the product development stage.
5. The safety of medical products must be considered in all phases of the product life cycle processes. A limitation to testing is insufficient. This fact must be in line with best practices and guidelines.
6. One hopes that standards for the safety of AI-based medical products will be developed and harmonized. This will still take years. Therefore, we need a guideline (only) in this interim phase.
7. This guideline should be available very soon (by July 2019) to be able to quickly serve the manufacturers as an orientation and enable them to act immediately. The high speed of development makes compromises regarding harmonization with the most parties possible inevitable.
8. The technological advancement in the area of artificial intelligence is immense. New procedures and technologies are continuously being published. On the one hand, a guideline should be a specific as possible. On the other, it cannot be so specifically targeted toward one procedure or technology, to achieve a sensible “shelf life”. Therefore, a guideline must address general concepts. However, it cannot claim to be complete.
9. Such a guideline must take into consideration the specifics of medical products, which includes the principles of patient safety (safety) and a risk-based approach. In a concrete case, selected actions for information security ("controls”) will be in conflict with the fundamental requirements. For this reason, there can be no set list of “controls” for medical products. The manufacturer's intended use of the product is critical.
10. The simple intelligibility and practicability is essential to the desired positive influence of a guideline on the safety of AI-based medical products. Therefore, there must be the least abstract or “high level” requirements possible but “binary decisive” test criteria.
11. To increase practicability, the authors have avoided collating many requirements to the greatest extent possible. Rather, they have limited themselves to those that they consider particularly relevant and implementable.
12. Additionally, to promote distribution and the level of familiarity, the guideline must be available and remain available at no cost.
13. The guideline should be available in German and English.
