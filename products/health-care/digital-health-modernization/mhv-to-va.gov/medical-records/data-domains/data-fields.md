**Medical records domains**
|Blue Button label | Suggested label|
|:------|:-------|
|VA Immunizations  |Vaccines|
|VA Allergies |Allergies|
|VA Problem List |Health conditions|
|VA Vitals and Readings|Vitals|
|VA Laboratory Results <br> VA Pathology Reports <br> VA Radiology Reports <br> VA Electrocardiogram (EKG) Reports |Lab and test results|
|VA Admissions and Discharges <br> VA Notes|Care notes and summaries|

**Vaccines**
|Data field       | Description           | Suggested label | Notes             | Questions           
|:------------------------|:-----------------------|:-----------------------|:-------------------|:---------------------|
|Immunization | Name of the vaccine | Vaccine | 
|Date received | Date patient got vaccine dose | Date |
|Location | Name/address/clinic code of facility where they got vaccine dose | Location |
|Reaction | Reactions or side effects to the vaccine recorded by provider | | Vaccine reactions may also be stored in allergies list and self-entered data |How often does a vaccine reaction appear in allergy list instead of this field? |
|Comments | Comments entered by provider | Provider notes | 
|Series | Info about vaccine series, if relevant | Series | May need explanatory text here. <br /> <br /> Vaccines in a series won't be grouped or linked in MVP version. | How does series data display — "COVID booster 1 of 2" or some other format? |

**Allergies**
|Data field       | Description           | Suggested label | Notes             | Questions|           
|:------------------------|:-----------------------|:-----------------------|:-------------------|:---------------------|
|Allergy name | Thing that caused the allergic reaction, like "penicillin" |Allergy |
|Date entered | Date provider entered the allergy record | Date entered | 
|Severity | Level of reaction, like "moderate" or "severe" | | |Are there set options to choose from in this field, or is it free entry?|
|Allergy type | The type of thing that caused the allergy, like "drug" for penicillin | | |Are there set options to choose from in this field, or is it free entry?|
|VA drug class | | | |What does this mean? Is there a list of classes to choose from?| 
|Reaction | Description of signs and symptoms, like "rash" |
|Observed/Historical || | |Does this mean the provider witnessed the reaction (observed) vs entered an allergy record based on patient's account of a previous allergic reaction? |
|Location |Name of facility where provider entered allergy record | Location | 
|Comments |Comments entered by provider | Provider notes | 

**Health conditions**
|Data field       | Description          | Suggested label | Notes             | Questions           |
|:------------------------|:-----------------------|:-----------------------|:-------------------|:---------------------|
|Issue/problem title |Name of the health condition | Health condition |
|Date/time entered | | | |Why is time important here? Can we display only date?|
|Status | | | |Are the only options active and inactive?|
|Location where the issue was entered |Name of facility |Location | |Is this field only necessary for the user to associate it with a specific appointment they had? What if it were a telehealth appt?|
|Provider's name | |Provider |
|Comments |Comments entered by provider |Provider notes |

**Vitals**
|Data field       | Description           | Suggested label | Notes             | Questions           |
|:------------------------|:-----------------------|:-----------------------|:-------------------|:---------------------|
|Category name | 
|Latest reading |
|Date of latest reading |
|Location of latest reading |
|Reading |
|Date of entry |
|Location of entry |
|Comments |

**Lab and test results**
|Category |Data field| Suggested label | Notes | Questions |
|:----------------|:-------------|:----------------|:------------------|:--------------------|
|All |Category |Type of test | |Is this information useful for patients? Could we remove this from the list view?|
|All|Title of lab report (if available)|Test (suggest using this without a label as the card header in list, H1 in detail) |If there's no title/test name available, we could conditionally display the type of test as the card header in list, H1 in detail. Hopefully this is rare. |
|All|Date collected |Date |
|All|Ordering provider |Provider who ordered the test |
|Radiology|Procedure/test name |Test ||Is this the same as "Title of lab report" in the All category above?|
|Radiology|Date/time exam performed |Date you got the test |
|Radiology|Ordering location| Where the test order started |
|Radiology|Requesting provider| Provider who ordered the test | | | In Chem/Hem and Microbio, the field is labeled “Ordering Provider”. Should this change?|
|Radiology|Reason for study| Reason for the test |
|Radiology|Performing location| Where you got the test |
|Radiology|Clinical history| | | |What does this mean? Is this medical history related to the reason for this test? |
|Radiology|Radiologist|
|Radiology|Report| | | |What does this mean? Is this where results are entered? |
|Chemistry/hematology|Lab test name (if avail)| Test (suggest using without label as card header in list, H1 in detail) |
|Chemistry/hematology|Date/time collected| Date and time you gave the sample |
|Chemistry/hematology|Specimen| Sample tested |
|Chemistry/hematology|Specific test-name| Test |
|Chemistry/hematology|Specific test-results| Results |
|Chemistry/hematology|Specific test-Units| Units | | |Can we remove the "Units" field, and add the units to the result and reference range?|
|Chemistry/hematology|Specific test-Reference range| Standard range ||Does the reference range adjust based on patient demographics or conditions?|
|Chemistry/hematology|Specific test-Status| | | |Under what circumstances would "status" be anything other than final? Can we remove this field?|
|Chemistry/hematology|Specific test-Performing location| Lab that analyzed the sample|
|Chemistry/hematology|Specific test-Interpretation| | | | What types of information does this include? What guidance do providers see for field? <br> Who inputs this and the comments field? Ordering provider? PC? Lab technician? We don't want the user to think they can add their own comments.|
|Chemistry/hematology|Ordering provider| Provider who ordered the test |
|Chemistry/hematology|Ordering location| Where the test order started |
|Chemistry/hematology|Collected location| Where you gave the sample |
|Chemistry/hematology|Comments| | | |How is this different from Interpretation field? |
|Chemistry/hematology|Performing Location| Lab that analyzed the sample | | |It seems that this field is referring to the overall lab results, and not related to individual tests. If all of the tests were performed in other locations, what is this field referring to?|
|Microbiology|Lab type | | | |What types can you choose from here? A: The value will always be "Microbiology" |
|Microbiology|Lab test (aka name, not always present)| Test |
|Microbiology|Date collected| Date you gave the sample |
|Microbiology|Date completed (not always present)| Date completed |
|Microbiology|Results| Results |
|Microbiology|Site/specimen (not always present)| Sample tested |
|Microbiology|Ordering provider| Provider who ordered the test |
|Microbiology|Ordering location| Where the test order started|
|Microbiology|Collected location| Where you gave the sample |
|Pathology|Type of report (surgical pathology/cytology)| Type of pathology test |
|Pathology|Specimen| Sample tested ||
|Pathology|Date obtained| Date you gave the sample | |Does "gave" work in this context? This may happen in the context of surgery, etc, as opposed to going to a lab to give blood|
|Pathology|Performing location| Lab that analyzed the sample |
|Pathology|Date completed| Date completed |
|Pathology|Report| | | |What does this mean? Is this where results are entered? |
|EKG|Procedure/test name| Test | | |For this category, this field will always read "Electrocardiogram (EKG)"|
|EKG|Date/time performed| Date and time of the test |
|EKG|Ordering location| Where the test order started |


**Category labels for labs and tests**
|Category | Suggested label | Notes             | Questions           |
|:----------------------|:----------------|:------------------|:--------------------|
|Chemistry/hematology|||Are all tests in this category blood tests? Would "blood tests" or "routine blood tests" be an accurate label here?|
|Pathology |||
|Microbiology | |This is a subtype of pathology. It looks for bacteria, viruses, fungi, and parasites.|Would "Tests for infections" be an accurate PL label?|
|Radiology | X-rays and imaging tests | 
|EKG |EKG (electrocardiogram) |Historical category |Are new EKGs added to medical records? |


**Care summaries and notes**
|Category|Data field       | Description           | Suggested label | Notes             | Questions           |
|:----------------------|:-----------------------|:--------------------|:------------------|:------------------|:--------------------|
|VA Note|Title|
|VA Note|Date and time|
|VA Note|Location|
|VA Note|Signed by|
|VA Note|Co-signed by|
|VA Note|Date and time signed|
|VA Note|Last updated|
|VA Note|Note|This is the actual content of the note|
|Admission & Dishcarge Summary|Title|
|Admission & Dishcarge Summary|Admission date|
|Admission & Dishcarge Summary|Location|
|Admission & Dishcarge Summary|Admitting physician|
|Admission & Dishcarge Summary|Discharge date|
|Admission & Dishcarge Summary|Discharge physician|
|Admission & Dishcarge Summary|Last updated|
|Admission & Dishcarge Summary|Discharge summary|














