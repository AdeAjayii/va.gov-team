# Community Care request submission

Status: In progress

## Services
### Current services used
- /v4/rest/appointment-service/patient/ICN/{icn}/community-care-appointment
- /v4/rest/appointment-service/patient/ICN/{icn}/appointment-requests/system/var/id/{request_id}/messages
- /v4/rest/patient/ICN/{icn}/preference

### Equivalent FHIR resource

- http://hl7.org/fhir/dstu2/appointment.html

## Data
### Data to FHIR model mapping
- Type of care (Appointment.type)
- Visit Type (**Unknown**)
- Status (Appointment.status)
  - Looks like we have to send "proposed"
- Method (**Unknown**)
   - Community Care or not
- Location (Appointment.participant[Location])
- Appointment date and time (Appointment.slot)
- User provided detail (**Appointment.comment?**)
- Preferred language (**Unknown**)
- Closest facility (**Appointment.participant[Organization]**)
- User contact details (**Unknown**)
### Missing/incomplete data list
- Preferred language
- Closest facility?
- Visit type
- Method
### Differences in scope of data returned
- N/A
## Outstanding questions

- Will we still need to include the VA organization?
- We currently allow you to omit the provider and also for users to enter the details on their own. Is that supported?
