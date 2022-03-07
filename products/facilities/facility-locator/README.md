# Facility Locator

## Index of relevant links and resources 

[**VSA Facilities Team transition document | March 2022**](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/teams/vsa/teams/facility-locator/product-transition-doc.md)

[**Issue response (including architecture diagrams)**](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/facilities/facility-locator/issue-response.md)

[**Error states**](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/facilities/facility-locator/error_states.md)

[**Facility Locator Subject Matter**](https://github.com/department-of-veterans-affairs/va.gov-team/tree/master/products/facilities/facility-locator/va-facility-subject-matter)
- This page is an index of links and resources related to the Facility Locator ecosystem. 

## Practice Specific

[**Engineering Index**](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/facilities/facility-locator/engineering/README.md)
- This page is an index of links and resources related to the Engineering practice, including Working with Engineering and processes for pull requests, triage and QA.   

[**Design Index**](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/facilities/facility-locator/Design/README.md)
- This page is an index of links and resources related to the Design practice, including Inclusivity and 508 Compliance.  

[**Product Index**](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/facilities/facility-locator/product/README.md)
- This page is an index of links and resources related to the Product practice. 

## Across VSP

[**Guidelines for documentation in GitHub**](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/platform/working-with-vsp/orientation/repo-guidelines.md)
- This page will help you determine where files should go and how to name them.

[**Documentation Best Practices**](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/platform/information-architecture/working-with-documentation.md)
- This page will help all teams working in the VA.gov GitHub ecosystem understand when to engage Documentation resources for support. 

[**Content Rules of Engagement**](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/platform/content/content-review-process.md)
- This page will help all teams working on VA.gov understand when to engage Content resources for review and support. 


## What to know about the product 
- va.gov/find-locations
- It is VA's single source of truth for Veterans and beneficiaries to find VA facilities and location details about all VA facilities, across VHA, VBA, and NCA
- It is the newer version of VA's old facility locator: <https://www.va.gov/directory/guide/home.asp>
- It is powered by the non-public-facing Vets API
- It uses Mapbox for maps functionality: <https://docs.mapbox.com/mapbox-gl-js/api/> (which was changed to an annual license version, effective Oct 1, 2019, facilitated by Nancy Smith of Oddball)
- It serves many purposes, from finding basic facility address and phone information to preparing for a visit, to understanding eligiblity for community care

## Other notes

- Facility Locator 1.0 work can be found in this old repo: <https://github.com/department-of-veterans-affairs/va.gov-team/tree/master/products/facilities/facility-locator>

-----
## Legacy info about the Facility Locator

<details>
  <summary> Product and system stakeholders </summary>
- VA Product owner: David Conlon 
- VA.gov Lead: Chris Johnston 
- Facility API Product Owner: Dave Mazik 
- VSSC Analyst/Engineer: Chad Holmes 
- Michael Villeneuve: He runs GEOBISL, and wrote custom queries that pass data from CDW to vets-api.
- Information Architecture: Mikki Northius, @Mikki on Slack
</details>
  
<details>
  <summary> VHA business stakeholders </summary>

All of these folks help drive the vision and implementation of VA Community Care benefits.

- Dr. Kamron Matthews: Works directly with community health care networks and regions for Veterans to receive community care benefits.
  - Zach Fain: Does a lot of implemntation work for networks
  - Tobie Wethington: Project Manager for community provider data from PPMS (used in Facility locator for Community Care Urgent Care, Community Care Provider Locator)
- Dr. Jen McDonald: Was involved with Mission Act implementation
- Dr. Leo Greenstone: Business sponsor to have AbleVets team build their community care provider lookup on Facility Locator
- Dr. Mark Upton: Has an interest in community care urgent care facilities
- All about the 2019-2020 roadmap to make the next version of the product even better for users.
</details>

<details>
  <summary> Product goals </summary>
- Switch primary data source from Vets API to Facility API: <https://developer.va.gov/explore/facilities/docs/facilities>
- Reach parity with all legacy VA facility locator tools, so they can be depracated
  - Main legacy facility locator: https://www.va.gov/directory/guide/home.asp
  - Will need to  meet users' needs, but also convince the business to turn off old tools
- Integrate urgent care facility and urgent care pharmacy facilities into the product
  - Here is VA's current product: <https://vaurgentcarelocator.triwest.com/>
- Incorporate Mission Act-required facility drive time functionality
- Update the product's information architecture to organize facilities based on users' mental models (e.g., mental health care vs. Vet Center)
- Update the product's UI and interaction design so users can get to facility results in just a few clicks/taps
- Update facility detail page to match new VAMC facility page design
  - Here is a health facility detail page design: <https://www.va.gov/pittsburgh-health-care/locations/pittsburgh-va-medical-center-university-drive/>
- Surface basic Veteran-benefit eligibility information for each facility type (e.g., health care facility, community care provider, etc.)
- Use the VHA health service taxonomy for health facilities
- Create/update new VBA service taxonomy and NCA service taxonomy, with new structured content designed, and powered by Drupal
- Make it faster
- Fix bugs
  </details>

  <details>
  <summary> Design problems </summary> 

    - Users don't have a way to get to urgent care facilities
  - See the following research study documentation:
    1. Main research repo: <https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/health-care/community-care/urgent-care/research>
    2. Research readout: <https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/health-care/community-care/urgent-care/research/jun-2019/findings.md>
    3. User flows Mural board: <https://app.mural.co/t/adhocvetsgov9623/m/adhocvetsgov9623/1560946920965/4bb321f266f232e3e1d91559b168a0f3c11fe84f>
- Search UI is inconsistent (i.e., free text search box, dropdowns, typeahead)
- Community care "facilities" are actually providers, so users are searching for persons, not places
- Facility API data often does not load or show up on facility detail pages
- Web browser's location/geo-location functionality doesn't always work (or work well) on facility search page

## What to research
- Pain points and bright spots with the current product (i.e., evaluative usability testing)
- Users' mental models for VA facilities and services, including community care
  - Specifically, how users think about in-network emergency care, urgency care, and urgent care pharmacy facilities
- How to integrate services and facilities into the UX (i.e., search by condition or service needed vs. facility type)
- How/if we should integrate content editing/publishing of some facility detail page content using the Drupal CMS
  - Images! Should we use Drupal to manage facility images for each facility detail page?
- Creating facility detail page URLs and content that are SEO (i.e., /wilmington-vet-center vs. /vba456)
- How to include drive-time functionality into UX
- How to make the product work faster for users
- How to better architect how we call data from the community care database
- All the data sources! How can we better streamline our data sources, and structured product content on the UI, so users get a consistent product experience
    
    </details>
