# Group works

You can group works with the `group_by` parameter:

* Get counts of works by Open Access status:\
  [`https://api.openalex.org/works?group_by=oa_status`](https://api.openalex.org/works?group\_by=oa\_status)

Or you can group using one the attributes below.

{% hint style="info" %}
It's best to [read about group by](../../how-to-use-the-api/get-groups-of-entities.md) before trying these out. It will show you how results are formatted, the number of results returned, and how to sort results.
{% endhint %}

### `/works` group\_by attributes

{% hint style="danger" %}
The `host_venue` and `alternate_host_venues` properties have been deprecated in favor of [`primary_location`](work-object/#primary\_location) and [`locations`](work-object/#locations). The attributes `host_venue` and `alternate_host_venues` are no longer available in the Work object, and trying to access them in filters or group-bys will return an error.
{% endhint %}

* [`authors_count`](filter-works.md#authors\_count)
* [`authorships.author.id`](work-object/#author) (alias `author.id`)
* [`authorships.author.orcid`](work-object/#author) (alias `author.orcid`)
* [`authorships.countries`](work-object/authorship-object.md#countries)
* [`authorships.institutions.country_code`](work-object/#institutions) (alias `institutions.country_code`)
* [`authorships.institutions.continent`](filter-works.md#authorships.institutions.continent-alias-institutions.continent) (alias `institutions.continent`)
* [`authorships.institutions.is_global_south`](filter-works.md#authorships.institutions.is\_global\_south-alias-institutions.is\_global\_south)
* [`authorships.institutions.id`](work-object/#institutions) (alias `institutions.id`)
* [`authorships.institutions.lineage`](work-object/authorship-object.md#institutions)
* [`authorships.institutions.ror`](work-object/#institutions) (alias `institutions.ror`)
* [`authorships.institutions.type`](work-object/#institutions) (alias `institutions.type`)
* [`authorships.is_corresponding`](work-object/authorship-object.md#is\_corresponding) (alias: `is_corresponding`): this marks whether or not we have corresponding author information for a given work
* [`apc_list.value`](work-object/#apc\_list)
* [`apc_list.currency`](work-object/#apc\_list)
* [`apc_list.provenance`](work-object/#apc\_list)
* [`apc_list.value_usd`](work-object/#apc\_list)
* [`apc_paid.value`](work-object/#apc\_paid)
* [`apc_paid.currency`](work-object/#apc\_paid)
* [`apc_paid.provenance`](work-object/#apc\_paid)
* [`apc_paid.value_usd`](work-object/#apc\_paid)
* [`best_oa_location.is_accepted`](work-object/#best\_oa\_location)
* [`best_oa_location.is_published`](work-object/#best\_oa\_location)
* [`best_oa_location.license`](work-object/#best\_oa\_location)
* [`best_oa_location.source.host_organization`](work-object/#best\_oa\_location)
* [`best_oa_location.source.id`](work-object/#best\_oa\_location)
* [`best_oa_location.source.is_in_doaj`](work-object/#best\_oa\_location)
* [`best_oa_location.source.issn`](work-object/#best\_oa\_location)
* [`best_oa_location.source.type`](work-object/#best\_oa\_location)
* [`best_oa_location.version`](work-object/#best\_oa\_location)
* [`best_open_version`](filter-works.md#best\_open\_version)
* [`cited_by_count`](work-object/#cited\_by\_count)
* [`cites`](filter-works.md#cites)
* [`concepts_count`](filter-works.md#concepts\_count)
* [`concepts.id`](work-object/#concepts)
* [`concepts.wikidata`](work-object/#concepts)
* [`corresponding_author_ids`](work-object/#corresponding\_author\_ids)
* [`corresponding_institution_ids`](work-object/#corresponding\_institution\_ids)
* [`countries_distinct_count`](work-object/README.md#countries_distinct_count)
* [`grants.award_id`](work-object/#grants)
* [`grants.funder`](work-object/#grants)
* [`has_abstract`](filter-works.md#has\_abstract)
* [`has_doi`](filter-works.md#has\_doi)
* [`has_orcid`](filter-works.md#has\_orcid)
* [`has_pmid`](filter-works.md#has\_pmid)
* [`has_pmcid`](filter-works.md#has\_pmcid)
* [`has_ngrams`](filter-works.md#has\_ngrams)
* [`has_references`](filter-works.md#has\_references)
* [`is_retracted`](work-object/#is\_retracted)
* [`is_paratext`](work-object/#is\_paratext)
* [`journal`](filter-works.md#journal)
* [`language`](work-object/#language)
* [`locations.is_accepted`](work-object/#locations)
* [`locations.is_published`](work-object/#locations)
* [`locations.source.host_institutions_lineage`](filter-works.md#locations.source.host\_institution\_lineage)
* [`locations.source.is_in_doaj`](work-object/#locations)
* [`locations.source.publisher_lineage`](filter-works.md#locations.source.publisher\_lineage)
* [`locations_count`](work-object/#locations\_count)
* [`open_access.any_repository_has_fulltext`](work-object/#open\_access)
* [`open_access.is_oa`](work-object/#is\_oa-1) (alias `is_oa`)
* [`open_access.oa_status`](work-object/#oa\_status) (alias `oa_status`)
* [`primary_location.is_accepted`](work-object/#primary\_location)
* [`primary_location.is_oa`](work-object/#primary\_location)
* [`primary_location.is_published`](work-object/#primary\_location)
* [`primary_location.license`](work-object/#primary\_location)
* [`primary_location.source.has_issn`](work-object/#primary\_location)
* [`primary_location.source.host_organization`](work-object/#primary\_location)
* [`primary_location.source.id`](work-object/#primary\_location)
* [`primary_location.source.is_in_doaj`](work-object/#primary\_location)
* [`primary_location.source.issn`](work-object/#primary\_location)
* [`locations.source.publisher_lineage`](filter-works.md#primary_location.source.publisher\_lineage)
* [`primary_location.source.type`](work-object/#primary\_location)
* [`primary_location.version`](work-object/#primary\_location)
* [`publication_year`](work-object/#publication\_year)
* [`repository`](filter-works.md#repository)
* [`sustainable_development_goals.id`](work-object/README.md#sustainable_development_goals)
* [`type`](work-object/README.md#type)
* [`type_crossref`](work-object/README.md#type_crossref)
