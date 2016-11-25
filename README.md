# Design

## To communicate with live environment
- bash alias to add nodes via curl
- api server running on port 8080
- visualization server running on port 8081
- upon change, saves serialized app

## To build application
- live server being updated
- runs on port 3000
- creates an API ending in /api


## Example: blog
- datastore:
  - content: markdown
  - published: date
- page: create datastore entry
- admin page: list entries, allow delete
- sitemap
- page: show story
- 404 page which lists other blog posts


Notes:
- datastore is pretty much like a rails model
- make an SEO thing with a sitemap.xml automatically
- dont create pages for API endpoints, go for user actions (also allow creating API endpoints)
- the important thing is not being able to zoom into your app, it's being able to zoom out
- views / layers:
 - API view
 - system view
 - errors view
 - performance layer
 - page view (see all the pages)
