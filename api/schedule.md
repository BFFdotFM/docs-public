---
description: 'What''s on BFF.fm, and when.'
---

# Schedules

{% api-method method="get" host="https://data.bff.fm" path="/shows/all.ics" %}
{% api-method-summary %}
Full BFF.fm Schedule
{% endapi-method-summary %}

{% api-method-description %}
iCalendar for complete BFF.fm weekly schedule.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="app\_id" type="string" %}
You may include this parameter to identify your app in our stats, so that we can understand who's building cool stuff for BFF.fm and feature you!
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```text
BEGIN:VCALENDAR
PRODID:-//Best Frequencies\, Inc//BFF.FM//EN
VERSION:2.0
METHOD:PUBLISH
X-WR-CALNAME;CHARSET=utf-8:No Magic on BFF.fm
X-PUBLISHED-TTL:PT15M
CALSCALE:GREGORIAN
BEGIN:VTIMEZONE
TZID:America/Los_Angeles
BEGIN:DAYLIGHT
TZOFFSETFROM:-0800
RRULE:FREQ=YEARLY;BYMONTH=3;BYDAY=2SU
DTSTART:20070311T020000
TZNAME:PDT
TZOFFSETTO:-0700
END:DAYLIGHT
BEGIN:STANDARD
TZOFFSETFROM:-0700
RRULE:FREQ=YEARLY;BYMONTH=11;BYDAY=1SU
DTSTART:20071104T020000
TZNAME:PST
TZOFFSETTO:-0800
END:STANDARD
END:VTIMEZONE
BEGIN:VEVENT
UID:show-237@bff.fm
CLASS:PUBLIC
TRANSP:TRANSPARENT
LAST-MODIFIED:20190331T163606Z
SUMMARY;CHARSET=utf-8:We Let The Hats Decide on BFF.FM
DESCRIPTION;CHARSET=utf-8:DJ super-combo\, DJ Sanspants and DJ Pants\, write weird things down on pieces of paper. Those pieces of paper get folded up and placed into a super combination of hats\, fez and cowboy. We each pick pieces of paper out of those respective hats and whatever combination of words and phrases gets picked becomes the theme of the episode. It'll get wacky\, we promise.&nbsp\;\n\n
LOCATION:San Francisco\, CA
URL:https://bff.fm/shows/we-let-the-hats-decide
ORGANIZER;CN=BFF.FM:MAILTO:calendar@data.bff.fm
DTSTAMP:20190404T130000Z
DTSTART;TZID=America/Los_Angeles:20190404T060000
DTEND;TZID=America/Los_Angeles:20190404T080000
RRULE:FREQ=WEEKLY
SEQUENCE:0
BEGIN:VALARM
TRIGGER:-PT15M
DESCRIPTION:Tune-in to BFF.FM for We Let The Hats Decide!
ACTION:DISPLAY
END:VALARM
END:VEVENT
BEGIN:VEVENT
UID:show-330@bff.fm
CLASS:PUBLIC
TRANSP:TRANSPARENT
LAST-MODIFIED:20190331T163606Z
SUMMARY;CHARSET=utf-8:World of Echo on BFF.FM
DESCRIPTION;CHARSET=utf-8:
LOCATION:San Francisco\, CA
URL:https://bff.fm/shows/world-of-echo
ORGANIZER;CN=BFF.FM:MAILTO:calendar@data.bff.fm
DTSTAMP:20190401T140000Z
DTSTART;TZID=America/Los_Angeles:20190401T070000
DTEND;TZID=America/Los_Angeles:20190401T080000
RRULE:FREQ=WEEKLY
SEQUENCE:0
BEGIN:VALARM
TRIGGER:-PT15M
DESCRIPTION:Tune-in to BFF.FM for World of Echo!
ACTION:DISPLAY
END:VALARM
END:VEVENT
BEGIN:VEVENT
// …
END:VEVENT
END:VCALENDAR
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



{% api-method method="get" host="https://data.bff.fm" path="/shows/index/:day.ics" %}
{% api-method-summary %}
Single Day Schedule
{% endapi-method-summary %}

{% api-method-description %}
iCalendar schedule for a single day of BFF.fm broadcasts.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name=":day" type="string" required=true %}
Day of the week. \`monday\`, \`tuesday\`, \`wednesday\`, \`thursday\`, \`friday\`, \`saturday\`, \`sunday\`
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-query-parameters %}
{% api-method-parameter name="app\_id" type="string" required=false %}
You may include this parameter to identify your app in our stats, so that we can understand who's building cool stuff for BFF.fm and feature you!
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
BEGIN:VCALENDAR
PRODID:-//Best Frequencies\, Inc//BFF.FM//EN
VERSION:2.0
METHOD:PUBLISH
X-WR-CALNAME;CHARSET=utf-8:No Magic on BFF.fm
X-PUBLISHED-TTL:PT15M
CALSCALE:GREGORIAN
BEGIN:VTIMEZONE
TZID:America/Los_Angeles
BEGIN:DAYLIGHT
TZOFFSETFROM:-0800
RRULE:FREQ=YEARLY;BYMONTH=3;BYDAY=2SU
DTSTART:20070311T020000
TZNAME:PDT
TZOFFSETTO:-0700
END:DAYLIGHT
BEGIN:STANDARD
TZOFFSETFROM:-0700
RRULE:FREQ=YEARLY;BYMONTH=11;BYDAY=1SU
DTSTART:20071104T020000
TZNAME:PST
TZOFFSETTO:-0800
END:STANDARD
END:VTIMEZONE
BEGIN:VEVENT
UID:show-237@bff.fm
CLASS:PUBLIC
TRANSP:TRANSPARENT
LAST-MODIFIED:20190331T163606Z
SUMMARY;CHARSET=utf-8:We Let The Hats Decide on BFF.FM
DESCRIPTION;CHARSET=utf-8:DJ super-combo\, DJ Sanspants and DJ Pants\, write weird things down on pieces of paper. Those pieces of paper get folded up and placed into a super combination of hats\, fez and cowboy. We each pick pieces of paper out of those respective hats and whatever combination of words and phrases gets picked becomes the theme of the episode. It'll get wacky\, we promise.&nbsp\;\n\n
LOCATION:San Francisco\, CA
URL:https://bff.fm/shows/we-let-the-hats-decide
ORGANIZER;CN=BFF.FM:MAILTO:calendar@data.bff.fm
DTSTAMP:20190404T130000Z
DTSTART;TZID=America/Los_Angeles:20190404T060000
DTEND;TZID=America/Los_Angeles:20190404T080000
RRULE:FREQ=WEEKLY
SEQUENCE:0
BEGIN:VALARM
TRIGGER:-PT15M
DESCRIPTION:Tune-in to BFF.FM for We Let The Hats Decide!
ACTION:DISPLAY
END:VALARM
END:VEVENT
BEGIN:VEVENT
UID:show-330@bff.fm
CLASS:PUBLIC
TRANSP:TRANSPARENT
LAST-MODIFIED:20190331T163606Z
SUMMARY;CHARSET=utf-8:World of Echo on BFF.FM
DESCRIPTION;CHARSET=utf-8:
LOCATION:San Francisco\, CA
URL:https://bff.fm/shows/world-of-echo
ORGANIZER;CN=BFF.FM:MAILTO:calendar@data.bff.fm
DTSTAMP:20190401T140000Z
DTSTART;TZID=America/Los_Angeles:20190401T070000
DTEND;TZID=America/Los_Angeles:20190401T080000
RRULE:FREQ=WEEKLY
SEQUENCE:0
BEGIN:VALARM
TRIGGER:-PT15M
DESCRIPTION:Tune-in to BFF.FM for World of Echo!
ACTION:DISPLAY
END:VALARM
END:VEVENT
BEGIN:VEVENT
// …
END:VEVENT
END:VCALENDAR
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://data.bff.fm" path="/shows/:show.ics" %}
{% api-method-summary %}
Specific Show Schedule
{% endapi-method-summary %}

{% api-method-description %}
iCalendar for a specific BFF.fm show.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name=":show" type="string" required=true %}
The slug for the show
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-query-parameters %}
{% api-method-parameter name="app\_id" type="string" required=false %}
You may include this parameter to identify your app in our stats, so that we can understand who's building cool stuff for BFF.fm and feature you!
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```text
BEGIN:VCALENDAR
PRODID:-//Best Frequencies\, Inc//BFF.FM//EN
VERSION:2.0
METHOD:PUBLISH
X-WR-CALNAME;CHARSET=utf-8:No Magic on BFF.fm
X-PUBLISHED-TTL:PT15M
CALSCALE:GREGORIAN
BEGIN:VTIMEZONE
TZID:America/Los_Angeles
BEGIN:DAYLIGHT
TZOFFSETFROM:-0800
RRULE:FREQ=YEARLY;BYMONTH=3;BYDAY=2SU
DTSTART:20070311T020000
TZNAME:PDT
TZOFFSETTO:-0700
END:DAYLIGHT
BEGIN:STANDARD
TZOFFSETFROM:-0700
RRULE:FREQ=YEARLY;BYMONTH=11;BYDAY=1SU
DTSTART:20071104T020000
TZNAME:PST
TZOFFSETTO:-0800
END:STANDARD
END:VTIMEZONE
BEGIN:VEVENT
UID:show-309@bff.fm
CLASS:PUBLIC
TRANSP:TRANSPARENT
LAST-MODIFIED:20190331T163836Z
SUMMARY;CHARSET=utf-8:No Magic on BFF.FM
DESCRIPTION;CHARSET=utf-8:An evening session with&nbsp\;Ben Ward playing eclectic blends of pop\, rock\, electronic\, dance and whatever else seems tangentially appropriate. A featured guest brings along their musical inspirations and stories\, and we'll pour over the record of the week. “This isn't about looking good.&nbsp\;This isn't about making people like you.&nbsp\;No magic\, just music.”\n\n
LOCATION:San Francisco\, CA
URL:https://bff.fm/shows/nomagic
ORGANIZER;CN=BFF.FM:MAILTO:calendar@data.bff.fm
DTSTAMP:20190403T030000Z
DTSTART;TZID=America/Los_Angeles:20190402T200000
DTEND;TZID=America/Los_Angeles:20190402T220000
RRULE:FREQ=WEEKLY
SEQUENCE:0
BEGIN:VALARM
TRIGGER:-PT15M
DESCRIPTION:Tune-in to BFF.FM for No Magic!
ACTION:DISPLAY
END:VALARM
END:VEVENT
END:VCALENDAR
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

