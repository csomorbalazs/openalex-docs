# Authorship object

The Authorship object represents a single author and her institutional affiliations in the context of a given work. It is only found as part of a `Work` object, in the [`work.authorships`](./#authorships) property.

### `author`

_String:_ An author of this work, as a dehydrated [`Author`](../../authors/author-object.md) object.

```json
author: {
    id: "https://openalex.org/A5085171399",
    display_name: "Juan Pablo Alperin",
    orcid: "https://orcid.org/0000-0002-9344-7439"
}
```

### `author_position`

_String:_ A summarized description of this author's position in the work's author list. Possible values are `first`, `middle`, and `last`.&#x20;

It's not strictly necessary, because author order is already implicitly recorded by the list order of `Authorship` objects; however it's useful in some contexts to have this as a categorical value.

```json
author_position: "first"
```

### `countries`

_List:_ The country or countries for this author.

We determine the countries using a combination of matched institutions and parsing of the raw affiliation strings, so we can have this information for some authors even if we do not have a specific institutional affiliation.

```json
countries: [
    "US"
]
```

### `institutions`

_List:_ The institutional affiliations this author claimed in the context of this work, as [dehydrated `Institution`](../../institutions/institution-object.md#the-dehydratedinstitution-object) objects.

```json
institutions: [
    {
        id: "https://openalex.org/I18014758",
        display_name: "Simon Fraser University",
        ror: "https://ror.org/0213rcc28",
        country_code: "CA",
        type: "education",
        lineage: ["https://openalex.org/I18014758"]
    }
]
```

### `is_corresponding`

_Boolean:_ If `true`, this is a corresponding author for this work.

{% hint style="warning" %}
This is a new feature, and the information may be missing for many works. We are working on this, and coverage will improve soon.
{% endhint %}

### `raw_affiliation_string`

_String:_ This author's affiliation as it originally came to us (on a webpage or in an API), as a raw unformatted string. Multiple affiliations are separated by a semicolon.

```json
raw_affiliation_string: "Canadian Institute for Studies in Publishing, Simon Fraser University,
```

### `raw_author_name`

_String:_ This author's name as it originally came to us (on a webpage or in an API), as a raw unformatted string.

```json
raw_author_name: "Juan Pablo Alperin"
```
