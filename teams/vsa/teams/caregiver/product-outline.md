# Caregivers Product Outline
- GitHub Label: #caregivers
- Slack channel: #vsa-caregivers
- VA.gov link: https://www.caregiver.va.gov/
- Demo video link: n/a
- Product POCs: C.C. Gong, Alayna Abel

---

### Table of Contents

# Executive Summary 
- [User Problem Statement](#user-problem-statement)
- [Solution Goals](#solution-goals)
- [Assumptions](#assumptions)
- [Requirements and Constraints](#requirements-and-constraints)
- [Discovery Takeaways](#discovery-takeaways)
- [Value Propositions](#value-propositions)
- [KPIs-OKRs](#kpis-and-okrs)

# Implementation Information
- [Status](#status)
- [Solution Narrative](#solution-narrative)
- [How to Access and Test](#how-to-access-and-test)
- [Error Handling](#error-handling)
- [Service Level Objective](#service-level-objective)
- [API Calls and Dependent Systems](#api-calls-and-dependent-systems)
- [Resources and Documentation](#resources-and-documentation)
- [Keywords](#Keywords)
- [Team](#team)
- [Screenshots](#screenshots)

---

# Executive Summary

## User Problem Statement

As a caregiver, it's difficult to apply for and manage benefits from the Program of Comprehensive Assistance for Family Caregivers (PCAFC).

## Solution Goals

### User Goals
- Caregivers want to be able to fill out the 1010-CG online.
- Caregivers want to understand PCAFC eligibility and requirements.
- Caregivers want to track the status of their application.
- Caregivers want to be able to manage the benefits for themselves and the Veterans they care for
- Caregivers want to have a single source of information relevant to being a Caregiver.
- Caregivers want to be able to contact a support person from the VA.

### Business Goals
- Feed application data directly to CARMA
- Accomodate the influx of applications that's expected due to changing program eligibility

## Assumptions
- Caregivers and Veterans will fill out the 1010-CG online form rather than the paper form


## Requirements and Constraints
- The paper 1010-CG requires wet signatures from both the Veteran and the Caregiver
- Many caregivers are used to filling out forms on behalf of their veterans
- Caregiver/Veteran relationships may change
- Some Veterans want to give their Caregiver access to all medical and benefits information, while others would not
 

## Discovery Takeaways
- Users like the idea of an online form
- Users like the ability to save the form in progress
- Users like the ability to download a submission receipt
- Mutliple online sources offer conflicting information
- Caregivers like the idea of having an online portal to access support, resources, and benefit information

## Value Propositions

#### User Value
 - Users will be able to submit the 1010-CG application online
 - Caregivers will be able to better understand the program
 - 

#### Business Value
- Start processing applications faster
- Fewer rejections

## KPIs and OKRs

### KPIs
 - How many applications are submitted
 - How many applications are submitted online
 - How many applications are successful vs. unsuccessful
 - Qualitative metrics on the application process and overall experience
- Customer satisfaction (application process, caregiver program in general, etc.)
- Call Center reports

#### Baseline KPIs
tbd

### OKRs
tbd

--- 

## Go-to-market Strategy
- *How are Veterans and others using this product going to know it exists?*
- *What marketing, outreach, or communications are necessary for this product to be successful?*

## Target Launch Date
- *What is your target launch date of your MVP/iteration?*
- *What is your date for when you'll evaluate impact after launch?*

---

# Implementation Info

## Status
- As of January 2020, we're focused on launching the MVP of the form

## Solution Narrative

**Pre-May 31st**
- Unauthenticated form
- Two signatures (printed names onto online form)
- Form intro page
- Downloadable submission receipt
- Return ICN number for veteran and caregiver (if applicable)
- Obtain static list of approved Caregiver facilities from CARMA
- Create table in vets-api to link CARMA ID to form submission (+ date)

** **May 31st - Launch online, unauthenticated 1010CG application experience to CSCs** **

** **June 30th - Publish/market online, unauthenticated 1010CG application experience** **

**Post-June 30th**
- Ability to attach Power of Attorney documentation
- Attach prefilled 1010CG PDF to CARMA application
- Prevent identical applications sent back-to-back
- Allow Veteran/Caregiver to track application status
- To support Caregiver program in its expansion and reduce number of phone calls asking status question
- Options:
  - Use application ID number to query for status update
  - Work with MPI to return status there

**Future, Phase 2**: 
- Webpage MVP, Redesign of online PFCAC pages

**Future, Phase 3**: 
- Caregiver Portal - benefits after the application

**Future, TBD**:
- Facilities API as a source of truth

## How to Access and Test
- Link: tbd
- Password protection info: tbd
- User authentication info: tbd

## Error Handling

## Service Level Objective

## API Calls and Dependent Systems
 - CARMA backend integration
 - VA API

## Resources and Documentation

- Discovery and Research: https://github.com/department-of-veterans-affairs/va.gov-team/tree/master/products/caregivers
- Technical Documentation: 
- Product specs
- Design
- Roadmap: https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/teams/vsa/teams/caregiver/OKR_Roadmap_Caregivers.png
- ATO documentation

## Keywords


## Team

- VA.gov Lead: Chris Johnston 
- VA Policy Expert(s): TBD
- VA Digital Strategist(s) `*`: C.C. Gong
- Product Manager `*`: Alayna Abel
- Design Lead: Shawna Hein
- Eng Lead: Paul Short
- VA Web Comms Partner: 
- VA Call Center Partner(s): TBD
- Production Testing Partner(s): TBD
- Designer(s): Jonathan Nelson
- Content Writer(s): Patrick Sanders
- Front-end Engineer(s): Justin Linn
- Back-end Engineer(s): Kevin Mircovich

`*` = approval required for launch

### Screenshots
#### Before: 
https://www.va.gov/health-care/forms/vha-10-10CG.pdf, https://www.caregiver.va.gov/
#### After:
TBD
