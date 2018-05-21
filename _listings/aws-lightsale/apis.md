---
name: AWS Lightsale
x-slug: aws-lightsale
description: Amazon Lightsail is the easiest way to get started with AWS for developers
  who just need virtual private servers. Lightsail includes everything you need to
  launch your project quickly - a virtual machine, SSD-based storage, data transfer,
  DNS management, and a static IP - for a low, predictable price. You manage those
  Lightsail servers through the Lightsail console or by using the API or command-line
  interface (CLI).
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
x-kinRank: "10"
x-alexaRank: ""
tags: Regions
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/regions/master/_listings/aws-lightsale/apis.md
specificationVersion: "0.14"
apis:
- name: Amazon Lightsale API Get Regions
  x-api-slug: amazon-lightsale-api
  description: Returns a list of all valid regions for Amazon Lightsail.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: ://///?Action=GetRegions
  tags: Regions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/regions/master/_listings/aws-lightsale/actiongetregions-get-openapi.md
- name: Amazon Lightsale API
  x-api-slug: amazon-lightsale-api
  description: Amazon Lightsail is the easiest way to get started with AWS for developers
    who just need virtual private servers. Lightsail includes everything you need
    to launch your project quickly - a virtual machine, SSD-based storage, data transfer,
    DNS management, and a static IP - for a low, predictable price. You manage those
    Lightsail servers through the Lightsail console or by using the API or command-line
    interface (CLI).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: :///
  tags: Regions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/regions/master/_listings/aws-lightsale/openapi.md
x-common:
- type: x-documentation
  url: https://docs.aws.amazon.com/lightsail/2016-11-28/api-reference/Welcome.html?fid=6DDA37DF97F08F8B-23761D4A79F7B1E
- type: x-pricing
  url: https://amazonlightsail.com/pricing/
- type: x-website
  url: https://amazonlightsail.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---