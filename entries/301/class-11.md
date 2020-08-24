# EJS

## CHEATSHEET

### Working with Volumes
`GET`

> request the following URI: `https://www.googleapis.com/books/v1/volumes?q=search+terms`

  - request has single parameter
  - q - Search for volumes that contain this text string. There are special keywords you can specify in the search terms to search in particular fields, such as:
    - `intitle`: Returns results where the text following this keyword is found in the title.
    - `inauthor`: Returns results where the text following this keyword is found in the author.
    `inpublisher`: Returns results where the text following this keyword is found in the publisher.
    `subject`: Returns results where the text following this keyword is listed in the category list of the volume.
    `isbn`: Returns results where the text following this keyword is the ISBN number.
    `lccn`: Returns results where the text following this keyword is the Library of Congress Control Number.
    `oclc`: Returns results where the text following this keyword is the Online Computer Library Center number.

#### Filtering
> You can use the filter parameter to restrict the returned results further by setting it the to one of the following values:

  - `partial` - Returns results where at least parts of the text are previewable.
  - `full` - Only returns results where all of the text is viewable.
  - `free-ebooks` - Only returns results that are free Google eBooks.
  - `paid-ebooks` - Only returns results that are Google eBooks with a price.
  - `ebooks` - Only returns results that are Google eBooks, paid or free. Examples of non-eBooks would be publisher content that is available in limited preview and not for sale, or magazines

#### Pagination
> You can paginate the volumes list by specifying two values in the parameters for the request:

  - `startIndex` - The position in the collection at which to start. The index of the first item is 0.
  - `maxResults` - The maximum number of results to return. The default is 10, and the maximum allowable value is 40.

#### Print Type
>You can use the printType parameter to restrict the returned results to a specific print or publication type by setting it to one of the following values:

  - `all` - Does not restrict by print type (default).
  - `books` - Returns only results that are books.
  - `magazines` - Returns results that are magazines.

#### Projection
> You can use the projection parameter with one of the following values to specify a predefined set of Volume fields to return:

  - `full` - Returns all Volume fields.
  - `lite` - Returns only certain fields. See field descriptions marked with double asterisks in the Volume reference to find out which fields are included.

#### Sorting
> By default, a volumes search request returns `maxResults` results, where `maxResults` is the parameter used in pagination (above), ordered by relevance to search terms.

You can change the ordering by setting the `orderBy` parameter to be one of these values:

  - `relevance` - Returns results in order of the relevance of search terms (this is the default).
  - `newest` - Returns results in order of most recently to least recently published



