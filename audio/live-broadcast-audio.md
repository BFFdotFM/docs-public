---
description: Get BFF.fm playback live in your app.
---

# Live Broadcast

{% api-method method="get" host="https://stream.bff.fm" path="/1/mp3.format" %}
{% api-method-summary %}
MP3 Audio Stream
{% endapi-method-summary %}

{% api-method-description %}
The live BFF.fm broadcast is available encoded in MP3, packaged in a variety of formats.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="format" type="string" required=true %}
The playlist format desired: \`mp3\`, \`xspf\`, \`pls\`, \`m3u\`
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="User-Agent" type="string" required=true %}
The name of your app, so that we can better understand a little bit about how our listeners prefer to hear BFF.fm
{% endapi-method-parameter %}
{% endapi-method-headers %}

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

{% code-tabs %}
{% code-tabs-item title="mp3.mp3" %}
```http
HTTP/1.0 200 OK
Access-Control-Expose-Headers: ETag, If-None-Match
Access-Control-Allow-Credentials: true
X-Loudness: -16.089101
icy-br: 128
icy-pub: 1
icy-description: BFF.fm
icy-audio-info: ice-samplerate=44100;ice-bitrate=128;ice-channels=2
Access-Control-Allow-Origin: *
icy-url: http://www.bff.fm
Instance-id: b753d6e5219ea5c48947a2de2cb08a58
Cache-Control: no-cache
Server: AIS Streaming Server 8.0.14
icy-genre: Pop
Expires: Mon, 26 Jul 1997 05:00:00 GMT
icy-metaint: 0
Access-Control-Allow-Headers: ETag, If-None-Match
Pragma: no-cache
icy-name: BFF.fm
Connection: close
Content-Type: audio/mpeg

[MP3 Binary Data]
```
{% endcode-tabs-item %}

{% code-tabs-item title="mp3.m3u" %}
```
http://stream.bff.fm/1/mp3.mp3

```
{% endcode-tabs-item %}

{% code-tabs-item title="mp3.pls" %}
```
[playlist]
File1=http://stream.bff.fm/1/mp3.mp3
Title1=BFF.fm – Best Frequencies Forever
Length1=-1
NumberOfEntries=1
Version=2
```
{% endcode-tabs-item %}

{% code-tabs-item title="mp3.xspf" %}
```markup
<?xml version="1.0" encoding="UTF-8"?>
<playlist xmlns="http://xspf.org/ns/0/" version="1">
  <title>BFF.fm – Best Frequencies Forever</title>
  <creator>Best Frequencies, Inc</creator>
  <info>https://bff.fm</info>
  <image>https://a.bff.fm/w/assets/favicons/apple-touch-icon/670e7f66554fa4d50219e02bee256e233047dc1e.png</image>
  <trackList>
    <track>
      <location>http://stream.bff.fm/1/mp3.mp3</location>
      <title>BFF.fm</title>
      <info>https://bff.fm</info>
    </track>
  </trackList>
</playlist>
```
{% endcode-tabs-item %}
{% endcode-tabs %}
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



