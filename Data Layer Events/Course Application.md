# Course Application

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "course_application",
  "detailed_event": "Course Application",
    "event_data": {
        "course_application_step": "<course_application_step>",
        "name": "<name>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.course_application_step|string|Datasource for Application Step Name||||||||
|event_data.name|string|Captures the human-friendly name of the form.|Payment Info, Mailing Address, Payment Address, Contact Us|||||||

## Attached Notes

<p><strong>Platform: myhbx</strong></p>
<p>This event fires when the user starts the 'personal information' application flow step. This event should only be fire once per page request. (step2)</p>
