swagger: "2.0"
x-collection-name: Meetup
x-complete: 1
info:
  title: Meetup
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /2/event_comment_likes:
    get:
      summary: Comment Likes
      description: Api for listing likes of a given event comment
      operationId: events
      x-api-path-slug: 2event-comment-likes-get
      parameters:
      - in: query
        name: comment_id
        description: Return likes for a given comment_id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Comments
  /:urlname/events/:event_id/comments/:comment_id/likes:
    get:
      summary: Event Comment and Reply Likes
      description: Returns lists of likes for an event comment or reply
      operationId: comments
      x-api-path-slug: urlnameeventsevent-idcommentscomment-idlikes-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Comments