# Retrieve Replies

## Request

**Method**: GET

**Path**:  /inquiry/{id}/replies

**Parameters**:
| Name | Type | Description |
|---|---|---|
|id|string|Inquiry Number to Retrieve Correspondence For|

**Headers**:
| Name | Type | Description |
|---|---|---|
|Authorization|JWT?|Token for access to the CRM API|
|ICN|string|User ICN|

## Response

<table>
<tr>
<td> Status </td> <td> Response </td>
</tr>
<tr>
<td> 200 </td>
<td>

```json
{ 
    "status": { 
        "code": 200, 
        "message": "OK", 
        "data": [
            {
                "id": "a6c3af1b-ec8c-ee11-8178-001dd804e106",
                "modifiedon": "1/2/23",
                "status_reason": "Completed/Sent",
                "description": "description",
                "message_type": "Valid values should be 722310000: Reply to VA and 722310001: Response from VA",
                "enable_reply": true,
                "attachmentNames": [
                    {
                        "id": "012345", 
                        "name": "File A.pdf"
                    }
                ]
            }
        ] 
    }
}
```

</td>
</tr>
<tr>
<td> 403 </td>
<td>

```json
{
    "status": {
        "code": 403,
        "message": "Unauthorized."
    }
}
```

</td>
</tr>
<tr>
<td> 404 </td>
<td>

```json
{
    "status": {
        "code": 404,
        "message": "Inquiry not found."
    }
}
```

</td>
</tr>
</table>

## Notes

* ~CC: No pagination, all valid correspondence will be returned.~
* CC: CRM will plan to mimic the current filtering on the portal view to only include Response and Reply messages. (Message Type = 722310000: Reply to VA and 722310001: Response from VA )
* ~CC: Handling of attachments:  Do not need the actual file until the submitter elects to open it. Need to define attachment identifiers (name, ID) to be used for UX display and for file request API.~
* ~CC: Reply button: Where will you get the logic for turning the button on/off?~
  * JH: "enable_reply": true, ??
