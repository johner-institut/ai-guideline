# Guideline for AI for medical products

## A) Meta information

### 1. Objective of the guideline

The objective of this guideline is to provide medical device manufacturers, authorities and notified bodies instructions and to provide them with a concrete checklist to

- understand what the expectations of the notified bodies and authorities are,
- to promote step-by-step implementation of safety of medical devices, that implement artificial intelligence methods, in particular machine learning,
- to compensate for the lack of a harmonized standard (in the interim) to the greatest extent possible.

The guideline is **not** meant to serves as a training manual or guideline to achieve the safety of AI based medical devices. It is to be a guideline for its review.

The annex lists the recitals which led to the development of this guideline.

### 2. Scope of applicability and target group

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

|Requirements|Comments|Regulatory references|
|:--|:--|:--|
|The manufacturer has created a list of all roles inside the scope of its QM system that are directly or indirectly concerned with AI. [^B2-01]||	ISO 13485, 5.5.1, 6.2., ISO 14971, 3.3., IEC 62304, 2017/745/ EU Article 10.9, 21 CFR part 820.30 (b)|
|The manufacturer has documented the competency requirements for each role inside the scope of its QM system that is directly or indirectly concerned with AI. [^B2-02]|Competencies are related to education, knowledge or skill. Examples of competencies: Machine learning, explainable AI, medicine (for relevant domains), clinical and usability validation.| ISO 13485, 6.2., ISO 14971:2019, 4.3, ISO 13485:2016, 7.3.2, IEC 82304, 6.1|
|The manufacturer has appropriate records for the training, further education and competencies that allow for the conclusion that the persons actually have these competencies.|| ISO 13485, 6.2. |
|The (software) development plans have defined the product-specific competencies (beyond or deviating).|Requirements of ISO 13485:2016| ISO 13485, 7.3.2., IEC 82304, 6.1. |

[^B2-01]: Examples are: Data Scientists, Developers, Testers, Regulatory Affairs and Quality Mangers, Service and Support Employees, Product Managers, Medical Device Consultants, Physicians

[^B2-02]: Competencies (level if understanding, capability to perform tasks) should be listed, not primary subjects

### 4. Documentation

The manufacturers should keep evidence that they have followed the relevant requirements of this guideline. There are no specific requirements for documentation and “objective evidence”.

In Europe at least, there is no obligation to create a specific document that summarizes the activities especially for AI. Manufacturers can integrate these aspects into existing documents such as QM documents (e.g. standard operating procedures, work instructions) and the technical documentation (e.g. software files, risk management files, clinical evaluation, summative evaluation of the usability).

## C) Requirements for product development

### 1. Intended use and stakeholder requirements

#### a) Intended medical use

|Requirements|Comments| Regulatory references|
|:--|:--|:--|
|The manufacturer has determined for which medical purpose (diagnosis, therapy, monitoring, predictions) the medical product should support.|The intended use / purpose should not be mistaken for the description of functionality (e.g. calculation of scores).| ISO 13485, 4.2.3. and 7.3.2. c., 2017/745/EU Annex II (1.1), ISO 14971:2019, 5.2, 21 CFR 814.20 (b)(3)(i), 21 CFR part 820.30(c)|
|The manufacturer has characterized the patients to be diagnosed, treated or monitored with the medical product. This characterization includes patient demographics, indications, contraindications and associated diseases.|This characterization is also included in IEC 62366-1. Patients may also simultaneously be users of the product.| 2017/745/EU, Annex I, 23.4 and Annex II, 1.1. c, 2017/746/EU, Annex II, 1.1. c, IEC 62366-1, 5.1. and 5.3., ISO 13485, 7.3.3 a., 21 CFR 814.20 (b)(3)(i)|
|The manufacturer has specified on which body locations the product will be used or from which body location the data originate.|Also called for in IEC 62366-1 clause 5.1.| 2017/745/EU, Annex II, 1.1., 2017/746/EU, Annex II, 1.1., IEC 62366-1, 5.1.3. |
|The intended use also suggests what the goal of machine learning techniques is.|Classification and regression, clustering, similarity search and recommender systems are typical goals of machine learning methods. The description of the role of machine learning is necessary to fulfill the requirement for the description of the "physical principle".| IEC 62366-1, 5.1, 2017/745/EU Annex II, 1.1, 21 CFR part 814.20, XAVIER University "Building Explainability and Trust for AI in Healthcare"|
|The manufacturer has determined the intended lifetime of the medical device.|This lifetime is determined, for example, by the state of the art (e.g., medical advances, new ML-methods, competitive products) and the speed at which the technical environment and libraries evolve.|


#### b) Intended users and context of use

| Requirements                                                 | Comments                                                     |Regulatory references
| :----------------------------------------------------------- | :----------------------------------------------------------- |:--|
| The manufacturer has characterized the intended users, e.g. using demographic features (age, gender), regarding the training, experience in medical domains, regarding technical knowledge, physical and mental limitations, linguistic skills and cultural background. | If the manufacturer does not foresee any limitations regarding these attributes, it must document this. | 2017/745/EU, Annex I, 5 and Annex II, 1.1, IEC 62366-1, 5.1., XAVIER University "Building Explainability and Trust for AI in Healthcare"|
| The manufacturer has characterized the intended use environment (also social environment such as stress, shift work, frequently changing colleagues)| This characterization is also required by IEC 62366-1. It is also relevant in the context of the explainability of AI. | 2017/745/EU, Annex I, 5, IEC 62366-1, 5, XAVIER University "Building Explainability and Trust for AI in Healthcare"|
|The manufacturer has described the core tasks that the medical device is to support. | The use scenarios that manufacturers must specify according to IEC 62366-1 can also be derived from these core tasks.| IEC 62366-1 |

#### c) Stakeholder requirements

| Requirements                                                 | Comments                                                     |Regulatory references|
| :----------------------------------------------------------- | :----------------------------------------------------------- |:--|
| The manufacturer has operationalized the goals listed in the intended use with quantitative values [^C.1.c.1]. | It is not unusual that these values are supplemented and revised during the course of development. | 2017/745/EU, Annex I, 23.4 and Annex III, 1.1, FDA SW validation guidance 5.2.2, FDA Guidance for the Content of Premarket Submissions for Software Contained in Medical Devices (s. "Software Requirements Specification")| 
| The manufacturer has set forth the runtime environment of the product regarding hardware (screen size, screen resolution, storage, network connection etc.) and software (e.g. operating system, browser, runtime environments such as Java runtime environment or .NET). | For apps, this characterization must be done for the app and for the server part. | ISO 13485, 7.3.3, 2017/745/EU, Annex I, 17.3 and 17.4, IEC 62304, 5.2, XAVIER University "Building Explainability and Trust for AI in Healthcare", FDA SW validation guidance 5.2.2, FDA Guidance for the Content of Premarket Submissions for Software Contained in Medical Devices (s. "Software Requirements Specification")|
| The manufacturer has specified the data interfaces using the levels of the [interoperability model](https://www.johner-institut.de/blog/tag/interoperabilitat/) and set forth the formats and for images, their specific properties (size, resolution, color coding). | This is required pursuant to IEC 62304 chapter 5.2.2. | IEC 62304, 5.2.2, FDA Guidance for the Content of Premarket Submissions for Software Contained in Medical Devices (s. "Software Requirements Specification")|
|The manufacturer has specified the requirements for the input data. | The input data may also depend on the generation of the data, e.g. on the recording method, on technical parameters (magnetic field strengths, number of conductive electrodes, direction), on environmental conditions during the recordings, on the manufacturer, on the medical device, etc.... | IEC 62304, 5.2, ISO 14971:2019, 5.3, FDA Guidance for the Content of Premarket Submissions for Software Contained in Medical Devices (s. "Software Requirements Specification") |
| The manufacturer has set forth all markets and all regulatory requirements relevant to these. | Show this list.  | 2017/745/EU, Annex IX, 2.2, ISO 13485, 5.2 and 7.2.1 | 
| The manufacturer has specified whether the system should continue to learn after it has been placed on the market. If this is the case, the manufacturer has specified whether this continuous training will be global/centralized or decentralized (e.g., per product or per hospital) and online or offline. | 

[^C.1.c.1]: **Example**: Purpose: The software supports radiologists in diagnosing cancers using CT images of the head. Quantitative value: 95% of radiologists working with software detect the cancer.


#### d) Input for risk management and clinical evaluation

| Requirements                                                 | Comments                                                     | Regulatory References| 
| :------------------------------------------------------------ | :------------------------------------------------------------ |:--|
| The manufacturer has listed alternative procedures and evaluated them in terms of benefit, safety, and performance. | The discussion of the state-of-the-art is a requirement of MEDDEV 2.7/1 and the MDR/IVDR. | 2017/745/EU, Annex I, 1., 2017/746/EU, Annex I, 1.,  MEDDEV 2.7/1, ISO 14971:2019, 4.2 and 10.9, FDA guidance on "Factors to Consider When Making Benefit-Risk Determinations in Medical Device Premarket Approval" (e.g. Part C)|
| The manufacturer has compared the aforementioned quantitative values with the relevant values of alternative methods. | Manufacturers should create a tabular overview.  |
| The manufacturer has justified why machine learning is superior to the other methods and thus justified the associated risks. | | 2017/745/EU, Annex I, 1., 2017/746/EU, Annex I, 1., MEDDEV 2.7/1 |
|The manufacturer has drawn up a list of risks specifically arising from the application of machine learning methods. | Is part of the risk management file | ISO 14971, 5.4. and 5.5., 2017/745/EU, Annex I, 3., DIN SPECT 2, ISO/TR 31004:2013 - Risk management - Guidance for the implementation of ISO 31000 |                                                                                                                                 
|The manufacturer has analyzed the risks that arise when patients other than those specified are diagnosed, treated, or monitored with the product. |    |
| The manufacturer has analyzed the risks arising if persons other than the specified users, use the product. |                                                              | ISO 14971, 5. |
| The manufacturer has analyzed the risks arising through use in an environment different than that specified. |  |  2017/745/EU, Annex I, 14.2.(d), 2017/746/EU, Annex I, 13.2.(d), ISO 14971, 5., IEC 82304, 4.1. (b)  |
| The manufacturer has analyzed the risks arising from inputs not in the specified format. | | ISO 14971, 5., IEC 82304, 4.1. (c)|                                                             
| Manufacturers have analyzed risks arising from data not generated according to the specified prerequisites. |                                                              |
|The manufacturer has assessed the risks when the system is used in a patient population other than that specified. | | ISO 14971, 4.2., 4.3., 5., IEC 82304, 4.1. |


### 2. Software requirements

#### a) Functionality and performance

|Requirements|Comments|Regulatory references|
|:--|:--|:--|
|The manufacturer has comprehensibly derived quantitative quality criteria or requirements for the software or/and the algorithm from the intended use [^C.2.a.1].|This comprehensibility can be represented particularly well with a traceability matrix.| ISO 13485, 7.3.3., IEC 62304, 5.2, XAVIER University "Building Explainability and Trust for AI in Healthcare", FDA guidance on "Software Validation", chapter 5.2.2|
|The manufacturer considered for example the following quantitative quality criteria or requirements: for classification problems, accuracy (Mean or Balanced Accuracy), positive predictive value (Precision), specificity and sensitivity; for regression problems, Mean Absoute Error and Mean Square Error.| For unbalanced data, i.e. when labels occur with very different frequencies, Balanced instead of Mean Accuracy should be used. However, the choice of quality criteria depends strongly on the intended use. | ISO 13485, 7.3.3., 7.3.4., IEC 62304, 5.2. |
|The manufacturer has specified the requirements regarding repeatability and reproducibility of requirements.|This is particularly relevant with "Continuous Learning Systems".| 2017/745/EU, Annex I, 17.1. , 2017/746/EU, Annex I, 16.1., ISO 13485, 7.3.3., 7.3.4 |
|The manufacturer has specified how the system will behave if the inputs do not meet the specified conditions [^C.2.a.2].|This is an aspect of robustness to be specified according to ISO 25010 and IEC 62304 Chapter 5.2. | ISO 25010,, IEC 62304, 5.2., ISO 14971:2019, 5.4, FDA guidance on "Software Validation" chapter 5.2.2, FDA digital health criteria|
|The manufacturer has determined which self-tests the system must perform and how it behaves if this is not successful.|This is particularly relevant for "Continuous Learning Systems".| ISO 13485, 7.3.3. |
|The manufacturer has determined how fast the system must create the outputs.|This determination may be done depending on the size and amount of data.| 2017/745/EU, Annex I, 17.1., 2017/746/EU, Annex I, 16.1., ISO 13485, 7.3.3. |
|The manufacturer has specified the availability of the medical device.|This is an aspect of robustness and must be specified pursuant to ISO 25010 and IEC 62304 chapter 5.2.| ISO 25010, IEC 62304, 5.2., ISO 14971, 4.3., ISO 13485, 7.3.3. |

[^C.2.a.1]: Examples:  **Example 1**: The stakeholder requirement states that 95% of radiologists must be able to detect a cancer with the product. The requirement of the algorithm states that it must display a sensitivity of 97%. **Example 2**: The stakeholder requirements state that arterial calcification must be able to be detected at a sensitivity of 92%. The requirements of the algorithm state that it must be able to exactly predict the strength of the plaques in the blood to 0.2 mm.

[^C.2.a.2]:  Examples: incomplete data sets, lack of data sets, wrong data format, excessive data quantities, data outside of specified value ranges, wrong temporal sequence of data.

#### b) User interface

| Requirements                                                 | Comments                                                     | Regulatory references|
| :----------------------------------------------------------- | :----------------------------------------------------------- | :--|
| The manufacturer has specified what the user interface must display when the preconditions are not met[^C.2.a.2] in order to operate the system safely (e.g., inputs not valid or not expected). |  | 2017/745/EU, Annex I, 5., 2017/746/EU, Annex 1, 5., IEC 62366-1, 5.2.  |
| The manufacturer has specified what the user interface must display if the output does not meet the specified quality criteria. |    |  |
| The manufacturer has determined whether instructions for use and training materials are required. | The MDR / IVDR allow exceptions to the obligation. | 2017/745/EU, Annex I, 23., 2017/746/EU, Annex I, 20., ISO 13485, 4.2.3., FD&C, 21 CFR parts 801 and 820.120|


#### c) Additional software requirements

| Requirements                                                 | Comments                                    | Regulatory references|
| :----------------------------------------------------------- | :------------------------------------------ |:--|
| The manufacturer has set forth which requirements the system must fulfill to detect internal system errors. | Could be an audit log or a monitoring port. | 2017/745/EU, Annex I, 17, 18, 23.4, IEC 62304, 5.2, 5.3 and 7.1,
ISO 149781:2019, 5.4, FDA guidance on software validation e.g. chapter 5.2.2, 5.2.3 and 5.2.4, GMLP Guiding Principles (by FDA et al) #2 (data integrity)  |
| According to the GDPR, the specified system must not expose patients to decisions based exclusively on automatic data processing. Manufacturers should address the corresponding requirement and be able to justify the chosen legal basis. | Requirement of Art. 22 of the GDPR.  | Art. 22 of the GDPR. |  |
| The manufacturer has determined the requirements that the software must meet in order to ensure the IT security of the product. | IT security is not the subject of this guideline, but the [IT-Sicherheits-Leitlinie](https://github.com/johner-institut/it-security-guideline/).  |



#### d) Special requirements for continuous learning systems

| Requirements                                                 | Comments                                                     | Regulatory references |
| :----------------------------------------------------------- | :----------------------------------------------------------- |:--|
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

| Requirements                                                 | Comments                                                     | Regulatory references|
| :------------------------------------------------------------| :------------------------------------------------------------|:--|
| The manufacturer has specified the number of data sets and given a justification why this is sufficient [^C.3.a.1]. | This concerns the data sets for training, validation and test. | ISO 13485, 7.3.7 |
|The manufacturer has characterized the inclusion and exclusion criteria of data by relevant attributes [^C.3.a.2]. | This includes documentation of data types, units and value range. | ISO 24028, XAVIER University "Building Explainability and Trust for AI in Healthcare" |
|The manufacturer has specified technical inclusion and exclusion criteria for data[^C.3.a.3]. ||
| The manufacturer has described the procedure by which it ensures that data sets that do not meet the inclusion criteria or should be excluded are actually excluded. | Procedure includes a software supported assessment. This software must be validated. |
| The manufacturer has described the collected data using descriptive statistics[^C.3.a.4]. | The ["Dataset Nutrition Label"](https://ahmedhosny.github.io/datanutrition/) is an recommended option. |
| The manufacturer has justified where the data are collected and why these are representative for the target population. As reasonable, these have been compared to scientific publications and to registers. |                                                              |
| The manufacturer has listed and discussed factors that could cause a bias in the data. |   | ISO 24028 e.g. 10.5, DAISAM |                                                           
| The manufacturer has analyzed which influences the type and location of data collection have on the data[^C.3.a.5]. |  
|The manufacturer has established a procedure to ensure that data protection requirements are met. | For example, the data is anonymized or pseudonymized before testing and training. The data protection officer should be involved in this.  |
| The manufacturer has examined and excluded the possibility of a “label leakage”[^C.3.a.6]. | This depends on the applied ML model is not a general best practice. |
| The manufacturer that uses surveys has justified the selection of the surveys, the time of survey and possibly the method for their assessment, in particular if no standardized survey exists. |                                                              |

[^C.3.a.1]: A specification for the number of data is hardly possible. This depends on the “signal-noise-ratio” among other things. For example, for one data set, the percentage of relevant genes and the strength and frequency of the predicted effects affect the number. For data to be classified, the number of the data sets with the rare class (e.g. the prevalence of diseases) is decisive.

[^C.3.a.2]: e.g. demographic data (age, gender), physical parameters (height, weight), diseases, vital parameters, lab parameters, presence of additional tests, case history.

[^C.3.a.3]: Examples: **Example 1**: Patients who must be ruled out due to a heart pacemaker or lung surgery because the images cannot be analyzed or could lead to erroneous classification. **Example 2**: Formats and technical parameters such as image sizes, resolution, brightness and contrasts, color coding, compression, recording equipment, recording method (e.g. CT versus MRI), with or without contrast agent, zoom. **Example 3**: Completeness of meta-data.

[^C.3.a.4]: Usually, the calculation of distributions (histograms), mean / average values, quartiles, possibly “joint distribution of features". The correlation of data among that data should be examined. Additional examples are found in the [publication by Sarah Holland et al.](https://arxiv.org/pdf/1805.03677.pdf) (such as in table 1)

[^C.3.a.5]: Examples: Influence of various measurement devices, surveys, policies (such as a clinic only takes lab parameters only in emergencies, another routinely. Frequency and reason examined with the patient), type of clinic (e.g. small hospital, from which all serious cases must be referred versus university hospital > survivor basis), self-selection bias (e.g. patients with various pre-existing conditions usually go to a hospital rather than a medical practice), type of study (prospective versus retrospective)

[^C.3.a.6]: These are data in which non-causal information are found in the data via the label, e.g. in the sorting (e.g. first the data of healthy persons, then of ill persons), in the hospital (from one the severe cases originate), in images (e.g. for skin cancer, one must always see a ruler). An additional example would be multiple CT images of a patient, in which the model learns using the patient and not the disease. This could happen if a rib fracture can be seen in addition to the cancer on multiple images.

#### b) Data labeling

| Requirements                                                 | Comments                                                     | Regulatory references|
| :------------------------------------------------------------| :------------------------------------------------------------|:--|
|  In the case of "Supervised Learning", the manufacturer has derived the labels from the intended use with which the training data are provided and justified this choice. |                                                              |
| The manufacturer has defined a procedure for labeling in "Supervised Learning", if labels were not yet present in the data.   | | ISO 13485, 4.1 |
| This procedure specifies quantitative classification criteria for labeling. The selection of these criteria has been justified by the manufacturer[^C.3.b.1]. | If the "Ground Truth” is not selected[^C.3.b.2], because it is too expensive or invasive, this must also be justified. |                                                            |
| This procedure specifies the requirements for the number, training and competency for the people responsible for labeling. |   ISO 13485, 6.2 and 7.3.2, FDA 21 CFR part 820.25  |                                                         |
| This procedure sets forth how the competencies of the persons responsible for labeling is tested. | This can be done by the labeling of selected data sets.      |
| This procedure sets forth how the persons responsible for labeling are trained and how the success of this training is evaluated. |                                                              |
| This procedure sets forth how the correctness of the label is systematically reviewed. The selection of this justification has been documented by the manufacturer. | The manufacturer can provide identical data sets of multiple persons and assess the consistency of the results. |
| This procedure sets forth, how the monitoring occurs, that the persons responsible for labeling are continually fit and willing to perform the labeling [^C.3.b.3]. | This can be done with datasets with already known labels that are inserted unnoticed by the person during labeling. |

[^C.3.b.1]: If, for example,  patients have to be classified as healthy and sick, the manufacturer must derive the criteria specifically for the intended use, when a patient is to be classified as healthy and when as sick.

[^C.3.b.2]: The “Ground Truth” is the most precise reference method (state of the art). For the determination of arterial hypertension, an invasive blood pressure measurement may provide the most exact results.

[^C.3.b.3]: The labeling of dozens of data sets is arduous. A payment per data set can cause an inappropriate motivation.

#### c) Procedure for (pre-)processing of data

| Requirements                                                 | Comments                                                     | Regulatory references|
| :------------------------------------------------------------| :------------------------------------------------------------|:--|
| The manufacturer has set a procedure that describes the pre-processing of the data. |   | ISO 13485:2016, 4.1.6, 7.3.6, XAVIER University "Building Explainability and Trust for AI in Healthcare", FDA 21 CFR part 820.70(i)   |
| This procedure describes the individual processing steps such as conversion, transformation, aggregation, normalization, format conversion, calculation of feature, conversion of numerical data into categories. | A graphic representation creates a rapid overview. The conversion of numerical to categorical values requires a justification. | | ISO 13485:2016, 4.1.6, 7.3.6, XAVIER University "Building Explainability and Trust for AI in Healthcare", FDA 21 CFR part 820.70(i)     |
| The procedure describes how the correctness of the interim steps and the final results are assessed[^C.3.c.0] through risk-based evaluations. | This is consistent with the requirements of ISO 13485:2016 chapter 4.1.6. The risk management file must contain these analyzes. |
| This procedure specifies how values with various measurement scales or units are detected and processed. | This depends on the ML-method used (e.g. tabular data / image data) and cannot be demanded as a general best practice.  |                                                            |
| This procedure specifies how values are detected and processed that have been collected with various measurement methods. | This depends on the ML- method used (e.g. tabular data / image data) and cannot be demanded as a general best practice.       |                                                     |
| This procedure specifies how values or metadata with the same names (such as in column headers) are detected and processed. | This, however, depends on the ML-method used (e.g. tabular data / image data) and cannot be demanded as a general best practice. |
| This procedure specifies how missing values within data sets are detected and processed. The manufacturer gives a rationale for the decision[^C.3.c.1]. | Make sure that the rationale differentiates between “missing at random” and “missing not at random”[^C.3.c.2]. |                                                        |
| This procedure specifies how outliers are detected and processed[^C.3.c.3]. The manufacturer gives a rationale for the decision[^C.3.c.4]. | Show example of a date / feature. This, however, depends on the ML-method used (e.g. tabular data / image data) and cannot be demanded as a general best practice. |
| This procedure specifies how unusable data sets are detected and handled[^C.3.c.5]. The determination was justified by the manufacturer. | Request example of a date / feature.                         |
| The manufacturer has identified, assessed, and managed the risks arising from data processing. | Risks can be caused, for example, by software errors, rounding errors, re-sampling and compression of data, and the sorting out of invalid data. |  AI4H-DAISAM | 

[^C.3.c.0]: Options include software tests and redundant or alternative calculations such as with Excel.

[^C.3.c.1]: The options for processing include deleting the data set, replacement by the average value of other data sets, new value “missing” (for categorical values).

[^C.3.c.2]: An example for "missing not at random” is lab values that are too high that are cut off.

[^C.3.c.3]: The options for processing include deleting the data set, correcting the value, setting the value to a set value (min/max).

[^C.3.c.4]: This justification is more important in the regression method than with tree-based methods.

[^C.3.c.5]: Examples are x-rays of poor quality or patients who do not meet the inclusion criteria.

#### d) Documentation and version control

| Requirements                                                 | Comments                                                     | Regulatory references|
| :------------------------------------------------------------| :------------------------------------------------------------|:--|
|  The manufacturer has described the "funnel", which shows how much data originates from which data sources (e.g. clinics) and at which processing step how many data records were dropped and for what reason.              |                                                              |
| The manufacturer has described which parts of the software are responsible for which processing step. | This should be part of the architecture of this software.  |                                                              
| The manufacturer has described the processed data using descriptive statistics [^C.3.a.4]. | ["Dataset Nutrition Label"](https://ahmedhosny.github.io/datanutrition/) is recommended.|                                                              
| The manufacturer has all software for data processing, including the libraries used in the process, documented and under version control. ||  ISO 13485, 4.1.6., 4.2.4., 7.5.6. |

### 4. Model development 

#### a) Preparation

| Requirements                                                 | Comments                                                     | Regulatory references|
| :------------------------------------------------------------| :------------------------------------------------------------|:--|
| The manufacturer has justified the selection of features that it considers during training. | This requires a list of all features.  | ISO 13485, 7.3.2., 7.3.3. |
| The manufacturer has described the dependency of the features among each other, especially for tabular data. | A Directed Acyclic Graph (DAG) helps with the visualization. This depends on the applied ML-method and cannot be demanded as a general best practice. | ISO 13485, 7.3.2., 7.3.3. |
| The manufacturer has documented and justified the ratio that it divides up the data into training, validation and test data. |                                                              |
| The manufacturer has documented the stratification it uses to divide up the data in to training, validation and test data[^C.4.a.1]. |                                                              |
| The manufacturer has documented how he ensures that multiple data sets for an object are in the same “bucket” (training, validation and test data). |                                                                                                  |                                                     |
| The manufacturer has documented how he ensures that test data are not used for model training and validation. |                                                              |                                                            |
| The manufacturer has described when it recodes the data specifically for the model or specifically for the library[^C.4.a.2]. |                                                              |

[^C.4.a.1]: For data with rare features or labels, it may be necessary to distribute the data not just at random.

[^C.4.a.2]: Examples of this are normalization, selection of class labels (e.g. 0 or 1), selection of column names, distribution of categorical values over multiple columns.

#### b) Training

| Requirements                                                 | Comments                                                     | Regulatory references|
| ------------------------------------------------------------ | ------------------------------------------------------------ | -- |                    
| The manufacturer performs model training, tuning of hyperparameters and model selection exclusively with the training and validation data (e.g. using cross-validation). |  The manufacturer should also show that the training actually improves the quality of the model.   |                                                         |
| The manufacturer tried different sets of hyperparameters and documented his final choice.[^C.4.b.1]. |                                                              |                                                           |
| The manufacturer has documented the choice of epochs[^C.4.b.2].  |       |
| The manufacturer has determined, documented and justified the quality dimensions on the basis of the intended use for which he wants to optimize the model. | This means that the choice of these quality parameters is specific to the intended use. |
| The manufacturer has - as far as reasonable - trained and compared several model types (including simpler and interpretable model). |   |

[^C.4.b.1]: Examples: Loss function, optimizer, learning rate, number of epochs

[^C.4.b.2]: It can be useful to show the dependence of the quality of the model on the number of epochs by means of learning curves. These learning curves exist, for example, for neural networks and boosting methods, but not for models with numerical solution (e.g. linear regression) or with a single tree.	

#### c) Evaluation

| Requirements                                                 | Comments                                                     | Regulatory references|
| ------------------------------------------------------------ | ------------------------------------------------------------ |--|
|The manufacturer has planned the evaluation of the model.| This plan can be part of a development or V&V plan. | ISO 13485, 7.3.2, 7.3.6 and 7.3.7, 
ISO 14971:2019, 10. |
|The manufacturer has documented the quality measures for the various models, e.g. in the case of a binary classification using a four-field table. | This documentation should not only include the values to which the manufacturer has optimized the model. |
|The manufacturer has not only evaluated and documented the quality measures for the different models globally, but also separately for different features, if applicable. | |
|The manufacturer has shown how to recognize and thus avoid overfitting. | | ISO 24028 9.8.2.23 |
|The manufacturer has examined the data sets that were predicted particularly well and those that were predicted particularly poorly. | A residuals analysis is recommended, in which the errors are plotted against the feature values, if applicable. |
|The manufacturer has examined the data sets for which the model is particularly safe and particularly unsafe[^C.4.c.1]. | |
|The manufacturer has justified the ultimate choice of model on the basis of the quality criteria and the intended use, and has explained in particular when simpler and more interpretable models were not used. |  | ISO 14971:2019, XAVIER University "Building Explainability and Trust for AI in Healthcare", DIN SPECT 2 |
|The manufacturer has considered, especially for tabular data for individual data sets, to have the model show the features that particularly influenced the decision [^C.4.c.2]. | This cannot be claimed as a general best practice. |
|The manufacturer has considered evaluating, especially for tabular data, how and how much individual features would have to change for the model to come to a different prediction. | This is referred to as ["counterfactuals"](https://christophm.github.io/interpretable-ml-book/counterfactual.html). This cannot generally be claimed as a best practice. 
|The manufacturer has considered analyzing/visualizing the dependence (strength, direction) of the predictions on the feature values, especially for tabular data [^C.4.c.3]. | This cannot be claimed as a best practice in general. |
|The manufacturer has considered synthesizing data sets that particularly activate the model[^C.4.c.4]. | This cannot be generally claimed as best practice. |
|The manufacturer has considered approximating the model with a simplified surrogate model such as a decision tree. | This cannot generally be claimed as best practice. |

[^C.4.c.1]: Classification tasks must take into account the current state of research.

[^C.4.c.2]: Approaches include LIME (Local Interpretable Model-agnostic Explanations), Beta (Black Box Explanations through Transparent Approximations), LRP (Layer-wise Relevance Propagation) and Feature Summary Statistics (incl. Feature Importance and Feature Interaction).

[^C.4.c.3]: Examples of Sharpley-Values, ICE-Plots, Partial Dependency Plots (PDP)

[^C.4.c.4]: For examples see http://yosinski.com/deepvis

#### d) Documentation

| Requirements                                                 | Comments                                                     |Regulatory references|
| ------------------------------------------------------------ | ------------------------------------------------------------ |--|
| The manufacturer has the model[^C.4.d.1] and/or the training code under version and configuration control. | That includes scripts and build files.   | ISO 13485, 4.1.6., 4.2.4., 7.5.6. |
| The manufacturer has documented his code according to a policy. | Usually at least public class, methods with pass and return values as well as attributes are to be documented |
| The manufacturer has described which data sets it used for training, validation and testing of the model. |  |ISO 24028 9.8.2.1, DAISAM|
| The manufacturer can reproduce the test and validation results. | For this purpose, it makes sense to use a version management system not only for the code, but also for data, test results and their evaluation. It is advisable to also document the infrastructure used in data processing and training (hardware, operating system, virtualization layers such as Docker). Any deviating results should be justified (e.g., hardware, random generators, rounding errors). Absolute paths and operating system specific commands are to be avoided. A README file in .txt or Markdown format helps to find your way around the documentation more quickly. |                                                               
| The manufacturer has the SOUP (libraries and frameworks) under version and configuration control. | | IEC 62304, 8.1.2. | 
| The manufacturer has documented the architecture of the model and the model itself including its algorithms and hyperparameters. | For example, in the case of a CNN, the number and type of layers, the linkage of the neurons or layers, the activation function, the optimizer and other parameters including their value ranges should be documented, among other things. The documentation of the model also includes the specification of the outputs such as the number of outputs, the respective data types, value ranges, units, etc.. | ISO 13485, 4.2.3., 4.2.5. |
| The manufacturer has described how it selected the architectures, trained the models, and optimized the hyperparameters, and justified this procedure. | Auditors want to be able to understand how the manufacturer has proceeded and why the chosen solution is the best. IEC 62304 and the FDA do not want "ad hoc design decisions".  |                                                              
| The manufacturer has described when it worked with a “pretrained model” and shown why this “pre-training” is suitable for the task. |                                                              |
| The manufacturer has documented the quality of the models based on the quality measures. | These quality metrics relate to the testing with the test data. | ISO 13485, 4.2.3., 4.2.5. |
| The manufacturer has specified the confidence intervals for the quality parameters depending on the input data. | Especially at the edges of the allowed input data, the confidence often decreases strongly. This information should also be provided to the users in the accompanying materials. |
| The manufacturer has documented, especially for tabular data, within which limits (e.g. feature values) the model achieves the requirements for the quality measures. | This depends on the applied ML-model and cannot be generally claimed as best practice. |  ISO 13485, 4.2.3., 4.2.5. |                         
| The manufacturer has tried out several models and their hyperparameters and documented the aspects mentioned in this section for them. | This documentation serves the manufacturer to compare different models and to justify his choice of a model. This is necessary to fulfill the requirement of ISO 14971 to maximize the risk-benefit ratio. |

[^C.4.d.1]: Trained models can be serialized.

### 5. Product development

#### a) Software development

| Requirements                                                 | Comments                        | Regulatory references|
| ------------------------------------------------------------ | ------------------------------- |--|
| The manufacturer has performed the required activities pursuant to IEC 62304 and documented them. | Notes for auditors[^C.5.a.1] | IEC 62304, IEC 82304, XAVIER University "Building Explainability and Trust for AI in Healthcare", FDA guidance on software validation, FDA OTS guidance  |
| If the manufacturer has implemented the model in another programming language or for another runtime environment, it has created a plan that repeats the activities pursuant to chapter 4. |  | IEC 62304, IEC 82304 |
| The manufacturer checks the performance (response times, resource consumption) on the target hardware (e.g. browser, mobile device). | 2017/745/EU, Annex I, 17.1., 17.3., 2017/746/EU, Annex I, 16.1., 16.3. |
| The manufacturer has described how all SOUP and OTS components are to be verified and has also carried out and documented this verification. | | IEC 62304, 5.3, 8.1.2, FDA OTS guidance |
| The manufacturer has attached the prescribed license conditions to the software and ensured the legality of the use of third-party software (e.g., open source software). | Manufacturers often use open source software, which may only be used within the scope of licenses and copy right statements. |

[^C.5.a.1]: The manufacturers should adhere to the normal best practices such as adherence to coding guidelines, review of code by code reviews using defined criteria, testing to code with unit tests with a defined coverage, etc.  A description of the code (architecture) should make it easy to understand which code performs which task.


#### b) Accompanying materials

| Requirements                                                 | Comments                                                     | Regulatory references|
| ------------------------------------------------------------ | ------------------------------------------------------------ |--|
| The instructions for use clearly identify the version of the product. | If possible, indicate the UDI. | 2017/745/EU, Annex I, chap. III, 23.1, 23.4., FD&C, FDA 21 CFR parts801 and 820.120, ISO 24028 e.g. 10.11.3 |
| The instructions for use describe the intended use of the product including the expected medical benefit. |   | 2017/745/EU, Annex I, chap. III, 23.1, 23.4., 21 CFR part 801, 21 CFR part 814.20, XAVIER: "Perspectives and Good Practices for AI and Continuously Learning Systems in Healthcare", ISO 24028, XAVIER University "Building Explainability and Trust for AI in Healthcare", ISO 24028 e.g. 10.11.3|
| The instructions for use specify the intended patient population using indications, contraindications and if relevant using other additional parameters such as age, gender, accompanying diseases or availability of information. | | 2017/745/EU, Annex I, chap. III, 23.1, 23.4. |
| The instructions for use explicitly list the patients / data / use case for which the product may not be used. |   | 2017/745/EU, Annex I, chap. III, 23.1, 23.4. |
| The instructions for use document the requirements of the input data (including formats, resolutions, value ranges, etc.). |                                                              |
| The instruction for use specify the intended primary and secondary users pursuant to intended use. |                                                              |
| The instructions for use describe the other conditions applicable to the product (e.g. runtime environment, use environment). |    
| The instructions for use describe how the product is to be used. | This also includes behavior in the event of an error and secondary use such as installation, upgrade and configuration. |
| The instructions for use describe the possible outputs. | This also includes the explanations of the product ("Explainability"). |
| The instructions for use describe the residual risks.        |    | 2017/745/EU, Annex I, 23.4, ISO 14971:2019, 8, ISO 24028 e.g. 10.11.3 |
| The instructions for use indicate the data with which the model was trained. | This is related both to the patient collective and to the features used. |
| The instructions for use describe the model and algorithms.  |                                                              |
| The instructions for use name the quality metrics.   |  Also specify confidence ranges here.                                                         |
| The instructions for use list the factors that could have a negative effect on the product's performance. |                                                              |
| The instructions for use specify whether the product is further trained during use. | Please observe notes in the chapter on continuous learning systems.  |                                                              |                                                              |
| The instructions for use describe how to update the product. |                                                              |
| The instructions for use contain references to additional literature. |                                                              |
| The instructions for use contain references to licensing rights. |    | 2017/745/EU, Annex I, 23.4, EU-Regulation 207/2012|
| The instructions for use identify the manufacturer and lists channels for posing questions. |  |  2017/745/EU, Annex I, 23.4, EU-Regulation 207/2012|
| The instructions for use list possible ethical problems.     | |
| The instructions for use contain the URL under which the most current versions of the instruction of use can be found. |    | 2017/745/EU, Annex I, 23.4, EU-Regulation 207/2012| 


#### c) Usability validation

|Requirements                                                  |Comments| Regulatory references|
| ------------------------------------------------------------ | --------- |--|
| As part of the usability validation, the manufacturer assesses whether users understand the instructions for use. | This includes other accompanying materials.  | IEC 62366-1, FDA HFE guidance |
| As part of the usability validation, the manufacturer evaluates whether the users blindly trust the product or verify the results. | | IEC 62366-1 |
| As part of the usability validation, the manufacturer evaluates whether users correctly recognize and understand the results. | This also includes the display of errors and the explanations ("explainability"). Manufacturers should include all safety-related use scenarios in the validation and all risk-minimizing measures on the interface. | IEC 62366-1, 5.7-5.9 |


####  d) Risk management

| Requirements                                                 | Comments | Regulatory references|
| ------------------------------------------------------------ | -------- |--|
| The manufacturer has evaluated the risks that arise if the inputs do not meet the specified requirements[^C.2.a.2]. |       |  ISO 14971:2019, 5.4,  IEC 62304, 7.1, DIN SPEC 2, IEC 82304 4.1.c) | 
| The manufacturer has derived the quantitative quality criteria based on the state of the art. | The manufacturer shall be able to name the quality criteria for alternative technologies and procedures and to argue if the medical device is not superior to the alternatives with respect to the quality criteria [^C.5.d.1]. | |       |          |
| The manufacturer has defined the gold standard and justified its choice, which will be used to verify the quality criteria. |   | XAVIER University "Building Explainability and Trust for AI in Healthcare", FDA proposed regulatory framework for modifications to AI/ML based SaMD: "reference standard" |
| The manufacturer has identified, evaluated, and managed risks that arise when outputs do not meet the specified quality criteria. | In this analysis, the manufacturer also considers the specific properties of the selected model as well as the confidence intervals of the output values determined during testing. | ISO 14971:2019, 5.3, IEC 62304, 7.1, IEC 82304, 4.1.c), XAVIER University "Building Explainability and Trust for AI in Healthcare", FDA guidance on software validation, 5.2.2 |
| The manufacturer has evaluated the consequences if the system provides socially unacceptable outputs (e.g. discriminatory). | These "consequences" are not necessarily risks in the sense of ISO 14971. | Ethics guidelines for trustworthy AI |
| The manufacturer has identified, evaluated and managed the risks if the system is not available. |   
| The manufacturer has identified, evaluated and managed the risks arising from software errors. | This includes errors in SOUP as well as in the software used for "pre-processing" the data and for training the model. | 
| The manufacturer has identified, evaluated and managed the risks arising from the specific choice of model architecture. | In doing so, manufacturers should also analyze whether the models have been optimized to the right specifications. | ISO 14971:2019 |
| The manufacturer has identified, evaluated, and managed the risks posed by the specific choice of target platform. | For example, the target platform might not provide the required computing power or might cause the software to crash. |
| The manufacturer has identified, evaluated and managed the risks arising from the selection of training, validation and test data. | This concerns both the sources of these data (such as patients, institutions) and the division of these data into training, validation and test data. For example, manufacturers should check that there is no overfitting or bias of the data. |
| The manufacturer has identified, evaluated and managed the risks of outputs (predictions, classifications, etc.) being correct only by chance. | Interpretability allows manufacturers to demonstrate why an ML-model has made a specific decision. |
| The manufacturer has identified the risks posed by the fact that the predictions themselves change the predicted outcomes. | In this phenomenon, the model changes from observer to actor [^C.5.d.2]. It is called "performative prediction." Producers should investigate the possible effects on people or systems and describe them e.g. with a DAC ("directed acyclic graph"), observe a possible "distribution shift" and, if necessary, an unaffected control group, and take action if necessary such as choosing a different model or re-training the existing model. |
| If the manufacturer uses self-tests, he has explained which of the specified quality criteria are checked with them and which risks are thereby controlled. | |
| The manufacturer has identified, evaluated and managed the risks from usage errors. | These risks should also take into account that users do not recognize or misunderstand the explanation of the outputs ("Explainability"). | IEC 62366-1, 5.3f, FDA HFE guidance, FDA guidance on software validation, 5.2.3 | 
| The manufacturer has identified, evaluated and controlled the other risks mentioned in chapter C.1.d). |   | 

[^C.5.d.1]: State-of-the-Art does not necessarily correspond to the Gold Standard, which in turn does not necessarily correspond to the Ground Truth. I.e., the system requirements may be lower than for a gold standard or ground truth, especially if the latter requires an invasive or very costly procedure.    
[^C.5.2.d]: Examples of this phenomenon can be found [here](https://mindfulmodeler.substack.com/p/correction-you-can-break-a-predictive).  

#### e) Clinical evaluation

|Requirements                                                  |Comments| Regulatory references|
| ------------------------------------------------------------ | --------- |--|
| As part of the clinical evaluation, the manufacturer has evaluated whether the promised medical benefit is achieved for the given quality parameters. || 2017/745/EU, Article 61, Annex XIV and Annex XV, 2017/746/EU, Annex XIII and Annex XIV, MEDDEV 2.7/1 rev.4, XAVIER University "Building Explainability and Trust for AI in Healthcare", FDA 21 CFR part 820.30(g)|
| As part of the clinical evaluation, the manufacturer has evaluated whether the promised medical benefits and risks are in line with the state of the art. | | 2017/745/EU, Article 61, Annex XIV and Annex XV, 2017/746/EU, Annex XIII and Annex XIV, MEDDEV 2.7/1 rev 4, ISO 14971:2019, 4.2  |


### 6. Product release

|Requirements                                                  |Comments| Regulatory references|
| ------------------------------------------------------------ | --------- |--|
| The manufacturer has ensured that all the above documentation is available. | This concerns, among other things, the documentation required in chapters 3.d), 4.d and 5.b). | 2017/745/EU, Annexes I and II, ISO 13485 e.g. 7.3.5
FDA 21 CFR part 820.30(e)
| The manufacturer has assessed the risks as acceptable in risk management and documented that all activities specified in the risk management plan have been carried out. | Note for auditors [^C.6.1] |
|The manufacturer has outlined in the Software as a Medical Device Pre-Specifications (SPS) what types of changes it anticipates for systems that it wishes to market in the USA[^C.6.2]. |  
| The manufacturer has shown in Algorithm Change Protocol (ACP) how it will perform these changes for systems that it wishes to market in the USA[^C.6.3]. |                            |
| The manufacturer has created a Post-Market Surveillance Plan, see below. |                            |

[^C.6.1]: Using examples, check that the efficacy of risk management measures was tested so that there is a traceability of risks for risk control measures.

[^C.6.2]: Changes may affect the intended use, the input data and the clinical and analytical performance.

[^C.6.3]: The approach must, for example, address handling data, re-training, the performance and the updates.

## D) Requirements for the phases downstream of development

#### 1. Production, Distribution, Installation

|Requirement|Comments| Regulatory references|
|:--|:--|:--|
|The manufacturer has described how it ensures that only exactly the intended artefacts (files) in exactly the intended version of the product or as a product are delivered.|This is configuration management. Also relevant to downloads or AppStores.| IEC 62304, 5.8.8. |
|The manufacturer has described how the persons responsible for the installation know which is the latest version and how confusion during installation can be ruled out. |This is only relevant for stand-alone software. Here, a procedure or work instruction would be expected.| ISO 13485, 7.8.3., 8.3.,  IEC 62304, 5.8.4. |
|The manufacturer has described how it will be ensured during installation that the requirements specified in the accompanying materials (see above) are actually met.|A procedural or work instruction would be expected here.| ISO 13485, 7.5.3. |
|The manufacturer has established procedures that ensure that it can communicate with the operators and users of its product in a timely manner.|| ISO 13485, 7.2.3., 8.3.3., IEC 82304, 8.4. |


#### 2. Post-Market Surveillance

|Requirements|Comments| Regulatory references|
|:--|:--|:--|
|The manufacturer has created a Post-Market Surveillance (PMS) Plan.|| 2017/745/EU, Chapter VII, 2017/746/EU, Chapter VII |
|The manufacturer has specified the data it wishes to collect and analyze in this PMS plan.|| 2017/745/EU, Chapter VII, 2017/746/EU, Chapter VII |
|The manufacturer has specified in the PMS plan the quality criteria and threshold values that it considers necessary for handling of in particular a re-evaluation of the risk-benefit analysis.|| 2017/745/EU, Chapter VII, 2017/746/EU, Chapter VII |
|The manufacturer has analyzed when determining these threshold values which feedback loops the threshold values can influence[^D.2.1].|This analysis also serves as a measure against the above risk through "Performance Prediction".| 2017/745/EU, Chapter VII, 2017/746/EU, Chapter VII |
|The manufacturer has analyzed when determining these threshold values which self-fulfilling prophecies the threshold values can influence[^D.2.2].|| 2017/745/EU, Chapter VII, 2017/746/EU, Chapter VII |
|In the PMS plan, the manufacturer described how it collects and analyzes information on adverse medical effects.|| 2017/745/EU, Chapter VII, 2017/746/EU, Chapter VII |
|In the PMS plan, the manufacturer described which information on (adverse) behavioral changes or (predictable) misuse is collected and analyzed[^D.2.3].|| 2017/745/EU, Chapter VII, 2017/746/EU, Chapter VII |
|In the PMS plan, the manufacturer described how it collects and analyzes information on additional “adverse effects” [^D.2.4].|| 2017/745/EU, Chapter VII, 2017/746/EU, Chapter VII |
|The manufacturer has described in the PMS plan how it collects information to be able to analyze whether the data in the field is consistent with the expected data or training data[^D.2.5].|Note for auditors[^D.2.6]| 2017/745/EU, Chapter VII, 2017/746/EU, Chapter VII |
|In the PMS plan, the manufacturer has described how and how often it wants to collect information on whether the product still meets the state of the art.|Note for auditors[^D.2.7]| 2017/745/EU, Chapter VII, 2017/746/EU, Chapter VII |
|In the PMS plan, the manufacturer has described how and how often it wants to collect information on whether the “Ground Truth” or the gold standard are still up to date.|| 2017/745/EU, Chapter VII, 2017/746/EU, Chapter VII |
|In the PMS plan, the manufacturer has described how and how often changes pursuant to the Algorithm Change Protocol (ACP) and within the “SaMD Pre-Specifications” (SPS) are made.|| 2017/745/EU, Chapter VII, 2017/746/EU, Chapter VII |
|The reports required by the plans are available at the times specified therein.|zBsp. PSUR|

[^D.2.1]: Examples for these feedback loops: **Example 1**: A travel recommendation app sends targeted advertising depending on feature (last trip). This influences travel behavior. **Example 2**: An algorithm provides prognoses. Therefore, the physician will treat the patients better or earlier...

[^D.2.2]: Example 1 (criminalistics)

[^D.2.3]: Example: Radiologists rely on the software and don't look at the images anymore, so they overlook findings.

[^D.2.4]: Examples would be ethical challenges such as the YouTube algorithm, which achieves the goal, maximizing the click count or use duration, but promoting violence and conspiracy videos.

[^D.2.5]: One speaks here of a distribution shift or data drift.

[^D.2.6:]: The manufacturer should set threshold values for features or for the variance / covariance over time. This allows visualization or quantification in particular for non-normally distributed data over the comparison of histograms or core density estimations.

[^D.2.7]: For example, have the manufacturer explain the process on how it is systematically informed of new developments in machine learning, and how it assesses these developments and reacts to them.



#### 3. Decommissioning


|Requirements|Comments| Regulatory references|
|:--|:--|:--|
|The manufacturer has created a decommissioning plan before withdrawing its product from the market. | Such a plan specifies, for example, whether and how the software must be uninstalled, whether data must be backed up or exported, how the confidentiality of the data remains guaranteed, who is responsible for these activities, how the progress of the decommissioning is monitored and ensured, and which organizations must be informed and how.| ISO 24028 |
|The manufacturer identifies, evaluates and controls the risks arising from decommissioning. | This is to be evaluated in the risk management file. Risks from the unavailability of the product, from usage errors and from an influence on other products should be considered.|  2017/746/EU Annex I, 3., ISO 14971:2019 chapter 10 in combination with 3.8 and 3.12, ISO 24028 |


## E) Annexes

### 1. Additional literature

#### a) Laws

- [Medical Device Regulation](https://eur-lex.europa.eu/legal-content/DE/TXT/?uri=uriserv:OJ.L_.2017.117.01.0001.01.DEU&toc=OJ:L:2017:117:FULL) MDR
- [In-vitro Diagnostic Device Regulation](https://eur-lex.europa.eu/legal-content/DE/TXT/?uri=uriserv:OJ.L_.2017.117.01.0176.01.DEU&toc=OJ:L:2017:117:FULL) IVDR

#### b) Standards and Best Practice Guides

- **IEC 62304/AMD1**, Medical device software – Software life cycle processes
- **IEC 82304-1**, Health software – Part 1: General requirements for product safety
- [FDA Guidance Documents on Machine Learning](https://www.fda.gov/medical-devices/software-medical-device-samd/artificial-intelligence-and-machine-learning-software-medical-device)

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
11. Do increase practicability, the authors have avoided collating many requirements to the greatest extent possible. Rather, they have limited themselves to those that they consider particularly relevant and implementable.
12. And to promote distribution and the level of familiarity, the guideline must be available and remain available at no cost.
13. The guideline should be available in German and English.
