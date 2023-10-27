---
description: Feeds for show archives.
---

# Shows & Podcasts

{% swagger baseUrl="https://data.bff.fm" path="/shows/:show.rss" method="get" summary="Single Show Podcast" %}
{% swagger-description %}
RSS feed of a specific show.
{% endswagger-description %}

{% swagger-parameter in="path" name="show" type="string" %}
Slug name for the show being requested
{% endswagger-parameter %}

{% swagger-parameter in="query" name="app_id" type="string" %}
You may include this parameter to identify your app in our stats, so that we can understand who's building cool stuff for BFF.fm and feature you!
{% endswagger-parameter %}

{% swagger-response status="200" description="RSS feed, with iTunes extensions." %}
```markup
<?xml version="1.0" encoding="UTF-8"?>
<rss version="2.0" 
  xmlns:atom="http://www.w3.org/2005/Atom" 
  xmlns:itunes="http://www.itunes.com/dtds/podcast-1.0.dtd">
  <channel>
    <title>No Magic - BFF.fm</title>
    <description>No Magic with Ben Ward on BFF.fm. Listen to show archives, or tune in live Tuesday 8:00 – 10:00pm. BFF.fm is a San Francisco-based community radio station. Our mission is to support emerging and underground artists and bring the Bay Area music scene to the world.</description>
    <itunes:summary><![CDATA[<p>An evening session with&nbsp;<a href="https://bff.fm/people/benward">Ben Ward</a> playing eclectic blends of pop, rock, electronic, dance and whatever else seems tangentially appropriate. A featured guest brings along their musical inspirations and stories, and we'll pour over the record of the week. <i>“This isn't about looking good.&nbsp;This isn't about making people like you.&nbsp;No magic, just music.”</i></p>]]></itunes:summary>
    <link>https://bff.fm/shows/nomagic</link>
    <atom:link href="https://data.bff.fm/shows/nomagic.rss" rel="self" type="application/rss+xml" />
    <lastBuildDate>Sun, 31 Mar 2019 16:50:16 +0000</lastBuildDate>
    <pubDate>Sun, 31 Mar 2019 16:50:16 +0000</pubDate>
    <language>en-us</language>
    <copyright>Copyright © 2019 BFF.fm</copyright>

    <image>
      <url>https://a.bff.fm/image/itunes/No_Magic_3.jpg</url>
      <link>https://bff.fm/shows/nomagic</link>
      <title>No Magic - BFF.fm</title>
    </image>
    <itunes:image href="https://a.bff.fm/image/itunes/No_Magic_3.jpg" />

    <itunes:owner>
      <itunes:name>BFF.fm</itunes:name>
      <itunes:email>podcasts@bff.fm</itunes:email>
    </itunes:owner>

    <atom:author>
      <atom:name>Ben Ward</atom:name>
      <atom:uri>https://bff.fm/people/benward</atom:uri>
    </atom:author>
    <itunes:author>BFF.fm / Ben Ward</itunes:author>

    <itunes:explicit>yes</itunes:explicit>
    <itunes:category text="Music" />

    <item>
      <link>https://bff.fm/broadcasts/17865</link>
      <guid isPermaLink="false">tag:bff.fm,2019-03-26:/broadcasts/17865</guid>
      <pubDate>Tue, 26 Mar 2019 20:00:00 +0000</pubDate>

      <title>#13: From the East</title>
      <itunes:title>From the East</itunes:title>

      <itunes:episodeType>full</itunes:episodeType>
      <itunes:episode>13</itunes:episode>
      <enclosure url="https://a.bff.fm/audio/nomagic/NoMagic-13.mp3" length="232918004" type="audio/mpeg" />

      <description><![CDATA[<p>This week's show was recorded by Ben in a hotel room in Minsk, Belarus. It's a solo effort, packed full of new music and features the really wonderful new album from&nbsp;<b>The Cinematic Orchestra<i></i></b><i></i>;&nbsp;<i>To Belong&nbsp;</i>is a great record, supported by really excellent vocal collaborations with the likes of <b>Moses Sumney</b> and <b>Roots Manuva</b>. Enjoy!</p>
      <p><strong><a href="https://bff.fm/broadcasts/17865#support">Enjoying the show? Please support BFF.FM with a donation.</a></strong></p>
      <section itemscope itemtype="https://schema.org/MusicPlaylist">
      <h3 itemprop="name">Playlist</h3>
      <ol>
      <li itemprop="track" itemscope itemtype="https://schema.org/MusicRecording">
      <time datetime="2019-03-27T03:00:00+00:00">0′00″</time><strong itemprop="recordingOf">Where We&#039;re Calling From</strong> by <strong itemprop="byArtist">Doves</strong> on <span itemprop="inAlbum">The Last Broadcast</span> (<span itemprop="publisher">Heavenly</span>)</li>
      <li itemprop="track" itemscope itemtype="https://schema.org/MusicRecording">
      <time datetime="2019-03-27T03:01:27+00:00">1′27″</time><strong itemprop="recordingOf">Lights Out For Darker Skies</strong> by <strong itemprop="byArtist">British Sea Power</strong> on <span itemprop="inAlbum">Do You Like Rock Music</span> (<span itemprop="publisher">Rough Trade</span>)</li>
      <li itemprop="track" itemscope itemtype="https://schema.org/MusicRecording">
      <time datetime="2019-03-27T03:07:59+00:00">7′59″</time><strong itemprop="recordingOf">Dream Variations</strong> by <strong itemprop="byArtist">Idlewild</strong> on <span itemprop="inAlbum">Interview Music</span></li>
      <li itemprop="track" itemscope itemtype="https://schema.org/MusicRecording">
      <time datetime="2019-03-27T03:15:06+00:00">15′06″</time><strong itemprop="recordingOf">Bellyache</strong> by <strong itemprop="byArtist">Yak</strong> on <span itemprop="inAlbum">Pursuit of Momentary Happiness</span> (<span itemprop="publisher">Universal</span>)</li>
      <li itemprop="track" itemscope itemtype="https://schema.org/MusicRecording">
      <time datetime="2019-03-27T03:18:46+00:00">18′46″</time><strong itemprop="recordingOf">My Mouth Ain&#039;t No Bible</strong> by <strong itemprop="byArtist">James Yorkston</strong> on <span itemprop="inAlbum">The Route To The Harmonium</span> (<span itemprop="publisher">Domino</span>)</li>
      <li itemprop="track" itemscope itemtype="https://schema.org/MusicRecording">
      <time datetime="2019-03-27T03:25:25+00:00">25′25″</time><strong itemprop="recordingOf">Strange Secrets Worth Knowing</strong> by <strong itemprop="byArtist">Improvement Movement</strong> on <span itemprop="inAlbum">Strange Secrets Worth Knowing</span></li>
      <li itemprop="track" itemscope itemtype="https://schema.org/MusicRecording">
      <time datetime="2019-03-27T03:27:25+00:00">27′25″</time><strong itemprop="recordingOf">Chain of Being</strong> by <strong itemprop="byArtist">Crows</strong> on <span itemprop="inAlbum">Chain of Being</span></li>
      <li itemprop="track" itemscope itemtype="https://schema.org/MusicRecording">
      <time datetime="2019-03-27T03:35:49+00:00">35′49″</time><strong itemprop="recordingOf">A Caged Bird/Imitations of Life (feat. Roots Manuva)</strong> by <strong itemprop="byArtist">The Cinematic Orchestra</strong> on <span itemprop="inAlbum">A Caged Bird/Imitations of Life (feat. Roots Manuva)</span> (<span itemprop="publisher">Ninja Tune</span>)</li>
      <li itemprop="track" itemscope itemtype="https://schema.org/MusicRecording">
      <time datetime="2019-03-27T03:42:39+00:00">42′39″</time><strong itemprop="recordingOf">First of the Tide (feat. Benge)</strong> by <strong itemprop="byArtist">Erland Cooper</strong> on <span itemprop="inAlbum">Sule Skerry</span> (<span itemprop="publisher">Phases</span>)</li>
      <li itemprop="track" itemscope itemtype="https://schema.org/MusicRecording">
      <time datetime="2019-03-27T03:45:56+00:00">45′56″</time><strong itemprop="recordingOf">Willow (feat. Robert Pattinson)</strong> by <strong itemprop="byArtist">Tindersticks</strong> on <span itemprop="inAlbum">“High Life” OST</span></li>
      <li itemprop="track" itemscope itemtype="https://schema.org/MusicRecording">
      <time datetime="2019-03-27T03:53:59+00:00">53′59″</time><strong itemprop="recordingOf">Zero One/This Fantasty (feat. Grey Reverend)</strong> by <strong itemprop="byArtist">The Cinematic Orchestra</strong> on <span itemprop="inAlbum">To Believe</span> (<span itemprop="publisher">Ninja Tune</span>)</li>
      <li itemprop="track" itemscope itemtype="https://schema.org/MusicRecording">
      <time datetime="2019-03-27T04:00:50+00:00">60′50″</time><strong itemprop="recordingOf">Home (feat. Tina Dico)</strong> by <strong itemprop="byArtist">Zero 7</strong> on <span itemprop="inAlbum">When it Falls</span> (<span itemprop="publisher">New State</span>)</li>
      <li itemprop="track" itemscope itemtype="https://schema.org/MusicRecording">
      <time datetime="2019-03-27T04:05:15+00:00">65′15″</time><strong itemprop="recordingOf">Bats in the Attic</strong> by <strong itemprop="byArtist">Jon Hopkins and King Creosote</strong> on <span itemprop="inAlbum">Diamond Mine</span> (<span itemprop="publisher">Domino</span>)</li>
      <li itemprop="track" itemscope itemtype="https://schema.org/MusicRecording">
      <time datetime="2019-03-27T04:08:38+00:00">68′38″</time><strong itemprop="recordingOf">One by One</strong> by <strong itemprop="byArtist">Dana Gavanski</strong> on <span itemprop="inAlbum">One by One</span> (<span itemprop="publisher">Full Time Hobby</span>)</li>
      <li itemprop="track" itemscope itemtype="https://schema.org/MusicRecording">
      <time datetime="2019-03-27T04:17:27+00:00">77′27″</time><strong itemprop="recordingOf">Ladies and Gentlemen</strong> by <strong itemprop="byArtist">Bronx Slang</strong> on <span itemprop="inAlbum">Bronx Slang</span></li>
      <li itemprop="track" itemscope itemtype="https://schema.org/MusicRecording">
      <time datetime="2019-03-27T04:20:14+00:00">80′14″</time><strong itemprop="recordingOf">Rubber Bullets</strong> by <strong itemprop="byArtist">Clinic</strong> on <span itemprop="inAlbum">Rubber Bullets</span></li>
      <li itemprop="track" itemscope itemtype="https://schema.org/MusicRecording">
      <time datetime="2019-03-27T04:22:35+00:00">82′35″</time><strong itemprop="recordingOf">Out of Body</strong> by <strong itemprop="byArtist">The Years</strong> on <span itemprop="inAlbum">Out of Body</span></li>
      <li itemprop="track" itemscope itemtype="https://schema.org/MusicRecording">
      <time datetime="2019-03-28T04:28:44+00:00">88′44″</time><strong itemprop="recordingOf">A Promise (feat. Heidi Vogel)</strong> by <strong itemprop="byArtist">The Cinematic Orchestra</strong> on <span itemprop="inAlbum">To Believe</span> (<span itemprop="publisher">Ninja Tune</span>)</li>
      <li itemprop="track" itemscope itemtype="https://schema.org/MusicRecording">
      <time datetime="2019-03-28T04:40:10+00:00">100′10″</time><strong itemprop="recordingOf">In The Dark (feat. Toulouse)</strong> by <strong itemprop="byArtist">Anaïs</strong> on <span itemprop="inAlbum">Lost my Faith</span> (<span itemprop="publisher">Universal</span>)</li>
      <li itemprop="track" itemscope itemtype="https://schema.org/MusicRecording">
      <time datetime="2019-03-28T04:44:13+00:00">104′13″</time><strong itemprop="recordingOf">Summer Blues</strong> by <strong itemprop="byArtist">Will Burns and Hannah Peel</strong> on <span itemprop="inAlbum">Chalk Hill Blue</span> (<span itemprop="publisher">Rivertones</span>)</li>
      <li itemprop="track" itemscope itemtype="https://schema.org/MusicRecording">
      <time datetime="2019-03-28T04:51:57+00:00">111′57″</time><strong itemprop="recordingOf">Sleep</strong> by <strong itemprop="byArtist">Son Lux</strong> on <span itemprop="inAlbum">Remnants</span></li>
      <li itemprop="track" itemscope itemtype="https://schema.org/MusicRecording">
      <time datetime="2019-03-28T04:56:27+00:00">116′27″</time><strong itemprop="recordingOf">Tutti</strong> by <strong itemprop="byArtist">Cosey Fanni Tutti</strong> on <span itemprop="inAlbum">TUTTI</span></li>
      </ol>
      </section>]]></description>
    </item>
  </channel>
</rss>
```
{% endswagger-response %}
{% endswagger %}

{% swagger baseUrl="https://data.bff.fm" path="/api/data/shows/all.opml" method="get" summary="All Shows Index" %}
{% swagger-description %}
OPML outline for all shows on BFF.fm, linking to respective RSS feeds.
{% endswagger-description %}

{% swagger-parameter in="query" name="app_id" type="string" %}
You may include this parameter to identify your app in our stats, so that we can understand who's building cool stuff for BFF.fm and feature you!
{% endswagger-parameter %}

{% swagger-response status="200" description="OPML outline of all BFF.fm shows (truncated.)" %}
```markup
<?xml version="1.0" encoding="utf-8" ?>
<opml version="2.0">
  <head>
    <title>Programs - BFF.fm</title>
    <dateCreated>Sun, 31 Mar 19 16:58:37 +0000</dateCreated>
    <ownerName>BFF.fm</ownerName>
    <ownerId>https://bff.fm</ownerId>
  </head>
  <body>
    <outline text="feeds">
      <outline type="rss" text="@indierockgirl radio" xmlUrl="https://data.bff.fm/shows/indierockgirl-radio.rss" htmlUrl="https://bff.fm/shows/indierockgirl-radio" category="Garage" />
      <outline type="rss" text="@Jon_Digital" xmlUrl="https://data.bff.fm/shows/jon-digital.rss" htmlUrl="https://bff.fm/shows/jon-digital" category="Pop,R&amp;B / Soul,Electronic" />
      <outline type="rss" text="A Thick Mist" xmlUrl="https://data.bff.fm/shows/a-thick-mist.rss" htmlUrl="https://bff.fm/shows/a-thick-mist" category="World,Rock,Experimental,Electronic" />
      <outline type="rss" text="Abuela&#039;s Pantry" xmlUrl="https://data.bff.fm/shows/abuela-s-pantry.rss" htmlUrl="https://bff.fm/shows/abuela-s-pantry" category="Local,Pop" />
      <!-- … -->
    </outline>
  </body>
</opml>
```
{% endswagger-response %}
{% endswagger %}

{% swagger method="get" path="/api/data/shows/scheduled.opml" baseUrl="https://data.bff.fm" summary="Schedule Index" %}
{% swagger-description %}
OPML outline including all shows that are regularly scheduled.
{% endswagger-description %}

{% swagger-parameter in="query" name="app_id" %}
You may include this parameter to identify your app in our stats, so that we can understand who's building cool stuff for BFF.fm and feature you!
{% endswagger-parameter %}

{% swagger-response status="200: OK" description="OPML outline of shows scheduled on the specified day." %}
```javascript
{
    // Response
}
```
{% endswagger-response %}
{% endswagger %}

{% swagger method="get" path="/api/data/shows/day/:day.opml" baseUrl="https://data.bff.fm" summary="Day Index" %}
{% swagger-description %}
OPML outline for day scheduled show linking to respective RSS feeds.
{% endswagger-description %}

{% swagger-parameter in="path" name="day" required="true" %}
Name of the schedule day to return. One of `monday` , `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `sunday`
{% endswagger-parameter %}

{% swagger-parameter in="query" name="app_id" %}
You may include this parameter to identify your app in our stats, so that we can understand who's building cool stuff for BFF.fm and feature you!
{% endswagger-parameter %}

{% swagger-response status="200: OK" description="OPML outline of shows scheduled on the specified day." %}
```javascript
{
    // Response
}
```
{% endswagger-response %}
{% endswagger %}

{% swagger method="get" path="/api/data/shows/podcasts.opml" baseUrl="https://data.bff.fm" summary="Podcasts Index" %}
{% swagger-description %}
OPML outline for all Podcasts in the BFF.fm Podcast Network.
{% endswagger-description %}

{% swagger-parameter in="query" name="app_id" %}
You may include this parameter to identify your app in our stats, so that we can understand who's building cool stuff for BFF.fm and feature you!
{% endswagger-parameter %}

{% swagger-response status="200: OK" description="OPML outline of shows scheduled on the specified day." %}
```javascript
{
    // Response
}
```
{% endswagger-response %}
{% endswagger %}
