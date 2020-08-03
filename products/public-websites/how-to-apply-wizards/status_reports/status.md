### 7/31 Status Meeting with Wizard Product/Development Leads
** Participants:
- John Hashimoto (Public Websites)
- Leah Keeler (GI Bill & Other Education - 1990)
- Luke Majewski (Higher Level Review/20-0996 & Disability Compensation/21-526ez )
- Jason Wolf (Personalized Career Planning/Chapter 36)
- Matt Self was unable to attend

** Topics:

- The collab cycle process/kick-off did not happen prior to dev start and as a result we are moving quickly to close that gap.  This may have implications on the dev work already committed.
  - Our goal: To [unify the collab cycle process](https://github.com/department-of-veterans-affairs/va.gov-team/issues/7549) as much as possible across the various efforts to ensure we leverage commonalities and avoid future speed bumps.
- Teams also provided updates on their timelines with the possibility that Public Websites might take-up the Disability effort if necessary to maintain momentum.

## Meeting Notes

- There are two active development projects involving "how to apply Wizards" -- Education and Personalized Career Planning/Chapter 26.  The work on HLR and Disability has been delayed due to other priorities.
  - Per Leah Keeler, the [Education Wizard dev work](https://github.com/department-of-veterans-affairs/va.gov-team/issues/11227) is nearly complete and could be deployed as soon as the week of August 10th -- assuming no issues.
  - Per Jason Wolf, the [Personalized Career dev work] is complete and in staging.
  - Per Luke Wajewski, the HLR and Disability work has not yet been initiated but he believes the work is bound/integrated, so there would be no great benefit in uncoupling the effort (e.g. Public Websites taking on the Disability Wizard work).
- The Education work (via Mahariel Rosario) did result in some valuable new enhancements/updates to the code that could be leveraged by the other teams and Leah will connect the dev leads from Education and HLR/Disability to collaborate. Details:
  - First, I created a WizardContainer component and placed that on the introduction page.  The WizardContainer holds the content surrounding the wizard and renders the actual Wizard .
  - The Wizard takes in the radio button components (called pages) and renders out the next page depending on where you are in the wizard.
  - I then created  setWizardStatus and setBenefitReferred functions and their get counterparts.
  - This approach allows any form that wants to use the same questions, content,  design, and display logic as the education benefits wizard to reuse the wizard container I made.
  
