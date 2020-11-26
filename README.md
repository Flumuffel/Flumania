# Api

{% api-method method="get" host="https://filme.flummy.tk/api" path="/v1/search/?id \| ?q" %}
{% api-method-summary %}
Search
{% endapi-method-summary %}

{% api-method-description %}
The Endpoint for anime search.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="q" type="string" required=false %}
Search for a anime
{% endapi-method-parameter %}

{% api-method-parameter name="id" type="number" %}
Id of the anime data
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```
{
    "Page": {
        "media": [{
            "id": 11433,
            "title": {
                "romaji": "Ano Natsu de Matteru",
                "english": "Waiting in the Summer",
                "native": "あの夏で待ってる",
                "userPreferred": "Ano Natsu de Matteru"
            },
            "coverImage": {
                "extraLarge": "https://s4.anilist.co/file/anilistcdn/media/anime/cover/large/bx11433-KLEzZeK6D46g.jpg",
                "large": "https://s4.anilist.co/file/anilistcdn/media/anime/cover/medium/bx11433-KLEzZeK6D46g.jpg",
                "medium": "https://s4.anilist.co/file/anilistcdn/media/anime/cover/small/bx11433-KLEzZeK6D46g.jpg",
                "color": "#e45050"
            },
            "description": "When a group of friends decide to make a movie over a long summer holiday, they end up learning a little about filmmaking and a lot more about each other and themselves. What begins as a simple way to avoid the summer doldrums quickly turns into something much more complex, intimate and revealing, as the maturing relationships between the members of the young cast take on new, and sometimes very unexpected, turns. <br><br>\r\n(Source: Sentai Filmworks) ",
            "status": "FINISHED",
            "episodes": 12,
            "isLicensed": true,
            "source": "ORIGINAL",
            "trailer": null,
            "popularity": 38710,
            "airingSchedule": {
                "edges": []
            }
        }]
    }
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```
{
    "Page": {
        "media": []
    }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



