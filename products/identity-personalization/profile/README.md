# Product Outline: VA.gov Profile

Last Updated April 5, 2021

### Communications
- GitHub Label: Profile
- Slack channel: [#vsa-authd-exp](https://dsva.slack.com/channels/vsa-authd-exp); [#va-profile](https://dsva.slack.com/channels/va-profile)
- Keywords
     - Profile
     - Profile 2.0
     - Contact information
     - Direct deposit
     - VA Profile (formerly Vet360)

### Roles  
  
|Name|Role|Email|
|----|----|-----|
|Samara Strauss |DSVA Lead| samara.strauss@va.gov |
|Anastasia Jakabcin (AJ) |Product Manager| ana@adhocteam.us |
|Tressa Furner |Designer| tressa.furner@adhocteam.us |
|Liz Lantz |Designer| liz.lantz@adhocteam.us |
|Erik Hansen | FE Engineer| erik@adhocteam.us |
|Sandra Hallie | FE Engineer| shallie@governmentcio.com |
|Lihan Li | BE Engineer | lihan@adhocteam.us |

---

### Table of Contents

- [Overview](#overview)
- [Products/Projects](#productsprojects)
- [Solution Narrative](#solution-narrative)
- [How to Access and Test](#how-to-access-and-test)
- [Error Handling](#error-handling)
- [Backend Systems that Support the Profile](#backend-systems-that-support-the-profile)
- [Design](#design)
- [Screenshots](#screenshots)

---

## Overview

The [VA.gov profile](https://staging.va.gov/profile) provides a centralized place where users can see what information the VA knows about them, and where they can update that information as needed.

Currently, the VA.gov profile supports the following information:

- Personal and contact information
- Military information
- Direct deposit information
- Account security
- Connected apps (managed by the Lighthouse team)

### Is VA Profile the same thing as the VA.gov profile?

**No, VA Profile and the VA.gov profile are not the same thing and do not have a 1:1 relationship.**

- **VA Profile**: This is a backend system that was formerly known as Vet360. It came about in 2018 to act as a connector between a bunch of VA backends and frontends, so that veterans could update their info in one place and it would save everywhere (or almost everywhere). The VA Profile team is not part of the OCTO/DEPO contracts. They are an entirely separate team that we work with, and they work with a lot of other teams. 
- **The VA.gov profile** — The VA.gov profile is a section of VA.gov, which you can view at https://staging.va.gov/profile/personal-information with pretty much any staging user. The VA.gov profile is a **frontend only**; we do not store any information. We rely entirely on [various VA backend systems](#api-calls-and-dependent-systems) to show and save data. VA Profile is only one of them, which we currently use to show and save contact information. 

## Solution Narrative

### Current projects

- We are currently working on efforts to add preferred facility information and notification preferences to the profile

|Product/Project| Outline|
|----|----|
|Direct deposit for edu| [Direct deposit for edu outline](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/identity-personalization/direct-deposit/edu-direct-deposit/README.md)|
|Preferred medical facility| [Preferred facility outline](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/identity-personalization/profile/preferred-facility/README.md) |
| Commmunications permissions/notifications preferences | [Notification preferences outline](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/identity-personalization/notifications/notification-preferences/README.md) |

### Past projects

|Product/Project| Outline|
|----|----|
|Combine profile and account (Profile 2.0)| [Profile 2.0 outline](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/identity-personalization/profile/Combine%20Profile%20and%20Account/README.md)|
|Connected apps | [Connected apps outline](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/identity-personalization/profile/connected-apps-data/README.md)
|Address validation| [Address validation outline](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/identity-personalization/profile/contact-information/address-validation/README.md)|
|Direct deposit for comp & pen | [Direct deposit for comp & pen outline](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/identity-personalization/direct-deposit/README.md)|
|Contact information| [Contact information outline](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/identity-personalization/profile/contact-information/README.md)|
|2018 MVP| [2018 MVP outline](https://github.com/department-of-veterans-affairs/vets.gov-team/blob/master/Products/Identity/Personalization/Profile/Readme.md)|

### Timeline

- 2016/17 — Prototypical "account" page on Vets.gov.
- Spring 2018 - Original EMIS profile launched to Vets.gov.
- Summer 2018 — Profile backend transitioned to VA Profile (then- Vet360).
- 2019 — Direct deposit for comp & pen added to the profile.
- 2019/2020 – Address validation added to the Mailing and Home address fields.
- 2020 - Profile 2.0 redesign (launched Fall 2020).
- 2021 — Direct deposit for edu added to the profile (pending). Preferred facility and notification preferences in progress.

## How to Access and Test

- Login with [any staging user](https://github.com/department-of-veterans-affairs/va.gov-team-sensitive/blob/master/Administrative/vagov-users/mvi-staging-users.csv) on https://staging.va.gov
- Visit https://staging.va.gov/profile/

## Error Handling

- [List of VA Profile (Vet360) error codes](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/identity-personalization/profile/contact-information/Profile%20Error%20Codes.md)

## Backend Systems that Support the Profile

- Contact information comes from VA Profile.
- Direct deposit for comp & pen information comes from EVSS.
- Direct deposit for edu information comes from BGS.
- Personal information comes from MPI.
- Military information comes from eMIS.

## Design 

- [2018 designs](https://github.com/department-of-veterans-affairs/va.gov-team/tree/master/products/identity-personalization/profile/profile-V1/design)
- [2020 Profile 2.0 designs](https://github.com/department-of-veterans-affairs/va.gov-team/tree/master/products/identity-personalization/profile/Combine%20Profile%20and%20Account/Design)

## Screenshots

This is the latest version of the profile:
