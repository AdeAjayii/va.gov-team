# Release Plan (WIP)

## When to use this release plan

If you answer yes to any of the questions below, you'll need to create a release plan using this template.

Does the feature you are working on moderately or significantly affect the Veteran experience of the product?
- _YES_

Does the feature you are working on change the structure of the underlying data?
- _YES - links and promo content on the existing/current homepage is hard coded on the front end but will draw from Drupal as the source of truth in the redesigned experience_

Does the feature's backend or downstream interactions change? 
- _YES - The frontend will call Drupal for the information_

Is this a brand new experience for a Veteran?
- _NO_

## Step 1: Development

| Feature Toggle name | Description | Issue
| ----------- | ----------- | ----------- |
| [_TBD_] | Controls opt-in modal display on live homepage | [#11653](https://app.zenhub.com/workspaces/vagov-cms-team-5c0e7b864b5806bc2bfc2087/issues/department-of-veterans-affairs/va.gov-cms/11653)
|[_feature_homepage_v2: FEATURE_HOMEPAGE_V2_] | CMS feature flag/config setting controls the new homepage design deployment to Prod | [#10965](https://github.com/department-of-veterans-affairs/va.gov-cms/issues/10965)

## Step 2: Validation

Since we use a [continuous delivery](https://depo-platform-documentation.scrollhelp.site/developer-docs/deployment-process) model, once code is in the `main` branch, it will be deployed that day. 

Before enabling your feature toggle in production, you'll need to:

- [ ] Follow [best practices for QA](https://depo-platform-documentation.scrollhelp.site/developer-docs/qa-and-accessibility-testing).
- [ ] Have your team perform as much validation in staging as possible. Validation may be challenging for some teams and systems due to downstream requirements, but the staging system should mimic the production system as much as possible.
- [ ] Work any downstream or dependant systems proactively to ensure that the feature is ready for use once it hits production.
- [ ] Have a go/no go meeting with the team to ensure that the feature is ready for use and signed off by each discipline and your DEPO/OCTO contact. During this meeting, you'll need to:
  - [ ] review the plan with your DEPO/OCTO representative.
  - [ ] review the release plan with your team.

### Define the Rollback process

> The opt-in modal will be governed by a [feature toggle - #11653](https://github.com/department-of-veterans-affairs/va.gov-cms/issues/11653). We will monitor the deployment for unexpected behavior. By turning off the modal, we can prevent Veterans and beneficiaries from being directed to the redesigned experience.  

> [VA-CMS Incident Response Procedure Overview](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/platform/cms/helpdesk/incident-response.md)

### Phase I: Moderated production testing during Soft launch period

Rather than a staged roll-out, the redesign will be "soft launched" in Production as a parallel page which Veterans and beneficiaries can visit via "opt in" from the existing VA.gov homepage. A similar method was used during the original launch of VA.gov but was managed using a preview subdomain which is not an option for this launch. Two options were evaluated during a design, accessibility and implementation discussion. The modal was chosen as the preferred approach over a banner. 

More information about this soft launch is available in the [Launch planning section of the initiative brief](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/public-websites/home-page/home-page-redesign-initiative/initiative-brief.md#soft-launch). 

#### Planning

- Desired date range or test duration: _Beginning mid-December 2022_ 
- Desired number of users: [_TBD_]
- How you'll recruit the right production test users: _via Opt-in_
- How you'll conduct the testing: _by monitoring analytics and feedback scores_
- How you'll give the test users access to the product in production w/o making it live on VA.gov: _opt-in modal displayed on existing/current homepage_ 
- What metrics-based criteria will you look at before advancing rollout to the next stage ("success criteria")?:[Cutover criteria](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/public-websites/home-page/home-page-redesign-initiative/cutover-determination-for-full-launch.md) 
- Links to the dashboard(s) showing "success criteria" metrics: [_TBD_] with link to dashboards (example: Google Analytics dashboard)
- Who is monitoring the dashboard(s)?: _Michelle Middaugh_

#### Results

- Number of unique users: [FILL_IN]
- Metrics at this stage (per your "success criteria"):[Cutover criteria](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/public-websites/home-page/home-page-redesign-initiative/cutover-determination-for-full-launch.md) 

|	Metric	| Baseline (Completion rate on existing homepage) - July 1 - October 31, 2022 (Number / % of users)	|	Target  | Soft launch measurement   |
|	---	|	---	|	---	|	--- 
| Veteran/beneficiary views | | ||
|	Use of authenticated experience	|	3,701,932 / 41.44%	|	50% | |
|	"Message your doctor or get a health care message" task completion | 587,173 / 6.57% 	|	 | |
|	"Download your benefit letters" task completion |	508,591 / 5.71%	|	 | |
|"Apply for education benefits" task completion  | 198,762 / 2.22%		|	 | |
|	User engagement - promo content #1  |	6 / <0.01%	|Increased | |		
|	User engagement - promo content #2 | 	0 / 0%		|Increased	 | |	
|	User engagement - promo content #3 | 	6 / <0.01% | Increased | | 
| Satisfaction score | | new homepage satisfaction scores are equivalent or better than existing page		|	 | |
 

## Post Launch metrics

Continue to check in on the KPIs of your feature at periodic intervals to ensure everything is working as expected. We recommend one-week and one-month check-ins, but this is only minimal.

### 1-week results

|	Metric	| Baseline (Completion rate on existing homepage) - July 1 - October 31, 2022 (Number / % of users)	|	Target  | 1 week  |
|	---	|	---	|	---	|	--- 
| Veteran/beneficiary views | | ||
|	Use of authenticated experience	|	3,701,932 / 41.44%	|	50% | |
|	"Message your doctor or get a health care message" task completion | 587,173 / 6.57% 	|	 | |
|	"Download your benefit letters" task completion |	508,591 / 5.71%	|	 | |
|"Apply for education benefits" task completion  | 198,762 / 2.22%		|	 | |
|	User engagement - promo content #1  |	6 / <0.01%	|Increased | |		
|	User engagement - promo content #2 | 	0 / 0%		|Increased	 | |	
|	User engagement - promo content #3 | 	6 / <0.01% | Increased | | 
| Satisfaction score | | new homepage satisfaction scores are equivalent or better than existing page		|	 | |

- Any issues with VA handling/processing?:  [PICK_ONE]: yes | no |  N/A
- Types of errors logged: [FILL_IN]
- Any changes necessary based on the logs, feedback on user challenges, or VA challenges? [PICK_ONE]: yes | no |  N/A
- If yes, what: [FILL_IN]

### 1-month results

|	Metric	| Baseline (Completion rate on existing homepage) - July 1 - October 31, 2022 (Number / % of users)	|	Target  | 1 month  |
|	---	|	---	|	---	|	--- 
| Veteran/beneficiary views | | ||
|	Use of authenticated experience	|	3,701,932 / 41.44%	|	50% | |
|	"Message your doctor or get a health care message" task completion | 587,173 / 6.57% 	|	 | |
|	"Download your benefit letters" task completion |	508,591 / 5.71%	|	 | |
|"Apply for education benefits" task completion  | 198,762 / 2.22%		|	 | |
|	User engagement - promo content #1  |	6 / <0.01%	|Increased | |		
|	User engagement - promo content #2 | 	0 / 0%		|Increased	 | |	
|	User engagement - promo content #3 | 	6 / <0.01% | Increased | | 
| Satisfaction score | | new homepage satisfaction scores are equivalent or better than existing page		|	 | |

- Any issues with VA handling/processing?: [PICK_ONE]: yes | no |  N/A
- Types of errors logged: [FILL_IN]
- Any UX changes necessary based on the logs, feedback on user challenges, or VA challenges? [PICK_ONE]: yes | no |  N/A
- If yes, what: [FILL_IN]

## Post-launch Questions

*To be completed once you have gathered your initial set of data, as outlined above.*

1. How do the KPIs you gathered compare to your pre-launch definition(s) of "success"?
1. What qualitative feedback have you gathered from users or other stakeholders?
1. Which assumptions you listed in your product outline were/were not validated?
1. How might your product evolve now or in the future based on these results?
1. What technical tasks are needed to clean up (i.e., removal of feature toggles)?
