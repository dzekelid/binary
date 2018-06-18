---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Futures Get Historical Future Chart Custom Binary
  description: Draw a custom historical chart for a future contract.
  version: 1.0.0
host: www.xignite.com
basePath: xFutures.json/XigniteFutures
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  Intraday, Future, , Binary:
    get:
      summary: Get Intraday Future Chart Binary
      description: Get a standard intraday price chart for a future contract in binary
        format.
      operationId: postGetintradayfuturechartbinary
      x-api-path-slug: intraday-future--binary-get
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
      - Intraday
      - Future
      - Chart
      - Binary
  Intraday, Future, , Custom, Binary:
    get:
      summary: Get Intraday Future Chart Custom Binary
      description: Get a custom intraday price chart for a future contract in binary
        format.
      operationId: postGetintradayfuturechartcustombinary
      x-api-path-slug: intraday-future--custom-binary-get
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
      - Intraday
      - Future
      - Chart
      - Custom
      - Binary
  Historical, Future, , Binary:
    get:
      summary: Get Historical Future Chart Binary
      description: Get a standard historical price chart for a future contract in
        binary format.
      operationId: postGethistoricalfuturechartbinary
      x-api-path-slug: historical-future--binary-get
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
      - Historical
      - Future
      - Chart
      - Binary
  Historical, Future, , Custom, Binary:
    get:
      summary: Get Historical Future Chart Custom Binary
      description: Draw a custom historical chart for a future contract.
      operationId: postGethistoricalfuturechartcustombinary
      x-api-path-slug: historical-future--custom-binary-get
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
      - Historical
      - Future
      - Chart
      - Custom
      - Binary
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