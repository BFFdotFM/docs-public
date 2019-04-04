# Now Playing

{% api-method method="get" host="https://data.bff.fm" path="/nowplaying.txt" %}
{% api-method-summary %}
  
Get Now Playing
{% endapi-method-summary %}

{% api-method-description %}
What's currently playing on the BFF.fm stream.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="app\_id" type="string" required=false %}
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
Title: There Goes The Fear
Artist: Doves
Album: The Last Broadcast
Label: Heavenly
Artwork: https://a.bff.fm/image/original/trs2.jpg
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



