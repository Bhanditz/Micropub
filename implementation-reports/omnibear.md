# Omnibear

Implementation Home Page URL: http://omnibear.com

Source code repo URL(s) (optional): https://github.com/keithjgrant/omnibear
* [x] 100% open source implementation

Programming Language(s): JavaScript

Developer(s): [Keith J. Grant](http://keithjgrant.com)

Answers are:
* [ ] Confirmed via micropub.rocks
* [x] Self-reported

## Discovery
* [x] The client discovers the Micropub endpoint given the profile URL of a user (e.g. the sign-in form asks the user to enter their URL, which is used to find the Micropub endpoint)

## Authentication
* [x] The client sends the access token in the HTTP `Authorization` header.
* [ ] The client sends the access token in the post body for `x-www-form-urlencoded` requests.
* [x] The client requests one or more `scope` values when obtaining user authorization.
 * create

## Syntax
* [ ] Creates posts using `x-www-form-urlencoded` syntax.
* [ ] Creates posts using JSON syntax.
* [ ] Creates posts using `x-www-form-urlencoded` syntax with multiple values of the same property name (e.g. tags).
* [ ] Creates posts using JSON syntax with multiple values of the same property name (e.g. tags).
* [ ] Creates posts using JSON syntax including a nested Microformats2 object.
* [ ] Creates posts including a file by sending the request as `multipart/form-data` to the Micropub endpoint.

Note: Current version creates posts using `multipart/form-data`, though it does not include a file.

## Creating Posts
* [ ] Allows creating posts with a photo referenced by URL rather than uploading the photo as a Multipart request.
* [ ] Allows creating posts with a photo including image alt text.
* [x] Recognizes HTTP 201 and 202 with a `Location` header as a successful response from the Micropub endpoint.
* [ ] Allows the user to specify one or more syndication endpoints from their list of endpoints discovered in the `q=config` or `q=syndicate-to` query.

## Media Endpoint
* [ ] Checks to see if the Micropub endpoint specifies a Media Endpoint, and uploads photos there instead.
* [ ] Uses multipart requests only as a fallback when there is no Media Endpoint specified.

## Updates
* [ ] Supports replacing all values of a property (e.g. replacing the post content).
* [ ] Supports adding a value to a property (e.g. adding a tag).
* [ ] Supports removing a value from a property (e.g. removing a specific tag).
* [ ] Supports removing a property.
* [ ] Recognizes HTTP 200, 201 and 204 as a successful response from the Micropub endpoint.

## Deletes
* [ ] Sends deletion requests using `x-www-form-urlencoded` syntax.
* [ ] Sends deletion requests using JSON syntax.
* [ ] Sends undeletion requests using `x-www-form-urlencoded` syntax.
* [ ] Sends undeletion requests using JSON syntax.

## Querying
* [ ] Queries the Micropub endpoint with `q=config`
 * [ ] Looks in the response for the Media Endpoint
 * [ ] Looks in the response for syndication targets
* [ ] Queries the Micropub endpoint with `q=syndicate-to`
* [ ] Queries the Micropub endpoint for a post's source content without specifying a list of properties
* [ ] Queries the Micropub endpoint for a post's source content looking only for specific properties

## Extensions

Please list any [Micropub extensions](https://indieweb.org/Micropub-extensions) that the client supports.

* `mp-slug`

## Vocabularies

Please list all vocabularies and properties the client supports, if applicable.

* Notes, Articles, Bookmarks, Likes, Reposts (http://microformats.org/wiki/h-entry)
 * content
 * category
 * in-reply-to
 * mp-slug
 * like-of
 * repost-of
