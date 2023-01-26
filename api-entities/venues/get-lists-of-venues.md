# Get lists of venues

You can get lists of venues:

* Get _all_ venues in OpenAlex\
  [https://api.openalex.org/venues](https://api.openalex.org/venues)

Which returns a response like this:

```json
{
    "meta": {
        "count": 226727,
        "db_response_time_ms": 32,
        "page": 1,
        "per_page": 25
    },
    "results": [
        {
            "id": "https://openalex.org/V2764455111",
            "issn_l": null,
            "issn": null,
            "display_name": "PubMed Central",
            // more fields (removed to save space)
        },
        {
            "id": "https://openalex.org/V4306400806",
            "issn_l": null,
            "issn": null,
            "display_name": "PubMed Central - Europe PMC",
            // more fields (removed to save space)
        },
        // more results (removed to save space)
    ],
    "group_by": []
}
```

## Page and sort venues

By default we return 25 results per page. You can change this default and [page](../../how-to-use-the-api/get-lists-of-entities/paging.md) through venues with the `per-page` and `page` parameters:

* Get the second page of venues results, with 50 results returned per page\
  [https://api.openalex.org/venues?per-page=50\&page=2](https://api.openalex.org/venues?per-page=50\&page=2)

You also can [sort results](../../how-to-use-the-api/get-lists-of-entities/sort-entity-lists.md) with the `sort` parameter:

* Sort venues by cited by count, descending\
  [https://api.openalex.org/venues?sort=cited\_by\_count:desc](https://api.openalex.org/venues?sort=cited\_by\_count:desc)

Continue on to learn how you can [filter](filter-venues.md) and [search](search-venues.md) lists of venues.