# Account security: User views and completes tasks - LOA1
**Last updated:** August 18, 2023

- If users have not yet verfied their identity, they can still add 2-factor authentication to their account and find a link to their sign in service (eg. ID.me) to change or manage their sign in information. 

## UX

### Link to sign in service
- The user will see a section with information on how to change their sign in information for their sign in service of choice. 
- The link will bring the user to the website where they manage their account (either Login.gov,DS Logon, MyHealtheVet, or ID.me).
- This section will never have a checkmark, as this task can be completed often and does not directly determine account security. 
- [Desktop mock-up, change sign in information for sign in service](https://www.sketch.com/s/ebd4596f-0707-46cb-941e-247a808725cc/a/v8lVM24)
- [Mobile mock-up, change sign in information for sign in service](https://www.sketch.com/s/ebd4596f-0707-46cb-941e-247a808725cc/a/KvlZnZ2)


### 2-factor authentication
- The user will see the name of the section and prompt that tells them they can add 2-factor authentication.
- If they have not yet added 2-factor authentication, there will not be a checkmark next to the section. 
- Clicking the link will lead the user through the process of 2-factor authentication.
- This uses the [process list component](https://design.va.gov/components/process-list) from the VA design system. A numeral will appear if it hasn't been completed, and a checkmark will appear if it has been completed.
- [Desktop mock-up, 2-factor authentication](https://www.sketch.com/s/ebd4596f-0707-46cb-941e-247a808725cc/a/DPDQDwq)
- [Mobile mock-up, 2-factor authentication](https://www.sketch.com/s/ebd4596f-0707-46cb-941e-247a808725cc/a/KvlZnZ2)


## Codes
N/A

## How to reproduce
1. Log into staging with any LOA1 user. 
   - Note that the Identity team doesn't maintain LOA1 accounts, so you may need to create your own. 
   - You can do this by selecting "Create an account with ID.me" when you're at Staging's sign-in dialog. 
   - DO NOT verify your identity on the ID.me side.  
   - Once created, log into Staging with that acct's email and password.
2. Navigate to profile or update the URL in your browser to point to `/profile/direct-deposit` or any other section of profile aside from `/profile/account-security`
