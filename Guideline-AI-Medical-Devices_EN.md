# Guideline for AI for medical products

## A) Meta information

### 1. Objective of the guideline

The objective of this guideline is to provide medical device manufacturers, authorities and notified bodies instructions and to provide them with a concrete checklist to

- understand what the expectations of the notified bodies and authorities are,
- to promote step-by-step implementation of safety of medical devices, that implement artificial intelligence methods, in particular machine learning,
- to compensate for the lack of a harmonized standard (in the interim) to the greatest extent possible.

The guideline is **not** meant to serves as a training manual or guideline to achieve the safety of AI based medical devices. It is to be a guideline for its review.

The annex lists the recitals which led to the development of this guideline.

### 2. Scope of applicability and target group.

This guideline is only applicable to medical devices that use AI methods, in particular machine learning. The guideline applies in particular to

- Manufacturers of these products
- Their service providers (such as engineering providers)
- People and organizations that must assess the safety of these products, such as auditors, authorities and notified bodies.

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

Much more, the guideline brings together best practices to best describe the required “state-of-the-art”.

Some of these best practices are not applicable in all situations, for all products or for all methods of machine learning. The manufacturers should at least justify non-obvious exclusions.

#### c) Use of the guideline

##### Creating and reviewing specifications

The manufacturers should first use the guideline to review the completeness of the specifications (process and work instructions, checklists, etc.). These tasks are normally assumed by the following roles:

- Process-related persons, in particular head of development
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

- Clear ID
- Review criteria, that can be simply assessed as met or not met
- Comments

The comments may contain:

- Note or reference to regulatory requirement
- Recommendations for implementation of reference to additional explanations
- Tips for auditors such as how the fulfillment of the criteria can be assessed
- Notes on binding nature and applicability and limitations

### 4. Authors and rights of use

The following authors created this guideline:

- Prof. Dr. Christian Johner ([Johner Institute](https://www.johner-institut.de))
- [Christoph Molnar](https://christophm.github.io/) ([LMU Munich](https://www.uni-muenchen.de/index.html))
- Dr. Andreas Purde, Dr. Abtin Rad ([TÜV SÜD](https://www.tuev-sued.de/))
- Prof. Dr. Christian Dierks ([Dierks + Company](https://www.dierks.company/))
- Stefan Bunk (CTO) and Sven Piechottka (Government & Regulatory Affairs) ([Merantix](https://www.merantix.com/healthcare/))

The guideline is published under the ([Creative Commons License](https://creativecommons.org/licenses/?lang=de)) of type [BY-NC-SA](https://creativecommons.org/licenses/by-nc-sa/4.0/). This requires a list of names of authors (“Christian Johner, Christoph Molnar et al.”) and allows third parties to build on this work, e.g. to correct it; however only for non-commercial purposes.

The license permits using the product for commercial consultancy purposes including audits and reviews. It is prohibited, however, to use this work itself in an unchanged or changed version for commercial purposes, e.g. in the form of sale as a brochure.

### 5. Document handling, document identification

This document is managed via the version management system git or the GitHub platform. Only the documents listed in this repository are valid.

The version history, including any authors may be found in the document history.

The released versions are labeled via one day as such in the repository. Versions without a tag are documents in the draft stage.

## B) General requirements

### 1. Process requirements

The manufacturers should cover all aspects listed below either in the procedural instructions or in the relevant plans to ensure that the safety of the product is systematically guaranteed. Normally, the following standard operating procedures or plans are affected:

- Development
- Risk management
- Data management
- Verification or validation (if not part of development)
- Post-market surveillance and vigilance
- Service, installation, decommissioning
- Customer communication
- Management review (ISO 13485:2016 requires consideration of “applicable new or revised regulatory requirements”.)

If the manufacturer outsources processes, the requirements apply accordingly. Examples would be a (software) development service provider or contract research organization to be required to consider the relevant chapters of this guideline.

### 2. Plans

The manufacturer should compile all product specific plans as required by respective regulations.

- Development plan (incl. verification and validation planning)
- Post-market surveillance plan
- Risk management plan
- Clinical evaluation plan

### 3. Competency requirements

The manufacturers must ensure and prove that they have sufficient competencies to ensure the relevant safety and performance of the products according to the state of the art. This proof is often gained most easily through internal or external training.

Manufacturers can use the competency of external resources.

|Requirements|Comments|
|:--|:--|
|The manufacturer has created a list of all roles inside the scope of its QM system that are directly or indirectly concerned with AI. [^B2-01]||
|The manufacturer has documented the competency requirements for each role inside the scope of its QM system that is directly or indirectly concerned with AI. [^B2-02]|Competencies are related to education, knowledge or skill. Examples of competencies: Machine learning, explainable AI, medicine (for relevant domains), clinical and usability validation.|
|The manufacturer has appropriate records for the training, further education and competencies that allow for the conclusion that the persons actually have these competencies.||
|The (software) development plans have defined the product-specific competencies (beyond or deviating).|Requirements of ISO 13485:2016|

[^B2-01]: Examples are: Data Scientists, Developers, Testers, Regulatory Affairs and Quality Mangers, Service and Support Employees, Product Managers, Medical Device Consultants, Physicians

[^B2-02]: Competencies (level if understanding, capability to perform tasks) should be listed, not primary subjects

### 4. Documentation

The manufacturers should keep evidence that they have followed the relevant requirements of this guideline. There are no specific requirements for documentation and “objective evidence”.

In Europe at least, there is no obligation to create a specific document that summarizes the activities especially for AI. Manufacturers can integrate these aspects into existing documents such as QM documents (e.g. standard operating procedures, work instructions) and the technical documentation (e.g. software files, risk management files, clinical evaluation, summative evaluation of the usability).

## C) Requirements for product development

### 1. Intended use and stakeholder requirements

#### a) Intended medical use

|Requirements|Comments|
|:--|:--|
|The manufacturer has determined for which medical purpose (diagnosis, therapy, monitoring, predictions) the medical product should support.|The intended use / purpose should not be mistaken for the description of functionality (e.g. calculation of scores).|
|The manufacturer has characterized the patients to be diagnosed, treated or monitored with the medical product. This characterization includes patient demographics, indications, contraindications and associated diseases.|This characterization is also included in IEC 62366-1. Patients may also simultaneously be users of the product.|
|The manufacturer has specified on which body locations the product will be used or from which body location the data originate.|Also called for in IEC 62366-1 clause 5.1.|
|The intended use also suggests what the goal of machine learning techniques is.|Classification and regression, clustering, similarity search and recommender systems are typical goals of machine learning methods. The description of the role of machine learning is necessary to fulfill the requirement for the description of the "physical principle".|
|The manufacturer has determined the intended lifetime of the medical device.|This lifetime is determined, for example, by the state of the art (e.g., medical advances, new ML-methods, competitive products) and the speed at which the technical environment and libraries evolve.|


#### b) Intended users and context of use

| Requirements                                                 | Comments                                                     |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| The manufacturer has characterized the intended users, e.g. using demographic features (age, gender), regarding the training, experience in medical domains, regarding technical knowledge, physical and mental limitations, linguistic skills and cultural background. | If the manufacturer does not foresee any limitations regarding these attributes, it must document this. |
| The manufacturer has characterized the intended use environment (also social environment such as stress, shift work, frequently changing colleagues)| This characterization is also required by IEC 62366-1. It is also relevant in the context of the explainability of AI. |
|The manufacturer has described the core tasks that the medical device is to support. | The use scenarios that manufacturers must specify according to IEC 62366-1 can also be derived from these core tasks.|


#### c) Stakeholder requirements

| Requirements                                                 | Comments                                                     |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| The manufacturer has operationalized the goals listed in the intended use with quantitative values [^C.1.c.1]. | It is not unusual that these values are supplemented and revised during the course of development. |
| The manufacturer has set forth the runtime environment of the product regarding hardware (screen size, screen resolution, storage, network connection etc.) and software (e.g. operating system, browser, runtime environments such as Java runtime environment or .NET). | For apps, this characterization must be done for the app and for the server part. |
| The manufacturer has specified the data interfaces using the levels of the [interoperability model](https://www.johner-institut.de/blog/tag/interoperabilitat/) and set forth the formats and for images, their specific properties (size, resolution, color coding). | This is required pursuant to IEC 62304 chapter 5.2.2. |
|The manufacturer has specified the requirements for the input data. | The input data may also depend on the generation of the data, e.g. on the recording method, on technical parameters (magnetic field strengths, number of conductive electrodes, direction), on environmental conditions during the recordings, on the manufacturer, on the medical device, etc.... 
| The manufacture has set forth all markets and all regulatory requirements relevant to these. | Show this list.  
|The manufacturer has specified whether the system should continue to learn after it has been placed on the market. If this is the case, the manufacturer has specified whether this continuous training will be global/centralized or decentralized (e.g., per product or per hospital) and online or offline. | 

[^C.1.c.1]: **Example**: Purpose: The software supports radiologists in diagnosing cancers using CT images of the head. Quantitative value: 95% of radiologists working with software detect the cancer.


#### d) Input for risk management and clinical evaluation

| Requirements                                                 | Comments                                                     |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| The manufacturer has listed alternative procedures and evaluated them in terms of benefit, safety, and performance. | The discussion of the state-of-the-art is a requirement of MEDDEV 2.7/1 and the MDR/IVDR. |
| The manufacturer has compared the aforementioned quantitative values with the relevant values of alternative methods. | Manufacturers should create a tabular overview.              |
| The manufacturer has justified why machine learning is superior to the other methods and thus justified the associated risks. |                                                              |
|The manufacturer has drawn up a list of risks specifically arising from the application of machine learning methods. | Is part of the risk management file |                                                                                                                                                    
|The manufacturer has analyzed the risks that arise when patients other than those specified are diagnosed, treated, or monitored with the product. |    |
| The manufacture has analyzed the risks arising if persons other than the specified users, use the product. |                                                              |
| The manufacturer has analyzed the risks arising through use in an environment different than that specified. |                                                              |                                                         |
| The manufacturer has analyzed the risks arising from inputs not in the specified format. |                                                              |                                                             |                                                             |
| Manufacturers have analyzed risks arising from data not generated according to the specified prerequisites. |                                                              |
|The manufacturer has assessed the risks when the system is used in a patient population other than that specified. |


### 2. Software requirements

#### a) Functionality and performance

|Requirements|Comments|
|:--|:--|
|The manufacturer has comprehensibly derived quantitative quality criteria or requirements for the software or/and the algorithm from the intended purpose [^C.2.a.1].|This comprehensibility can be represented particularly well with a traceability matrix.|
|The manufacturer considered for example the following quantitative quality criteria or requirements: for classification problems, accuracy (Mean or Balanced Accuracy), positive predictive value (Precision), specificity and sensitivity; for regression problems, Mean Absoute Error and Mean Square Error.| For unbalanced data, i.e. when labels occur with very different frequencies, Balanced instead of Mean Accuracy should be used. However, the choice of quality criteria depends strongly on the intended use. |
|The manufacturer has specified the expected value ranges of the outputs.||
|The manufacturer has specified the requirements regarding repeatability and reproducibility of requirements.|This is particularly relevant with "Continuous Learning Systems".|
|The manufacturer has specified how the system will behave if the inputs do not meet the specified conditions [^C.2.a.2].|This is an aspect of robustness to be specified according to ISO 25010 and IEC 62304 Chapter 5.2. |
|The manufacturer has determined which self-tests the system must perform and how it behaves if this is not successful.|This is particularly relevant for "Continuous Learning Systems".|
|The manufacturer has determined how fast the system must create the outputs.|This determination may be done depending on the size and amount of data.|
|The manufacturer has specified the availability of the medical device.|This is an aspect of robustness and must be specified pursuant to ISO 25010 and IEC 62304 chapter 5.2.|

[^C.2.a.1]: Examples:  **Example 1**: The stakeholder requirement states that 95% of radiologists must be able to detect a cancer with the product. The requirement of the algorithm states that it must display a sensitivity of 97%. **Example 2**: The stakeholder requirements state that arterial calcification must be able to be detected at a sensitivity of 92%. The requirements of the algorithm state that it must be able to exactly predict the strength of the plaques in the blood to 0.2 mm.

[^C.2.a.2]:  Examples: incomplete data sets, lack of data sets, wrong data format, excessive data quantities, data outside of specified value ranges, wrong temporal sequence of data.

#### b) User interface

| Requirements                                                 | Comments                                                     |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| The manufacturer has specified what the user interface must display when the preconditions are not met[^C.2.a.2] in order to operate the system safely (e.g., inputs not valid or not expected). |                                                              |                                                          |
| The manufacturer has specified what the user interface must display if the output does not meet the specified quality criteria. |                                                              |
| The manufacturer has determined whether instructions for use and training materials are required. | The MDR / IVDR allow exceptions to the obligation. |

#### c) Additional software requirements

| Requirements                                                 | Comments                                    |
| :----------------------------------------------------------- | :------------------------------------------ |
| The manufacturer has set forth which requirements the system must fulfill to detect internal system errors. | Could be an audit log or a monitoring port. |
| According to the GDPR, the specified system must not expose patients to decisions based exclusively on automatic data processing. Manufacturers should address the corresponding requirement and be able to justify the chosen legal basis. | Requirement of Art. 22 of the GDPR.  |                                             |
| The manufacturer has determined the requirements that the software must meet in order to ensure the IT security of the product. | IT security is not the subject of this guideline, but the [IT-Sicherheits-Leitlinie](https://github.com/johner-institut/it-security-guideline/).  |



#### d) Special requirements for continuous learning systems

| Requirements                                                 | Comments                                                     |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| The manufacturer has defined when and how often the model is updated. | For this purpose, the manufacturer should define the "triggers" of these updates. He must also describe whether these updates take place per individual medical device or for all medical devices of the type.  |                                                              |
| The manufacturer has specified how the additional data will be quality assured and how incorrect, missing or implausible data will be dealt with. |   
| The manufacturer has defined in which range the output data may change. | This requires a description of how the algorithms change.  |  
| The manufacturer has described how it continues to ensure the correctness and accuracy of the output data and what happens if this can no longer be guaranteed. | Self-checks, the possibility of roll-backs, limiting outputs are possible approaches. |
|The manufacturer has described whether and how users are informed about changes to the algorithm and whether they can decide about them. | |
|The manufacturer has identified and managed the specific risks arising from continuous learning. | To this end, the manufacturer must justify that it achieves a better risk-benefit ratio through continuous learning. |

[^C.2.d.1]: The state-of-the-art of technology is not necessarily consistent with the state of science and thus the gold standard nor with the “Ground Truth”. This means that the system requirements are lower than with a gold standard respectively the "Ground Truth". This would be the case in particular if the latter require an invasive or very cost-intensive procedure.

### 3. Data Management

Data generally have to be understood as training, validation and test data. Each type has to fulfill specific requirements. If not specified differently, however, the usage of the term "data" relates in the following to all three types.

#### a) Data collection

| Requirements                                                 | Comments                                                     |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| The manufacturer has specified quality control of data.      | This includes a list of allowed / expected data sources, specification of data source requirements and a description how invalid  data are identified and excluded. |
| The manufacturer has set the number of data sets and given a reason why this is sufficient[^C.3.a.1]. |                                                              |
| The manufacturer has characterized the inclusion and exclusion criteria of individual patients using relevant attributes[^C.3.a.2]. | For example: demographic attributes (age, gender), diseases, vital parameters, ... |
| The manufacturer has specified the technical inclusion and exclusion criteria for data[^C.3.a.3]. | For example: Data ranges, types, unit of measure, precision, file formats, encodings, image parameters, language, ... |
| The manufacturer has specified the timeframe within which data have to be collected, if applicable. |                                                              |
| The manufacturer has described the procedure by which it ensures that data sets that do not meet the inclusion criteria or should be excluded are actually excluded. | Procedure includes a software supported assessment. This software must be validated. |
| The manufacturer has described the collected data using descriptive statistics[^C.3.a.4]. | The ["Dataset Nutrition Label"](https://ahmedhosny.github.io/datanutrition/) is an recommended option. |
| The manufacturer has justified where the data are collected and why these are representative for the target population. As reasonable, these have been compared to scientific publications and to registers. |                                                              |
| The manufacturer has listed and discussed factors that could cause a bias in the data. |                                                              |
| The manufacturer has analyzed which influences the type and location of data collection have on the data[^C.3.a.5]. |                                                              |
| The manufacturer has examined and excluded the possibility of a “label leakage”[^C.3.a.6]. | This depends on the applied ML model is not a general best practice. |
| The manufacturer that uses surveys has justified the selection of the surveys, the time of survey and possibly the method for their assessment, in particular if no standardized survey exists. |                                                              |
| The manufacturer has specified a patient data protection policy. |                                                              |
| This data protection policy describes the roles including their type of access and data rights (create, delete, change read). |                                                              |
| This data protection policy  describes how to decommission data. |                                                              |
| This data protection policy describes the method by which data are anonymized or pseudonomized before testing and training. |                                                              |
| The manufacturer has ensured that data scientists have no access to protected data. |                                                              |
| The manufacturer has appointed a data protection officer.    |                                                              |
| The manufacturer has received ethical approval (e.g. for genetic data), if legally required. |                                                              |

[^C.3.a.1]: A specification for the number of data is hardly possible. This depends on the “signal-noise-ratio” among other things. For example, for one data set, the percentage of relevant genes and the strength and frequency of the predicted effects affect the number. For data to be classified, the number of the data sets with the rare class (e.g. the prevalence of diseases) is decisive.

[^C.3.a.2]: e.g. demographic data (age, gender), physical parameters (height, weight), diseases, vital parameters, lab parameters, presence of additional tests, case history.

[^C.3.a.3]: Examples: **Example 1**: Patients who must be ruled out due to a heart pacemaker or lung surgery because the images cannot be analyzed or could lead to erroneous classification. **Example 2**: Formats and technical parameters such as image sizes, resolution, brightness and contrasts, color coding, compression, recording equipment, recording method (e.g. CT versus MRI), with or without contrast agent, zoom. **Example 3**: Completeness of meta-data.

[^C.3.a.4]: Usually, the calculation of distributions (histograms), mean / average values, quartiles, possibly “joint distribution of features". The correlation of data among that data should be examined. Additional examples are found in the [publication by Sarah Holland et al.](https://arxiv.org/pdf/1805.03677.pdf) (such as in table 1)

[^C.3.a.5]: Examples: Influence of various measurement devices, surveys, policies (such as a clinic only takes lab parameters only in emergencies, another routinely. Frequency and reason examined with the patient), type of clinic (e.g. small hospital, from which all serious cases must be referred versus university hospital > survivor basis), self-selection bias (e.g. patients with various pre-existing conditions usually go to a hospital rather than a medical practice), type of study (prospective versus retrospective)

[^C.3.a.6]: These are data in which non-causal information are found in the data via the label, e.g. in the sorting (e.g. first the data of healthy persons, then of ill persons), in the hospital (from one the severe cases originate), in images (e.g. for skin cancer, one must always see a ruler). An additional example would be multiple CT images of a patient, in which the model learns using the patient and not the disease. This could happen if a rib fracture can be seen in addition to the cancer on multiple images.

#### b) Data annotation

| Requirements                                                 | Comments                                                     |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| The manufacturer using “supervised learning” has derived the labels from the intended use and justified this selection. |                                                              |
| The manufacturer using “supervised learning” has described how the ground truth is derived. |                                                              |
| The manufacturer using "supervised learning"  has specified a procedure to ensure correct labelling. |                                                              |
| This procedure specifies and justifies the quantitative classification / segmentation criteria for data annotation. |                                                              |
| This procedure specifies how and how frequently the correctness of the labelling is monitored. |                                                              |
| The procedure specifies how to deal with inconsistency of data annotation from multiple annotators. |                                                              |
  | This procedure specifies the data format and/or syntactic and or standards (e.g. coding system) for annotations. |                                                              |
| This procedure specifies quantitative classification criteria for labeling. The selection of these criteria has been justified by the manufacturer[^C.3.b.1]. | If the "Ground Truth” is not selected[^C.3.b.2], because it is too expensive or invasive, this must also be justified. |
  | This procedure specifies a detailed instruction for the task including background information and prototypical examples. |                                                              |
| This procedure specifies the requirements for the number, training and competency for the people responsible for labeling. |                                                              |
| This procedure sets forth how the competencies of the persons responsible for labeling is tested. | This can be done by the labeling of selected data sets.      |
| This procedure sets forth how the persons responsible for labeling are trained and how the success of this training is evaluated. |                                                              |
| This procedure sets forth how the correctness of the label is systematically reviewed. The selection of this justification has been documented by the manufacturer. | The manufacturer can provide identical data sets of multiple persons and assess the consistency of the results. |
| This procedure sets forth, how the monitoring occurs, that the persons responsible for labeling are continually fit and willing to perform the labeling [^C.3.b.3]. | This can be done with datasets with already known labels that are inserted unnoticed by the person during labeling. |

[^C.3.b.1]: If, for example,  patients have to be classified as healthy and sick, the manufacturer must derive the criteria specifically for the intended use, when a patient is to be classified as healthy and when as sick.

[^C.3.b.2]: The “Ground Truth” is the most precise reference method (state of the art). For the determination of arterial hypertension, an invasive blood pressure measurement may provide the most exact results.

[^C.3.b.3]: The labeling of dozens of data sets is arduous. A payment per data set can cause an inappropriate motivation.

#### c) Procedure for (pre-)processing of data

| Requirements                                                 | Comments                                                     |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| The manufacturer has set a procedure that describes the pre-processing of the data before data is used to train or test the model. |                                                              |
| This procedure describes the individual processing steps such as conversion, transformation, aggregation, normalization, format conversion, calculation of feature, conversion of numerical data into categories. | A graphic representation creates a rapid overview. The conversion of numerical to categorical values requires a justification. |
| The procedure describes how the correctness of the interim steps and the final results are assessed[^C.3.c.0] through risk-based evaluations. | This is consistent with the requirements of ISO 13485:2016 chapter 4.1.6. The risk management file must contain these analyzes. |
| This procedure specifies how values with various measurement scales or units are detected and processed. |                                                              |
| This procedure specifies how values are detected and processed that have been collected with various measurement methods. |                                                              |
| This procedure specifies how values or metadata with the same names (such as in column headers) are detected and processed. | This, however, depends on the ML-method (e.g. tabular data, image data) and cannot be demanded as a general best practice. |
| This procedure specifies how missing values within data sets are detected and processed. The manufacturer gives a rationale for the decision[^C.3.c.1]. | Make sure that the rationale differentiates between “missing at random” and “missing not at random”[^C.3.c.2]. |
| This procedure specifies how unusable data sets are detected and handled as per the data inclusion and exclusion criteria. |                                                              |
| This procedure describes how data for training, testing and validation are kept separately. |                                                              |
| This procedure describes how new data can be added after initial processing already has been performed (if applicable). |                                                              |
| The procedure describes how uniqueness of data is ensured.   |                                                              |
| This procedure specifies how outliers are detected and processed[^C.3.c.3]. The manufacturer gives a rationale for the decision[^C.3.c.4]. | Show example of a date / feature. This, however, depends on the ML method (e.g. tabular data, image data) and cannot be demanded as a general best practice. |
| This procedure specifies how unusable data sets are detected and handled[^C.3.c.5]. The determination was justified by the manufacturer. | Request example of a date / feature.                         |
| The manufacturer has analyzed and mitigated all risks caused by data processing. |                                                              |


[^C.3.c.0]: Options include software tests and redundant or alternative calculations such as with Excel.

[^C.3.c.1]: The options for processing include deleting the data set, replacement by the average value of other data sets, new value “missing” (for categorical values).

[^C.3.c.2]: An example for "missing not at random” is lab values that are too high that are cut off.

[^C.3.c.3]: The options for processing include deleting the data set, correcting the value, setting the value to a set value (min/max).

[^C.3.c.4]: This justification is more important in the regression method than with tree-based methods.

[^C.3.c.5]: Examples are x-rays of poor quality or patients who do not meet the inclusion criteria.

#### d) Documentation and version control

| Requirements                                                 | Comments                                                     |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| The manufacturer has listed the data sources.                |                                                              |
| The manufacturer has documented all data processing steps mentioned in the previous chapter. |                                                              |
| This document specifies rules for data inclusion and exclusion. |                                                              |
| This document provides  a rationale if additional data have been excluded or if data have been kept despite meeting the specification. |                                                              |
| This document describes how all data can be traced back to its source. |                                                              |
| The document describes how compliance with the requirements is verified. |                                                              |
| The manufacturer has described the "funnel” that allows detection of how much data originates from which data source (e.g. clinics) and at which processing step how many data sets have fallen away for which reason. |                                                              |
| The manufacturer has described the collected data using descriptive statistics[^C.3.a.4]. | The ["Dataset Nutrition Label"]() is recommended.            |
| The manufacturer has put training, validation and test data under version control. |                                                              |
| The manufacturer has protected all data and code from loss and unwanted changes. | This includes a documented procedure for backups and restoring, and backup records. |
| The manufacturer has documented all software for data processing including the libraries used and listed under version control. |                                                              |
| The manufacturer has set forth a policy (e.g. SOP) specifying the configuration and version control process. |                                                              |
| The manufacturer has kept records demonstrating that the software actually is under version control. |                                                              |

### 4. Model development requirements

#### a) Model preparation

| Requirements                                                 | Comments                                                     |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| The manufacturer has justified the selection of the features considered during training. | List the features and rationales why these features were taken into account. |
| The manufacturer has described the dependency of the features among each other. | A Directed Acyclic Graph (DAG) helps in visualization. This, however, depends on the ML-method and cannot be demanded as a general best practice. |
| The manufacturer has documented and justified the ratio that it divides up the data into training, validation and test data. |                                                              |
| The manufacturer has documented the stratification it uses to divide up the data in to training, validation and test data[^C.4.a.1]. |                                                              |
| The manufacturer has documented how it ensures that multiple data sets for an object are in the same “bucket” (training, validation and test data). |                                                              |
  | The manufacturer has provided justification if data are not split at random. |                                                              |
| The manufacturer has documented how it ensures that the development team is prevented from gaining access to test data. |                                                              |
| The manufacturer has documented how he ensures that test data are not used for model training and validation. |                                                              |
| The manufacturer has set forth a role-based policy for data access. |                                                              |
| The manufacturer has described when it recodes the data specifically for the model or specifically for the library[^C.4.a.2]. |                                                              |

[^C.4.a.1]: For data with rare features or labels, it may be necessary to distribute the data not just at random.

[^C.4.a.2]: Examples of this are normalization, selection of class labels (e.g. 0 or 1), selection of column names, distribution of categorical values over multiple columns.

#### b) Model training

| Requirements                                                 | Comments                                                     |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| The manufacturer has documented model specific data processing. |                                                              |
| The manufacturer performs model training, tuning of hyperparameters and model selection exclusively with the training and validation data (e.g. using cross-validation). |                                                              |
| The manufacturer has documented and justified the choice of the hyperparameters[^C.4.b.1]. |                                                              |
| The manufacturer has set a forth a policy forbidding the use of test data to optimize the model (only training and validation data may be used.) |                                                              |
| The manufacturer has documented and justified the choice of epochs[^C.4.b.2], if neural networks were used. | Where possible, display  learning curves.                    |
| The manufacturer has determined and documented the quality metrics for which it wants to optimize the model and justified it based on the intended use. | The selection of these quality metrics is specific to the intended use. |
| The manufacturer has trained multiple models with multiple hyperparameters (including simpler and interpretable models). |                                                              |
| The manufacturer has verified that the training actually trains the model. | Document that the training process improves the model's performance. |

[^C.4.b.1]: Examples: Loss function, optimizer, learning rate, number of epochs

[^C.4.b.2]: It might be helpful to illustrate the dependency between the quality of the model on the one hand and number of epochs on the other hand e.g. using learning curves. These learning curves, however, exist for neuronal networks and boosting procedures, for example, but not for models with numerical solution (e.g. linear regression) or for a single tree.

#### c) Model evaluation

| Requirements                                                 | Comments                                                     |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| The manufacturer has set forth a model evaluation plan which specifies the evaluation activities, the roles involved and the milestones at which these activities have to be performed. |                                                              |
| The manufacturer has set forth a validation specification and validation results for the evaluation of the model with validation data set. |                                                              |
| The manufacturer has set forth a test specification and test results for the final evaluation of the model with new test data. |                                                              |
| The manufacturer has documented the quality metrics for the various models, such as for a binary classification using a confusion table. | This documentation should not include only the values that the manufacturer has used to optimize the model. |
| The manufacturer has specified values for the specified quality metrics. |                                                              |
| The manufacturer has not only globally assessed and documented the quality metrics for the various models, but also separately for various features. |                                                              |
| The manufacturer has examined the data sets that have exhibited good model performance versus datasets that have performed badly. | We recommend a residual analysis in which the errors are listed via the feature values. |
| For individual data sets there may be an evaluation of the feature that the model particularly determined in the decision. |                                                              |
| The manufacturer has examined the data sets in which the model is particularly secure and particularly insecure[^C.4.c.1]. |                                                              |
| The manufacturer has justified the ultimate selection of the model using the quality criteria and intended use and in particular shown if simpler and interpretable models were not used. |                                                              |
| The manufacturer has considered (in particular for tabular data sets) to show for individual data sets the feature that the model particularly determined in the decision[^C.4.c.2]. | This, however, depends on the ML-method and cannot be demanded as a general best practice. |
| The manufacturer has considered to evaluate how and how strongly individual features had to change for the model to come to another prediction. | This is referred to as ["Counterfactuals"](https://christophm.github.io/interpretable-ml-book/counterfactual.html). This, however, depends on the ML-method and cannot be demanded as a general best practice. |
| The manufacturer has analyzed/visualized the dependency (strength, direction) of the prediction of the feature values[^C.4.c.3]. | This, however, depends on the ML-method and cannot be demanded as a general best practice. |
| The manufacturer has considered to synthesize data sets that activate the model particularly strong[^C.4.c.4]. | This, however, depends on the ML-method and cannot be demanded as a general best practice. |
| The manufacturer has approximated the model using a simplified surrogate model such as a decision tree. | This, however, depends on the ML-method and cannot be demanded as a general best practice. |
| The manufacturer has documented and justified the selection of the model based on its performance on a representative dataset. |                                                              |
| This documentation lists the various models that have been compared. |                                                              |
| This documentation includes a comparison of these models (architectures). |                                                              |
| This comparison includes quality metrics.                    |                                                              |
| This documentation shows that clearly designed, representative datasets and model performance on those datasets is adequate following an assessment criterion e.g. an acceptable risk-benefit-ratio. |                                                              |
| The manufacturer has done a risk-benefit assessment that discusses interpretability, performance (e.g. quality metrics, efficiency) and robustness. |                                                              |

[^C.4.c.1]: For classification tasks, the model is particularly insecure with probabilities around 0.5.

[^C.4.c.2]: Approaches include LIME (Local Interpretable Model-agnostic Explanations), Beta (Black Box Explanations through Transparent Approximations), LRP (Layer-wise Relevance Propagation) and Feature Summary Statistics (incl. Feature Importance and Feature Interaction).

[^C.4.c.3]: Examples of Sharpley-Values, ICE-Plots, Partial Dependency Plots (PDP)

[^C.4.c.4]: For examples see http://yosinski.com/deepvis

#### d) Model documentation

| Requirements                                                 | Comments                                                     |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| The manufacturer has the model[^C.4.d.1] and/or the training code under version and configuration control. |                                                              |
| The manufacturer can reproduce test and validation results.  | This can prompt for version and configuration control of data, test results and assessments. |
| The manufacturer has the SOUP (libraries and frameworks) under version and configuration control. |                                                              |
| The manufacturer has documented the architecture of the model, the model itself including its hyperparameters. |                                                              |
| The manufacturer has documented the data the model has been trained on. |                                                              |
| The manufacturer has documented potential problems (e.g. biases) and limitations. |                                                              |
| The manufacturer has documented the used software libraries and frameworks (SOUPs). |                                                              |
| The manufacturer has described when it worked with a “pretrained model” and shown why this “pre-training” is suitable for the task. |                                                              |
| The manufacturer has documented the quality metrics and the evaluation results, e.g. of performance and robustness as specified in the model evaluation requirements. | This quality metrics relate to the testing with the test data. |
| The manufacturer has documented (in particular when using tabular data) the limits (such as feature values) within which the model has achieved the quality metrics. | This, however, depends on the ML method and cannot be demanded as a general best practice. |
| The manufacturer has set forth a SOP for documentation and/or version and configuration control of: software code and libraries, configuration files, hyperparameters, test and evaluation results (including quality metrics), software libraries and frameworks. |                                                              |

[^C.4.d.1]: Trained models can be serialized.

### 5. Product development

#### a) Software development

| Requirements                                                 | Comments                        |
| ------------------------------------------------------------ | ------------------------------- |
| The manufacturer has performed the required activities pursuant to IEC 62304 and documented them. | Notes for auditors[^C.5.a.1]    |
| If the manufacturer has implemented the model in another programming language or for another runtime environment, it has created a plan that repeats the activities pursuant to chapter 4. |                                 |
| The manufacturer has set forth a verification plan that requires software system tests. |                                 |
| The manufacturer has determined the software safety class (alternatively the Level of Concern). |                                 |
| The manufacturer has set forth a software requirement specification (SRS). |                                 |
| The SRS specifies user interfaces related requirements.      |                                 |
| The manufacturer has documented the software architecture.   |                                 |
| The manufacturer has performed software unit, integration and system tests. | This includes coverage reports. |
| The manufacturer has documented the strategy for black box testing. |                                 |
| The tests cover all software / product requirements (including non-functional requirements). |                                 |
| The tests  verify risk mitigation measures are effective.    |                                 |
| The tests verify that the system safely manages unseen security attacks. |                                 |
| The manufacturer has  described the software version, test data, test environment (e.g. hardware), tester and evaluation of test results. |                                 |
| After changes to the software the tests are repeated unless the manufacturer can provide a rationale for skipping test activities. |                                 |
| The manufacturer has ensured that tests are reproducible.    |                                 |
| The manufacturer tests the performance (response times, resource consumption) on the target hardware (e.g. browser, mobile device) and has verified that the specified that the performance requirements are met. |                                 |
| The manufacturer has listed and uniquely identified each SOUP / OTS component. |                                 |
  | The manufacturer has specified requirements for each SOUP / OTS component. |                                 |
| The manufacturer has documented the trace between these requirements and respective tests. |                                 |
| The manufacturer has described how to verify all SOUP or OTS components. |                                 |
| The manufacturer has a validation plan for the training functionality of ML library. |                                 |

[^C.5.a.1]: The manufacturers should adhere to the normal best practices such as adherence to coding guidelines, review of code by code reviews using defined criteria, testing to code with unit tests with a defined coverage, etc.



####  b) Risk management

| Requirements                                                 | Comments |
| ------------------------------------------------------------ | -------- |
| The manufacturer has specified the functionalities of the chosen ML libraries that are used for training. |          |
| The manufacturer has specified the functionalities of the chosen ML libraries that are used for prediction. |          |
| The manufacturer has analyzed the risks of a training function not meeting the specifications. |          |
| The manufacturer has analyzed the risks of predict function not meeting the specifications. |          |
| The manufacturer has analyzed the risk for the most important components of the chosen software architecture at least. |          |
| The manufacturer has analyzed the risks that are specific to chosen technologies. |          |
| The manufacturer has listed all steps of data processing and annotation and analyzed the errors that can occur in each step, and analyzed the risks arising from these errors. |          |
  | The manufacturer has analyzed the consequences of porting the software and data to the target system. |          |
| The manufacturer has analyzed the consequences of model bias. |          |
| The manufacturer has analyzed consequences of wrong reference data (e.g. wrong gold standard, wrong comparison). |          |



#### c) Accompanying materials

| Requirements                                                 | Comments                                                     |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| The instructions for use clearly identify the version of the product. | If possible, indicate the UDI                                |
| The instructions for use describe the intended use of the product including the expected medical benefit. |                                                              |
| The instructions for use specify the intended patient population using indications, contraindications and if relevant using other additional parameters such as age, gender, accompanying diseases or availability of information. |                                                              |
| The instructions for use explicitly list the patients / data / use case for which the product may not be used. |                                                              |
| The instructions for use reveal limitations.                 |                                                              |
| The instructions for use document the requirements of the input data (including formats, resolutions, value ranges, etc.). |                                                              |
| The instruction for use specify the intended primary and secondary users pursuant to intended use. |                                                              |
| The instructions for use describe the other conditions applicable to the product (e.g. runtime environment, use environment). |                                                              |
| The instructions for use describe the residual risks.        |                                                              |
| The instructions for use indicate the data with which the model was trained. | This is related both to the patient collective and to the features used. |
| The instructions for use describe the model and algorithms.  |                                                              |
| The instructions for use name the quality metrics.           |                                                              |
| The instructions for use list the factors that could have a negative effect on the product's performance. |                                                              |
| The instructions for use explain risks arising from a product not meeting the performance requirements. |                                                              |
| The instructions for use specify whether the product is further trained during use. If it is further trained, the instructions for use provide information how the system learns over time. |                                                              |
| The instructions for use describe how to update the product. |                                                              |
| The instructions for use contain references to additional literature. |                                                              |
| The instructions for use contain references to licensing rights. |                                                              |
| The instructions for use identify the manufacturer and lists channels for posing questions. |                                                              |
| The instructions for use list possible ethical problems.     |                                                              |
| The instructions for use contain the URL under which the most current versions of the instruction of use can be found. |                                                              |
| The instructions for use of continuous learning systems describe what triggers algorithm updates and how to identify the version of this algorithm. |                                                              |
| The instructions for use of continuous learning systems describe how to permit, delay and roll-back algorithm updates. |                                                              |
| The  document on instructions for use is under version control. |                                                              |
| The manufacturer has set forth a procedure specifying how to develop and verify the instructions for use. |                                                              |

### 6. Product validation

#### a) Usability validation

|Requirements                                                  |Comments|
| ------------------------------------------------------------ | --------- |
|The manufacturer has documented risk arising from a lack of usability in the risk management file. ||
| The risk management file lists risks that arise from misunderstanding, overlooking or ignoring the product’s visual output. ||
| The risk management file lists risks that arise from users blindly trusting or mistrusting the product. ||
| The risk management file lists the risks that have to be mitigated by instructing users e.g. by training or accompanying materials. ||
| The plan of the summative evaluation describes how the effectiveness of these measures is validated. ||
| The usability evaluation report reveals whether the instructions for use are adequate to mitigate risks. ||
| The manufacturer has evaluated all safety relevant use scenarios. ||
| This evaluation contains an assessment of safety relevance for each use scenario. ||
| The use scenarios included in the summative evaluation cover all safety relevant use scenarios. ||
| The summative evaluation evaluates the effectiveness cover all risk mitigation measure. ||
| The manufacturer has defined and specified the usability metrics for (a) understandability, (b) learnability and (c) operability of the product. | For example: production description completeness, customizability, input and output understandability, ... |
| The manufacturer has defined and specified the ‘quality in use’- metrics to measure the extent to which the product meets the needs of target users to achieve specified goals of effectiveness, productivity, and satisfaction in a specified context of use. | For example: task completion, error frequency, user wait time, ... |
| The manufacturer assesses whether the users understand the instructions for use. |           |
| The manufacturer assesses whether the users correctly detect and understand the results during usability validation. |           |

#### b) Clinical evaluation

|Requirements                                                  |Comments|
| ------------------------------------------------------------ | --------- |
| The manufacturer assesses whether the promised medical benefit is achieved with the quality parameters. |           |
| The clinical evaluation contains the medical benefits the manufacturer claims. | |
| The clinical evaluation lists the data (sources) that have been evaluated and that support and that contradict the hypothesis, that the benefits have been achieved | |
| If the data have been collected from other products, than the clinical evaluation discusses the clinical and technical equivalence of the other products. | |
| The clinical evaluation evaluates the impact of quality parameters on the achievement of the medical benefit. | |
| The manufacturer assesses whether the promised medical benefit is achieved is consistent with the state of the art. |           |
| The clinical evaluation lists alternative methods, technologies or procedures. | |
| The clinical evaluation compares the risks and benefits of these alternatives. | |

### 7. Product release

| Requirements                                                 | Comments                   |
| ------------------------------------------------------------ | -------------------------- |
| The manufacturer has documented the model using the criteria listed in chapter 4.d). |                            |
| The manufacturer has assessed and documented the risks as acceptable in risk management and that all of the activities specified in the risk management plan were performed. | Notes for auditors[^C.6.1] |
| There is a usability evaluation report concluding that all activities to formative and summative evaluation plan have been performed. |                            |
| The manufacturer has shown in a "Software as a Medical Device Pre-Specifications “(SPS) report which types of changes it anticipates for systems that it wishes to market in the USA[^C.6.2]. |                            |
| The manufacturer has shown in Algorithm Change Protocol (ACP) how it will perform these changes for systems that it wishes to market in the USA[^C.6.3]. |                            |
| The manufacturer has created a Post-Market Surveillance Plan, see below. |                            |

[^C.6.1]: Using examples, check that the efficacy of risk management measures was tested so that there is a traceability of risks for risk control measures.

[^C.6.2]: Changes may affect the intended use, the input data and the clinical and analytical performance.

[^C.6.3]: The approach must, for example, address handling data, re-training, the performance and the updates.

## D) Post-market requirements

### 1. Production, Distribution, Installation

|Requirement|Comments|
|:--|:--|
|The manufacturer has applied version- and configuration control.|Version and configuration control apply to the software as well to accompanying materials such as instructions for installation and use.|
|The manufacturer has ensured that the product has a unique identification (ID).|In EU and in the US, there is typically the need for a UID-DI and UDI-PI.|
|The manufacturer has ensured that there is a bill of materials.|The bill of material also contains all SOUP/OTS Software.|
|The manufacturer has described how it ensures that only exactly the intended artefacts (files) in exactly the intended version of the product or as a product are delivered.|This is configuration management. Also relevant to downloads or AppStores.|
|The manufacturer has described installation, update and decommissioning of the product.||
| These instructions specify the runtime environment.          ||
| These instructions specify how the correct installation can be verified. ||
|The manufacturer has described how the persons responsible for installation know which is the most current version and how mistakes in installation can be ruled out.|This is only relevant to stand-alone software. A SOP or work instruction would be expected here.|
|The manufacturer has described how one ensures during installation that the requirements specified in the accompanying material are actually fulfilled (see above).|A SOP or work instruction would be expected here.|
|The manufacturer has established procedures that ensure that it can communicate with the operators and users of its product in a timely manner||
|The manufacturer set forth an SOP  covering customer communication including handling of customer complaints.||
| The manufacturer has set up  a website that contains information about latest product releases and news related to security vulnerabilities .||
| This website provides the means to download the software.    ||
| The instructions for use reference this website.             ||
| The instructions for use and the website reveal contact information e.g. e-mail, phone number, and/or a contact form. ||

### 2. Post-Market Surveillance

|Requirements|Comments|
|:--|:--|
|The manufacturer has created a Post-Market Surveillance (PMS) Plan specifically for the product.||
|The manufacturer has created a SOP specifying how to compile post-market surveillance plans.||
|The PMS lists all relevant data sources to be monitored.|These sources include information from SOUP manufacturers (also of ML libraries) and also includes security disclosures by those vendors|
|The manufacturer has specified the data it wishes to collect and analyze in this PMS plan.||
|The PMS plan describes for each data source how, how often and by whom data are collected.||
|The PMS plan specifies how data has to be analyzed.||
|The PMS plan requires that quality metrics such as sensitivity and specificity are monitored.||
|The PMS plan requires to collect and analyze data to assess how the use of the system changes over time.||
|The manufacturer has specified in the PMS plan the quality criteria and threshold values that it considers necessary for handling of in particular a re-evaluation of the risk-benefit analysis.||
|The manufacturer has analyzed when determining these threshold values which feedback loops the threshold values can influence[^D.2.1].||
|The manufacturer has analyzed when determining these threshold values which self-fulfilling prophecies the threshold values can influence[^D.2.2].||
|In the PMS plan, the manufacturer described how it collects and analyzes information on adverse medical effects.||
|In the PMS plan, the manufacturer described which information on (adverse) behavioral changes or (predictable) misuse is collected and analyzed[^D.2.3].||
|In the PMS plan, the manufacturer described how it collects and analyzes information on additional “adverse effects” [^D.2.4].||
|The manufacturer has described in the PMS plan how it collects information to be able to analyze whether the data in the field is consistent with the expected data or training data[^D.2.5].|Note for auditors[^D.2.6]|
|In the PMS plan, the manufacturer has described how and how often it wants to collect information on whether the product still meets the state of the art.|Note for auditors[^D.2.7]|
|In the PMS plan, the manufacturer has specified for continuous learning systems whether and how often which data sets have to be retested after algorithm updates.||
|In the PMS plan, the manufacturer has specified how and how frequently changes in algorithm updates are assessed.||
|In the PMS plan, the manufacturer has listed threshold values that trigger actions.|The threshold values include quality metrics and features.|
|In the PMS plan, the manufacturer has specified the frequency and content of compiling post-market surveillance reports.||
|In the PMS plan, the manufacturer has described how and how often it wants to collect information on whether the “Ground Truth” or the gold standard are still up to date.||
|In the PMS plan, the manufacturer has described how and how often changes pursuant to the Algorithm Change Protocol (ACP) and within the “SaMD Pre-Specifications” (SPS) are made.||
|The manufacturer should perform PMS and compile reports, both according to the post-market surveillance plan.||
|There is a PMS report for each product respectively product type.||
|These PMS reports clearly identify the respective products via its ID.||
|These PMS reports identify the post-market data and conclude whether activities are required.||
|The manufacturer has established a post-market risk management system.|It is possible to combine post-market risk management and post-market surveillance.|
|The manufacturer has specified how, how often and by whom the state of the art is monitored and re-assessed.||
|This state-of-the-art assessment takes latest algorithms for machine learning and for improving interpretability into account.||
|This state-of-the-art assessment takes alternatives for the "ground-truth" respectively the gold standard.||
|The manufacturer has specified how, how often and by whom post-market data are evaluated for new or changed hazards, hazardous situations, and risks.||
|The post-market risk analysis searches for (adverse) behavioural changes or (foreseeable) misuse.||
|For products that have been placed on the market for more than one-year, the manufacturer has documented post-market risk management activities.||
|For products marketed in the US the manufacturer has created an Algorithm Change Protocol (ACP) and a "SaMD Pre-Specifications" (SPS).||
|The manufacturers has described design changes and analyzed their impacts.||

[^D.2.1]: Examples for these feedback loops: **Example 1**: A travel recommendation app sends targeted advertising depending on feature (last trip). This influences travel behavior. **Example 2**: An algorithm provides prognoses. Therefore, the physician will treat the patients better or earlier...

[^D.2.2]: Example 1 (criminalistics)

[^D.2.3]: Example: Radiologists rely on the software and don't look at the images anymore, so they overlook findings.

[^D.2.4]: Examples would be ethical challenges such as the YouTube algorithm, which achieves the goal, maximizing the click count or use duration, but promoting violence and conspiracy videos.

[^D.2.5]: One speaks here of a distribution shift or data drift.

[^D.2.6:]: The manufacturer should set threshold values for features or for the variance / covariance over time. This allows visualization or quantification in particular for non-normally distributed data over the comparison of histograms or core density estimations.

[^D.2.7]: For example, have the manufacturer explain the process on how it is systematically informed of new developments in machine learning, and how it assesses these developments and reacts to them.



### 3. Decommissioning


|Requirements|Comments|
|:--|:--|
| The manufacturer has established a plan before decommissioning the medical device. ||
| This plan describes how  users and operators are informed. ||
| This plan describes the disposal of the product.             ||
| This plan describes archiving of product and data (e.g. training, test, validation data), software, documentation, considering security and privacy concerns. ||
| The manufacturer has analyzed risks of decommissioning.      ||
| This risk analysis assesses risks for patients due to a product that is no longer available. ||
| This risk analysis assesses risks due to negative impact on other systems. ||


## E) Annexes

### 1. Additional literature

#### a) Laws

- [Medical Device Regulation](https://eur-lex.europa.eu/legal-content/DE/TXT/?uri=uriserv:OJ.L_.2017.117.01.0001.01.DEU&toc=OJ:L:2017:117:FULL) MDR
- [In-vitro Diagnostic Device Regulation](https://eur-lex.europa.eu/legal-content/DE/TXT/?uri=uriserv:OJ.L_.2017.117.01.0176.01.DEU&toc=OJ:L:2017:117:FULL) IVDR

#### b) Standards and Best Practice Guides

- **IEC 62304/AMD1**, Medical device software – Software life cycle processes
- **IEC 82304-1**, Health software – Part 1: General requirements for product safety
- [FDA Guidance Documents on Machine Learning](https://www.fda.gov/medical-devices/software-medical-device-samd/artificial-intelligence-and-machine-learning-software-medical-device)
- WHO/ITU: [Good practices for health applications of machine learning: Considerations for manufacturers and regulators](https://aiaudit.org/assets/pdf/standards/FGAI4H-K-039.pdf) 

#### c) Industry literature, textbooks

- Christoph Molnar: [Interpretable Machine Learning](https://christophm.github.io/interpretable-ml-book/)
- Patrick Hall: [Machine Learning Interpretability
  with H2O Driverless AI](http://docs.h2o.ai/driverless-ai/latest-stable/docs/booklets/MLIBooklet.pdf)
- Patrick Hall: [On the Art and Science of Machine Learning Explanations](https://arxiv.org/pdf/1810.02909.pdf)
- Johner Institute: [Video training on machine learning for medical products](www.auditgarant.de)

### 2. Recitals

1. Manufacturers are increasingly developing medical products that use the process of artificial intelligence, in particular machine learning. Many of these procedures are still very new, and lack best practices. This creates new risks for patients, users and third parties.
2. The EU directives (MDR, IVDR) explicitly require the safety of the products in the relevant annexes I. Bu concrete requirements for these classes of products are completely lacking. Therefore, both the manufacturers and the notified bodies and authorities lack concrete guidelines on how to evaluate the safety of the products.
3. Contrary to most other fundamental requirements, no standards on the subject of AI are harmonized. Therefore, there is no canonical catalog of requirements that reflects the recognized state of the art of technology.
4. The FDA has started to formulate requirements on using Continuous Learning Systems, CLS. These specifications are unsuitable to sufficiently set requirements for the products and processes as early as the product development stage.
5. The safety of medical products must be considered in all phases of the product life cycle processes. A limitation to testing is insufficient. This fact must be in line with best practices and guidelines.
9. One hopes that standards for the safety of AI-based medical products will be developed and harmonized. This will still take years. Therefore, we need a guideline (only) in this interim phase.
10. This guideline should be available very soon (by July 2019) to be able to quickly serve the manufacturers as an orientation and enable them to act immediately. The high speed of development makes compromises regarding harmonization with the most parties possible inevitable.
11. The technological advancement in the area of artificial intelligence is immense. New procedures and technologies are continuously being published. On the one hand, a guideline should be a specific as possible. On the other, it cannot be so specifically targeted toward one procedure or technology, to achieve a sensible “shelf life”. Therefore, a guideline must address general concepts. However, it cannot claim to be complete.
12. Such a guideline must take into consideration the specifics of medical products, which includes the principles of patient safety (safety) and a risk-based approach. In a concrete case, selected actions for information security ("controls”) will be in conflict with the fundamental requirements. For this reason, there can be no set list of “controls” for medical products. The manufacturer's intended use of the product is critical.
14. The simple intelligibility and practicability is essential to the desired positive influence of a guideline on the safety of AI-based medical products. Therefore, there must be the least abstract or “high level” requirements possible but “binary decisive” test criteria.
15. Do increase practicability, the authors have avoided collating many requirements to the greatest extent possible. Rather, they have limited themselves to those that they consider particularly relevant and implementable.
16. And to promote distribution and the level of familiarity, the guideline must be available and remain available at no cost.
17. The guideline should be available in German and English.
