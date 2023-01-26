# Get lists of authors

You can get lists of authors:

* Get _all_ authors in OpenAlex\
  [https://api.openalex.org/authors](https://api.openalex.org/authors)

Which returns a response like this:

```json
{
    "meta": {
        "count": 264762265,
        "db_response_time_ms": 81,
        "page": 1,
        "per_page": 25
    },
    "results": [
        {
            "id": "https://openalex.org/A2479313101",
            "orcid": "https://orcid.org/0000-0002-7436-3176",
            "display_name": "Charles Thomas Parker",
            // more fields (removed to save space)
        },
        {
            "id": "https://openalex.org/A2307396757",
            "orcid": "https://orcid.org/0000-0002-4465-7034",
            "display_name": "George M. Garrity",
            // more fields (removed to save space)
        },
        // more results (removed to save space)
    ],
    "group_by": []
}
```

## Page and sort authors

By default we return 25 results per page. You can change this default and [page](../../how-to-use-the-api/get-lists-of-entities/paging.md) through works with the `per-page` and `page` parameters:

* Get the second page of authors results, with 50 results returned per page\
  [https://api.openalex.org/authors?per-page=50\&page=2](https://api.openalex.org/authors?per-page=50\&page=2)

You also can [sort results](../../how-to-use-the-api/get-lists-of-entities/sort-entity-lists.md) with the `sort` parameter:

* Sort authors by cited by count, descending\
  [https://api.openalex.org/authors?sort=cited\_by\_count:desc](https://api.openalex.org/authors?sort=cited\_by\_count:desc)

Continue on to learn how you can [filter](filter-authors.md) and [search](search-authors.md) lists of authors.