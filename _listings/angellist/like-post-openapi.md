---
swagger: "2.0"
x-collection-name: AngelList
x-complete: 0
info:
  title: AngelList Add Like
  description: Add like.
  termsOfService: https://angel.co/terms
  contact:
    name: AngelList
    url: https://angel.co/api
    email: api@angel.co
  version: v1
host: api.angel.co
basePath: /1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /like:
    post:
      summary: Add Like
      description: Add like.
      operationId: like
      x-api-path-slug: like-post
      parameters:
      - in: query
        name: likable_id
      - in: query
        name: likable_type
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Likes
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---