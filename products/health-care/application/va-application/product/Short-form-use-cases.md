# Product Use Cases Template

_Track and maintain the various use cases that exist for a given product and is best maintained alongside the product outline._

_The purpose of this document is for designers, PMs, and engineers to align early on on potential use cases and edge cases so these things aren't coming up randomly and late in the process. We recommend the team schedule a 30 minute meeting to brainstorm all use cases/edge cases early on.  Examples of cases that could be captured here include: "Veteran logs in but is not LOA3ed.", "Veteran searches and gets no results." etc etc_

Link to product outline: [Product outline](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/teams/vsa/teams/health-benefits/healthcare-application/product-outline.md)

## Contents
<details>
<summary></summary>
  
- Authenticated-immediate alert ([chart](https://www.sketch.com/s/da85cf44-4503-4e98-834e-ff068b242ef6/a/EL9RYvq))
- Authenticated-self-report ([chart](https://www.sketch.com/s/da85cf44-4503-4e98-834e-ff068b242ef6/a/jgDjqJb))
- Unauthenticated-self-report ([chart](https://www.sketch.com/s/da85cf44-4503-4e98-834e-ff068b242ef6/a/dlvDq7j))
- Full application flow/ less than 50% disability rating ([chart](https://www.sketch.com/s/da85cf44-4503-4e98-834e-ff068b242ef6/a/zxZzO2l))
  
  
</details>

## Use Case A

* **Description** Authenticated / Disability 50% +
  - Veteran is logged-in (authenticated) and has a disability rating of 50% or higher.
    - General flow: customer sees standard bio info (name, ssn, dob)
    - Next is presented with a new "Short form alert" page
    - From here he enters Veteran info as shown in the flow diagram (required fields that are not pre-populated)
    - And lastly, goes to Insurance screen
    - And then Review and Submit.
  

* **Link to designs**
  - ([chart](https://www.sketch.com/s/da85cf44-4503-4e98-834e-ff068b242ef6/a/EL9RYvq))

* **Instructions to access in Staging (or Prod for Drupal)** (_Note: credentials should be stored in sensitive repos only_)
  - lorem ipsum

## Use Case B 

* **Description** Authenticted / Self Reports Disability rating of 50% +
  - Veteran is logged-in (authenticated) and we don't have a disability rating of 50% or higher.
    - General flow: Customer progresses through standard authenticated flow and enterans Veteran Info
    - Upon reaching the "Current Compensation from VA" screen, they select the radio button option for a disability rating of 50% o higher
    - Sees a confirmation screen asking to confirm their rating is 50% or higher
    - From there, goes into the short-form flow as per Use Case A.


* **Link to designs**
  - ([chart](https://www.sketch.com/s/da85cf44-4503-4e98-834e-ff068b242ef6/a/jgDjqJb))

* **Instructions to access in Staging (or Prod for Drupal)** (_Note: credentials should be stored in sensitive repos only_)
  - lorem ipsum

## Use Case C

* **Description** Unauthenticated / Self Reports Disability rating of 50% +
  - lorem ipsum

* **Link to designs**
  - ([chart](https://www.sketch.com/s/da85cf44-4503-4e98-834e-ff068b242ef6/a/dlvDq7j))

* **Instructions to access in Staging (or Prod for Drupal)** (_Note: credentials should be stored in sensitive repos only_)
  - lorem ipsum

## Use Case D

* **Description** Full application flow / less than 50% disability rating
  - Veteran is either auth or unauth
  - Less than 50% disabilty rating
  - Existing flow
  

* **Link to designs**
  - ([chart](https://www.sketch.com/s/da85cf44-4503-4e98-834e-ff068b242ef6/a/zxZzO2l))

* **Instructions to access in Staging (or Prod for Drupal)** (_Note: credentials should be stored in sensitive repos only_)
  - lorem ipsum

