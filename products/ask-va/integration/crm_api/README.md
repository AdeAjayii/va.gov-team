## README.md

Overview of APIs goes here.


# API Integration Status

|Color | Status |
|---|---|
⬜ | Not Started |
🟨 | In Progress |
🟩 | Done |
🟥 | Blocked |

| Artifact | Endpoint | Source | API Status | Integration | Notes | Docs |
|---|---|---|:---:|:---:|---|:---:|
Status | GET /ping | Dynamics | 🟩 | 🟨 |  | [link](Status_Ping.md) |
Form | GET /topics?[id] | Dynamics | ⬜ | ⬜ |  | [link](form-get-topics.md) |
Form | PUT /inquiry/new | Dynamics | ⬜ | ⬜ |  | [link](Form_SubmitInquiry.md) |
Form | GET /alerts | Dynamics | ⬜ | ⬜ |  | [link](Form_RetrieveBannerMessage.md) |
Form | GET /inquiry?[id] | Dynamics | ⬜ | ⬜ | find by inquiry number? | [link](Form_RetrieveInquiryStatus.md) |
Dashboard | GET /search?[text] | Dynamics | ⬜ | ⬜ |  | link |
Dashboard | GET /correspondence | Dynamics | ⬜ | ⬜ | | [link](Dashboard_RetrieveCorrespondence.md) |
Dashboard | PUT /correspondence?[id] | Dynamics | ⬜ | ⬜ |  | [link](Dashboard_SubmitAReply.md) |
Dashboard | PUT /attachment?[id] | Dynamics | ⬜ | ⬜ |  | [link](Dashboard_UploadFile.md) |
Dashboard | PUT /profile/new | VA Profile | ⬜ | ⬜ | Offloading to VA Profile  | [link](Dashboard_CreateMyProfile.md) |
Dashboard | GET /profile | VA Profile | ⬜ | ⬜ | Offloading to VA Profile | [link](Dashboard_ReadMyProfile.md) |
Dashboard | POST /profile | VA Profile | ⬜ | ⬜ | Offloading to VA Profile | [link](Dashboard_UpdateMyProfile.md) |
Form | Medical Facilities | Lighthouse/Dynamics | ⬜ | ⬜ |  | [link](Form_MedicalFacilities.md) |
Form | School Facility Codes | WEAMS(?)/Dynamics | ⬜ | ⬜ |  | [link](Form_SchoolFacilityCodes.md) |
Form | GET /states | Dynamics | ⬜ | ⬜ |  | [link](Form_States.md) |
Form | GET /zipcodes?[prefix] | Dynamics | ⬜ | ⬜ |  | [link](Form_ZipCodes.md) |
Form | GET /provinces | Dynamics | ⬜ | ⬜ |  | [link](Form_CanadianProvinces.md) |
Dashboard | ~GET /inquiry~ | Dynamics | ⬜ | ⬜ |  | [link](Dashboard_RetrieveInquiries.md) |
Form | ~PUT /attachment?[id]~ | Dynamics | ⬜ | ⬜  |  | [link](Form_UploadFile.md) |
