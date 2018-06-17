---
name: BMC Software
x-slug: bmc-software
description: Transform your digital enterprise with BMC IT solutions. From mainframe
  to cloud to mobile, we???ll help you drive innovation and industrial efficiency.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
x-kinRank: "8"
x-alexaRank: "27308"
tags: Alarms
created: "2018-06-17"
modified: "2018-06-17"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/alarms/master/_listings/bmc-software/apis.md
specificationVersion: "0.14"
apis:
- name: BMC Software API Get All Alarms
  x-api-slug: bmc-software-api
  description: Get all of the Alarms
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/alarms
  tags: Alarms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alarms/master/_listings/bmc-software/v1alarms-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alarms/master/_listings/bmc-software/v1alarms-get-openapi.md
- name: BMC Software API Get Alarm by Id
  x-api-slug: bmc-software-api
  description: Retrieves a single alarm
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/alarm/:alarmId
  tags: Alarms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alarms/master/_listings/bmc-software/v1alarmalarmid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alarms/master/_listings/bmc-software/v1alarmalarmid-get-openapi.md
- name: BMC Software API Get Alarms by Name
  x-api-slug: bmc-software-api
  description: Retrieves alarms by name
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/alarms/search
  tags: Alarms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alarms/master/_listings/bmc-software/v1alarmssearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alarms/master/_listings/bmc-software/v1alarmssearch-get-openapi.md
- name: BMC Software API Create Alarm
  x-api-slug: bmc-software-api
  description: Create an Alarm
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/alarms
  tags: Alarms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alarms/master/_listings/bmc-software/v1alarms-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alarms/master/_listings/bmc-software/v1alarms-post-openapi.md
- name: BMC Software API Update Alarm
  x-api-slug: bmc-software-api
  description: Update an Alarm
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/alarm/:alarmId
  tags: Alarms
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alarms/master/_listings/bmc-software/v1alarmalarmid-put-openapi.md
- name: BMC Software API Delete Alarm
  x-api-slug: bmc-software-api
  description: Deletes an alarm
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/alarm/:alarmId
  tags: Alarms
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alarms/master/_listings/bmc-software/v1alarmalarmid-delete-openapi.md
- name: BMC Software API Create Alarm
  x-api-slug: bmc-software-api
  description: Create an Alarm
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v2/alarms
  tags: Alarms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alarms/master/_listings/bmc-software/v2alarms-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alarms/master/_listings/bmc-software/v2alarms-post-openapi.md
- name: BMC Software API Update Alarm
  x-api-slug: bmc-software-api
  description: Updates an alarm
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v2/alarms/:alarmId
  tags: Alarms
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alarms/master/_listings/bmc-software/v2alarmsalarmid-put-openapi.md
- name: BMC Software API Get All Alarms
  x-api-slug: bmc-software-api
  description: Get all of the Alarms
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v2/alarms
  tags: Alarms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alarms/master/_listings/bmc-software/v2alarms-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alarms/master/_listings/bmc-software/v2alarms-get-openapi.md
- name: BMC Software API Get Alarm by Id
  x-api-slug: bmc-software-api
  description: Retrieves a single alarm
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v2/alarms/:alarmId
  tags: Alarms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alarms/master/_listings/bmc-software/v2alarmsalarmid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alarms/master/_listings/bmc-software/v2alarmsalarmid-get-openapi.md
- name: BMC Software API Delete Alarm
  x-api-slug: bmc-software-api
  description: Deletes an alarm
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v2/alarms/:alarmId
  tags: Alarms
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alarms/master/_listings/bmc-software/v2alarmsalarmid-delete-openapi.md
- name: BMC Software API
  x-api-slug: bmc-software-api
  description: Transform your digital enterprise with BMC IT solutions. From mainframe
    to cloud to mobile, we???ll help you drive innovation and industrial efficiency.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https:///
  tags: Alarms
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alarms/master/_listings/bmc-software/openapi.md
x-common:
- type: x-blog
  url: http://www.bmc.com/blogs
- type: x-blog-rss
  url: http://feeds.feedburner.com/BmcBlogs
- type: x-crunchbase
  url: https://crunchbase.com/organization/bmc
- type: x-documentation
  url: https://docs.bmc.com/docs/dashboard.action
- type: x-email
  url: customer_support@bmc.com
- type: x-email
  url: NA_Accounts_Payable@bmc.com
- type: x-email
  url: Collections_NA@bmc.com
- type: x-email
  url: education@bmc.com
- type: x-email
  url: investor@bmc.com
- type: x-email
  url: global_security@bmc.com
- type: x-email
  url: Compliance_EthicsOffice@bmc.com
- type: x-email
  url: 26Ethics@bmc.com
- type: x-email
  url: Community_Relations@bmc.com
- type: x-github
  url: https://github.com/bmcsoftware
- type: x-twitter
  url: https://twitter.com/bmcsoftware
- type: x-website
  url: http://www.bmc.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---