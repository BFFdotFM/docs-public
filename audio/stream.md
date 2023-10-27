---
description: Get BFF.fm playback live in your app.
---

# Live Broadcast

{% swagger baseUrl="https://stream.bff.fm" path="/1/mp3.format" method="get" summary="MP3 Audio Stream" %}
{% swagger-description %}
The live BFF.fm broadcast is available encoded in MP3, packaged in a variety of formats.
{% endswagger-description %}

{% swagger-parameter in="path" name="format" type="string" %}
The playlist format desired: \`mp3\`, \`xspf\`, \`pls\`, \`m3u\`
{% endswagger-parameter %}

{% swagger-parameter in="header" name="User-Agent" type="string" %}
The name of your app, so that we can better understand a little bit about how our listeners prefer to hear BFF.fm
{% endswagger-parameter %}

{% swagger-parameter in="query" name="app_id" type="string" %}
You may include this parameter to identify your app in our stats, so that we can understand who's building cool stuff for BFF.fm and feature you!
{% endswagger-parameter %}

{% swagger-response status="200" description="" %}
{% tabs %}
{% tab title="mp3.mp3" %}
{% code title="mp3.mp3" %}
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
{% endcode %}
{% endtab %}

{% tab title="mp3.m3u" %}
{% code title="mp3.m3u" %}
```
http://stream.bff.fm/1/mp3.mp3

```
{% endcode %}
{% endtab %}

{% tab title="mp3.pls" %}
{% code title="mp3.pls" %}
```
[playlist]
File1=http://stream.bff.fm/1/mp3.mp3
Title1=BFF.fm – Best Frequencies Forever
Length1=-1
NumberOfEntries=1
Version=2
```
{% endcode %}
{% endtab %}

{% tab title="mp3.xspf" %}
{% code title="mp3.xspf" %}
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
{% endcode %}
{% endtab %}
{% endtabs %}
{% endswagger-response %}
{% endswagger %}

