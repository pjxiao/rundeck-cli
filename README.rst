===========
RUNDECK-CLI
===========


Usage::

    $ ./rundeck-cli init
    Endpoint [None]: http://example.com
    Token [None]: rundeckclirundeckclirundeckcli

    $ ./rundeck-cli get-job my-job-id
    > GET /api/1/job/my-job-id?format=yaml HTTP/1.1
    > User-Agent: curl
    > Host: example.com
    > Accept: */*
    > X-Rundeck-Auth-Token: rundeckclirundeckclirundeckcli
    >
    < HTTP/1.1 200 OK
    < Set-Cookie: JSESSIONID=rundeckrundeckrundeckrunde;Path=/
    < Expires: Thu, 01 Jan 1970 00:00:00 GMT
    < Content-Type: text/yaml;charset=UTF-8
    < Transfer-Encoding: chunked
    <
    - id: my-job-id
      project: my-project
      ...
