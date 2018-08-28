---
swagger: "2.0"
x-collection-name: LiveChat
x-complete: 0
info:
  title: LiveChat Queue waiting times
  description: Shows the Minimum, Average and Maximum waiting time.
  version: 1.0.0
host: api.livechatinc.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /reports/chats/queued_visitors/waiting_times:
    get:
      summary: Queue waiting times
      description: Shows the Minimum, Average and Maximum waiting time.
      operationId: ReportsChatsQueuedVisitorsWaitingTimesGet
      x-api-path-slug: reportschatsqueued-visitorswaiting-times-get
      parameters:
      - in: query
        name: date_from
      - in: query
        name: group
      - in: header
        name: X-API-Version
      responses:
        200:
          description: OK
      tags:
      - Queue
      - Waiting
      - Times
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