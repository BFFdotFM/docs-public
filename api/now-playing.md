# Now Playing

## Unified Metadata

{% swagger method="get" path="/api/data/onair/now.json" baseUrl="https://data.bff.fm" summary="On Air" %}
{% swagger-description %}
An endpoint which will return what's currently playing on BFF.fm at the finest fidelity available: the track, or current playing show.
{% endswagger-description %}

{% swagger-parameter in="query" name="app_id" %}
You may include this parameter to identify your app in our stats, so that we can understand who's building cool stuff for BFF.fm and feature you!
{% endswagger-parameter %}

{% swagger-response status="200: OK" description="" %}
Example Track response

```
{
   title: I NEED YOU TO (BREONNA TAYLOR)
   attribution: Tobe Nwigwe
   collection: THE PANDEMIC PROJECT
   licensor: Self Released
   image: https://a.bff.fm/…/album.jpg
   url: https://bff.fm/broadcasts/234345324
   type: track
}
```

Example Show response

```
{
   title: No Magic
   attribution: Ben Ward
   collection: BFF.fm
   licensor: BFF.fm
   image: https://a.bff.fm/…/logo.jpg
   url: https://bff.fm/shows/nomagic
   type: show
}
```


{% endswagger-response %}
{% endswagger %}

## Track Metadata

{% swagger baseUrl="https://data.bff.fm" path="/api/data/tracks/detail.text" method="get" summary="Detailed Metadata" %}
{% swagger-description %}
What's currently playing on the BFF.fm stream.
{% endswagger-description %}

{% swagger-parameter in="query" name="app_id" type="string" %}
You may include this parameter to identify your app in our stats, so that we can understand who's building cool stuff for BFF.fm and feature you!
{% endswagger-parameter %}

{% swagger-response status="200" description="Cake successfully retrieved." %}
```
Title: There Goes The Fear
Artist: Doves
Album: The Last Broadcast
Label: Heavenly
Artwork: https://a.bff.fm/image/original/trs2.jpg
```
{% endswagger-response %}
{% endswagger %}

{% hint style="info" %}
See Also: [Audio Hijack Pro's “Now Playing.txt” documentation](https://rogueamoeba.com/support/knowledgebase/?showArticle=AHBroadcastNotes#nowplayingfile).
{% endhint %}

{% swagger baseUrl="https://data.bff.fm" path="/api/data/tracks/now.text" method="get" summary="One-Line Summary" %}
{% swagger-description %}
A single-line summary of what's playing on BFF.fm. `Track Name` followed by `Artist`, separated by `-`.
{% endswagger-description %}

{% swagger-parameter in="query" name="app_id" type="string" %}
You may include this parameter to identify your app in our stats, so that we can understand who's building cool stuff for BFF.fm and feature you!
{% endswagger-parameter %}

{% swagger-response status="200" description="" %}
```
Because It's Not Love (But It's Still A Feeling) - The Pipettes
```
{% endswagger-response %}
{% endswagger %}

{% swagger method="get" path="/api/data/tracks/now.json" baseUrl="https://data.bff.fm" summary="JSON structured Detailed Metadata" %}
{% swagger-description %}
The current artist, track, album and record label being played on BFF.fm
{% endswagger-description %}

{% swagger-parameter in="query" name="app_id" %}
You may include this parameter to identify your app in our stats, so that we can understand who's building cool stuff for BFF.fm and feature you!
{% endswagger-parameter %}
{% endswagger %}

