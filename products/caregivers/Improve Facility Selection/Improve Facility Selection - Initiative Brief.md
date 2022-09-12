# Initiative Outline - Improve Facility Selection on the 10-10CG

#### [Epic for 10-10CG Improve Facility Selection](https://github.com/department-of-veterans-affairs/va.gov-team/issues/19433)
#### [Transition document for Facility Selection](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/caregivers/Transition%20hub/In%20progress%20features/Facility%20selection.md)

---

## Overview
* We want to increase the confidence with which Veterans select a facility on the 10-10CG, since it's key to getting their application routed appropriately.  

**Request from CG Team:**

>- Current
>     - Provide VA.gov a limited list of VAMCs for Veterans to select
>          - Filtered to where CSC is and does not allow a Veteran to fully answer the questions
>               - **Name of VA medical center or clinic where you receive, or plan to receive, health care services**
>               - **Name of facility where you last received medical treatment**
>     - Worked with Lighthouse team to add “CSC” present toggle in the API
>- PI 7
>     - Connect Lighthouse API to updated internal CARMA VAMC info
>- Needed from VA.gov
>     - Original plan was to have VA.gov connect to Lighthouse as well so they could switch away from the manual list
>     - Open up choices for the Veteran to choose from for those 2 questions
>          - CARMA or MuleSoft would then route the application to the correct VAMC queue in CARMA
>
>CARMA looking into connection with Lighthouse API for VAMC info (eg name, phone number, address, etc)
>- Would go to prod in ~August 2022
>- VA.gov Scope: look into changing VA.gov list of VAMC info for Veteran questions on 1010CG from manual CARMA list to the Lighthouse API

**Feedback from the Facilities team:**
>The facilitator locator uses the Lighthouse API to get data out of the legacy VAST facilities dB to populate search results. 

## Problems to solve

* Facility names change often
* Veterans may not know the name of the larger VA Medical Facility 
* Applicants may not know the name of a facilty with Caregiver services
* The layout of the page has been confusing in user research

 
## Desired User Outcomes
- Facility selection is easy and builds confidence
- Facility names are up-to-date
- 

## Undesired User Outcomes
- Increased difficulty completing the online form


## Desired Business Outcomes
- CSCs won't have to reroute applications because of incorrect facility selection

## Undesired Business Outcomes
- Increase in the number of applications that are misrouted 

---
## Measuring Success


### Key Performance Indicators (KPIs)

- User feedback (Medallia)
- Feedback from CSCs on misrouted applications


#### Baseline KPI Values
- Number of online Caregiver applications filled out per month:

### Objectives and Key results (OKRs)
_What are the measurable targets you're aiming for that delivers value for Veterans?_

- Objective: Make it easier for Veterans with representatives to fill out the online form
  - Key result: number of applications that are not misrouted or delayed **Where can we get this information??**
  - Key result: Facilities list is complete, accurate and up to date
       - [JSON static file](https://github.com/department-of-veterans-affairs/vets-json-schema/blob/8cdc5f35ad743af51170adad84b92a8b49504bdf/dist/caregiverProgramFacilities.json) contained 142 facilities
       - Facilities API contains **NUMBER** facilities
  - 
  


---

## Assumptions
- Veterans and Caregivers want to select the facility that is most convenient to them

## Solution Approach
- Provide an updated facility selection page that is easy to use and understand why we are asking for it
     - Connect with active Facilities API in place of the current static json file
     - Revisit UI against the current Facilities selection page on va.gov, and other private sector locator search pages
     - Conduct research/usability sessions with Veterans and Caregivers to determine the best, easy to use design
     - Redesign Facility selection page


### Initial goals
- Update the current search functionality with an updated API service for a more complete and accurate facilities list
- Update the current UI to be easier to use and understand

### Risks
- Applicants may not understand the reason for selecting a facility
- Applicants may not understand how to use the facility selector/search
- API dependencies may cause unplanned outages, causing our facility selector page to be unresponsive


--- 


## Launch Dates
- *Target Launch Date*
  - tbd
- *Actual Launch Date* 
  - tbd
- *What date will you evaluate impact after launch?*
