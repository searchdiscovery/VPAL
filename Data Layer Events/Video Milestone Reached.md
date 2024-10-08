# Video Milestone Reached

CRP status: N/A for CRP flow

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "video_progress",
  "detailed_event": "Video Milestone Reached",
    "event_data": {
        "identifier": "<identifier>",
        "type": "<type>",
        "video_duration": <video_duration>,
        "video_milestones_reached": <video_milestones_reached>,
        "video_percent": "<video_percent>",
        "video_provider": "<video_provider>",
        "video_title": "<video_title>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.identifier|string|Captures the ID of video content viewed by visitor.|YT456789, BC4567890, 876546789|||||||
|event_data.type|string|Captures the type of video viewed.||||||||
|event_data.video_duration|integer|Captures the length of the video viewed by the visitor.|36, 67, 178, 600||||0|||
|event_data.video_milestones_reached|integer|Count of video milestones reached \(25%, 50%, 75%\).||||||||
|event_data.video_percent|string|Captures the milestone \(25%, 50%, 75%\) reached when viewing a video.|25, 50, 77, 99|||||||
|event_data.video_provider|string|Captures the video player used by the visitor for each video.|youTube, bright cove, JW Player, vimeo|||||||
|event_data.video_title|string|Captures the Name of video content viewed by visitor.|Twitch\_FPS, Age of Empires, Halo|||||||

## Attached Notes

<p><strong>Platform: harvardonline, PLL, VPAL</strong></p>
<p><em>TBD if we can just leverage Vimeo integration in GTM rather than have you code this to the dataLayer - please confirm prior to implementing.</em></p>
<p><span style="font-weight: 400;">Trigger this event when a user has reached a milestone (ie every 25% after starting with 0%) in a video.</span></p>
<p><span style="font-weight: 400;">Example page:</span></p>
<p><a href="https://www.harvardonline.harvard.edu/course/data-privacy-technology"><span style="font-weight: 400;">https://www.harvardonline.harvard.edu/course/data-privacy-technology</span></a><span style="font-weight: 400;">&nbsp;</span><span style="font-weight: 400;">(video is in the top-right)</span></p>
