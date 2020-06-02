# Caution Flag Release Plan

So! You're thinking about how you want to launch your product. You know you'll perform usability testing and you'll QA the heck out of it in staging, which are both very critical components of product development. But they don't tell you how people will naturally use your product when you're not there to guide them to it, how any submitted data will get to VA, whether that data will be easy or difficult for VA to process, whether people will be likely to submit duplicates, abandon partway through, or encounter bugs unique to the production environment. All of which could be very detrimental to users, which is the antithesis of what we're here to do. 

So: **how might we craft a release plan to test our product "in the wild" at a smaller scale, and learn how it'll actually be used, and what problems it actually might have or create, and then fix/adjust prior to going live to millions of VA.gov users?**

That's what this Release Plan Template is for! And note - there are feature toggles and beta banners at your disposal that you can use as a part of your plan.

---

## Phase I: moderated production testing (also known as User Acceptance Testing, or UAT)

### Planning:
- Desired date range or test duration: 04/13/2020 - 04/16/2020
- Desired number of users: 2
- How you'll recruit the right production test users: NA - our UAT is completed on Staging with VA Education Services counterparts
- How you'll conduct the testing: UAT is completed on Staging with VA Education Services counterparts
- How you'll give the test users access to the product in production w/o making it live on VA.gov: Education Services has access to staging

### Results:
- Number of users: x
- Number of bugs identified / fixed: x/x
- Was the data submitted (if any) easy for VA to process?: yes/no, lorem ipsum
- Types of errors logged: lorem ipsum
- Any UX changes necessary based on the logs, or feedback on user challenges, or VA challenges? yes/no 
- If yes, what: lorem ipsum

## Phase II: unmoderated production testing: NA

### Planning:
- Desired date range: mm/dd/yy - mm/dd/yy
- Desired number of unique users: x
- How you'll make the product available in production while limiting the # of users who can find/access it: lorem ipsum
- "Success" criteria (by the numbers): [use your KPIs to help guide this. It could be things like abondomnent rate < 20%, reported contact center calls < 2 calls, error rate < 5%, etc.]

### Results:
- Number of unique users: x
- Actual results (per your "success criteria")
- Was the data submitted (if any) easy for VA to process?: yes/no, lorem ipsum
- Types of errors logged: lorem ipsum
- Any UX changes necessary based on the logs, or feedback on user challenges, or VA challenges? yes/no 
- If yes, what: lorem ipsum

More phases? Sure! If it makes sense for your product! Plan them out with the same structure as above.

## Go Live!

### Planning:
- Desired date: 04/22/2020
- Post-launch KPI 1: xx lorem ipsum
- Post-launch KPI 2: xx lorem ipsum
- Post-launch KPI 3: xx lorem ipsum
- Go / No Go: (ready / not ready)[https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/platform/product-management/go-no-go-meeting-template.md] Planning to hold this meeting with Education Services + DEPO representative + OIT on 04/20/2020

### 1-week results:
- Number of unique users: x
- Post-launch KPI 1 actual: xx lorem ipsum
- Post-launch KPI 2 actual: xx lorem ipsum
- Post-launch KPI 3 actual: xx lorem ipsum
- Any issues with VA handling/processing?: yes/no, lorem ipsum
- Types of errors logged: lorem ipsum
- Any UX changes necessary based on the logs, or feedback on user challenges, or VA challenges? yes/no 
- If yes, what: lorem ipsum

### 1-month results:
- Number of unique users: x
- Post-launch KPI 1 actual: xx lorem ipsum
- Post-launch KPI 2 actual: xx lorem ipsum
- Post-launch KPI 3 actual: xx lorem ipsum
- Any issues with VA handling/processing?: yes/no, lorem ipsum
- Types of errors logged: lorem ipsum
- Any UX changes necessary based on the logs, or feedback on user challenges, or VA challenges? yes/no 
- If yes, what: lorem ipsum

## Post-launch Questions 

_To be completed once you have gathered your initial set of data, as outlined above._ 

1. How do the KPIs you gathered compare to your pre-launch definition(s) of "success"?
   a. Applications to institutions and schools with caution flags decreases
      i. Applications and payments of GI Bill benefits to institutions with caution flags decreses.
      ii. Fewer people looking at profile pages with the most caution flags
         i. Would probably want to look at this at the same time of year due to cyclical process of 
         ii. Need more information from UXers via GA 
      iii. On the profile page, we are able to track click on "view more details" to view more information (we don't have a baseline for the before) 
         i. Need more information from UXers via GA 
         ii. We want fewer people
      iv. Click the link in the caution flag to external link to learn even more (we don't have a baseline for the before) 
         i. Need more information from UXers via GA 
1. What qualitative feedback have you gathered from users or other stakeholders, if any?
   a. Qualitative input from Usability Testing
   b. Des to double check to see if UAT feedback was qualitative
1. Which of the assumptions you listed in your product outline were/were not validated?
   a. We didn't have a product outline due to when we jumped into the VSP process
1. How might your product evolve now or in the future based on these results?
   a. Make it easier for EDU to make updates to Caution Flag content so that they can continue to provide more specific warnings and notifications to the users. 
