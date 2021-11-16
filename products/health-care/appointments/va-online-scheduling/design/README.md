# VAOS Design

VA Online scheduling is built on the [VA.gov design system](https://design.va.gov/).

Templates for the appointments list and scheduling flows can be found in the VA.gov Design Sketch workspace.
* [Templates and styles doc](https://www.sketch.com/s/ccd66412-dd7c-41ba-9528-88892a33af63)
  * [Appointments list](https://www.sketch.com/s/ccd66412-dd7c-41ba-9528-88892a33af63/p/50DC3685-35CE-4EE4-924C-73B1E444D4C5)
  * [Appointment detail pages](https://www.sketch.com/s/ccd66412-dd7c-41ba-9528-88892a33af63/p/650F35EF-9085-46F2-AAD2-BC8FEAB3DEA1)
  * [Scheduling pages](https://www.sketch.com/s/ccd66412-dd7c-41ba-9528-88892a33af63/p/F5D9EABE-09D2-43FE-8894-9B643E298347)

VAOS is [one of many touchpoints](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/health-care/appointments/va-online-scheduling/design/scheduling-channels-touchpoints.md) Veterans can use to schedule health care appointments.

We measure the success of designs by following the [VAOS OKRs & KPIs](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/health-care/appointments/va-online-scheduling/analytics/vaos-kpis.md).

We track design work on the [VAOS Product/Design Board](https://app.zenhub.com/workspaces/vaos---productdesign-5fff340c2d80a4000fb6f69c/board?labels=vaos-product-design&repos=33202667,62409417,133843125,66304117)

## VA appointments list

Current state documentation of the appointments list:
* [Add to calendar details](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/health-care/appointments/va-online-scheduling/design/add-to-calendar.md)
* The home page appointment and confirmation pages have been updated (see staging.va.gov) - older version for reference:
* [Confirmation cards](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/health-care/appointments/va-online-scheduling/design/confirmation-cards.md)
* [Appointment cards](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/health-care/appointments/va-online-scheduling/design/appointment-cards.md)


## Scheduling flows

* [Alerts and notifications](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/health-care/appointments/va-online-scheduling/design/alerts-audit.md)
* [COVID-19 vaccine flow](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/health-care/appointments/va-online-scheduling/design/cheetah_flow.md)
* [Community care flow](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/health-care/appointments/va-online-scheduling/design/community_care_flow.md)
* [Direct schedule flow](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/health-care/appointments/va-online-scheduling/design/direct-schedule-flow.md)
* [Appt request flow](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/health-care/appointments/va-online-scheduling/design/request_flow.md)

## User flows


![Flows](images/VAOS-User-Flows.png)


<details>
<summary>Previous flow diagrams</summary>
  
- [Updated VAOS Flow - Flowmapp](https://app.flowmapp.com/share/0fdcf2559a4c55625591f89c2e5d7649/userflow/83089/)
- [VAOS Flow - Figma](https://www.figma.com/file/KGChcQHMrTReo7T7cML418/VAOS-Flow)

</details>


## Background

At the end of 2019, the VAOSR initiative, a re-design project, launched with UAT testing with Veterans on the new application flow. By May 2020, VAOSR was at 100% availability on VA.gov. Around the same time, due to Covid-19, all facilities turned off direct scheduling (the ability to choose a date and time in VAOS).

In October 2020, the team collaborated with the Facility Locator team to research community care scheduling. The goal was to improve the provider selection as there was a steep drop-off rate on the community care provider selection page. Veterans had to navigate to Facility Locator to find their preferred provider and then copy/paste their information into VAOS. The team tested a prototype for selecting providers directly in VAOS and the Facility Locator uncovered insights about how schedules and Veterans search for providers. 

By December 2020, the team started work on improvements to the appointment list on the VAOS homepage. Veterans were having difficulty navigating the list and finding appointments, as well as distinguishing between video, phone, and in-person appointments.

Because other teams also display appointments, the VAOS team kicked off a cross-team effort to help other teams display appointments across different channels and tools where a Veteran might need to see them and followed up with usability testing.

Additional dev work on the homepage was put on hold as the team pivoted to COVID-19 vaccine scheduling in VAOS. This functionality is currently in pilot with limited facilities as of April 2021.


