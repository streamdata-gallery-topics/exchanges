---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite IPOs List Exchanges
  description: Post listexchanges
  version: 1.0.0
host: ipos.xignite.com
basePath: xIPOs.json/XigniteIPOs
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ListExchanges:
    get:
      summary: List Exchanges
      description: Post listexchanges
      operationId: ListExchanges
      x-api-path-slug: listexchanges-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Exchanges
  /ListFutureExchanges:
    get:
      summary: List Future Exchanges
      description: Returns a list of future exchanges
      operationId: ListFutureExchanges
      x-api-path-slug: listfutureexchanges-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Future
      - Exchanges
  /AreExchangesOpen:
    get:
      summary: Are Exchanges Open
      description: Are exchanges open.
      operationId: AreExchangesOpen
      x-api-path-slug: areexchangesopen-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Are
      - Exchanges
      - Open
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