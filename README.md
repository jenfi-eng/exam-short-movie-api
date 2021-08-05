# Movie APIs ETL

A common function that Jenfi does is API querying and saving the data into a data model then providing an output.

## Instructions

1. Use any language, framework are most comfortable with.
1. Read below.
1. **Zip up the test**, email it back (do not create a PR).

## Requirements

1. Query API for list then specific movies
1. Load the data into a database
1. Produce these outputs from DB calls:
    - Actors & Number of movies they've appeared in, descending order, top 10:

      | Actor Name | Number of Movies |
      | ----- | ---- |
      | Awesome Actress | 2 |
      | Actor Dude | 1 |

    - Movie title and Box Office value, descending order, top 10:

      | Movie Title | Box Office |
      | ----- | ---- |
      | Boy Spider | $10,000,000 |
      | Nickel Boy | $2,000,000 |

1. Output should be a JSON array

## Movie Database APIs for Querying

We'll be using 2 APIs.

- List: https://jsonmock.hackerrank.com/api/movies/search/?Title=spiderman

Use the exact query above (no modifications).

The list API has 13 movies across 2 pages. Each movie in the list has a `imdbID` to uniquely identify the movie. Use this to in the next API to query data for the specific API:

- Specific movie: http://www.omdbapi.com/?apikey=`api-key`&i=`imdbID`
- `api-key` is in your email

## Notes

- Don't query omdbapi too often, we only have 1k queries.
- Don't spend >2 hours on this.
