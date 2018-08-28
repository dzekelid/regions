---
name: AWS Polly
x-slug: aws-polly
description: Amazon Polly is a service that turns text into lifelike speech. Polly
  lets you create applications that talk, enabling you to build entirely new categories
  of speech-enabled products. Polly is an Amazon AI service that uses advanced deep
  learning technologies to synthesize speech that sounds like a human voice. Polly
  includes 47 lifelike voices spread across 24 languages, so you can select the ideal
  voice and build speech-enabled applications that work in many different countries.Amazon
  Polly delivers the consistently fast response times required to support real-time,
  interactive dialog. You can cache and save Polly&rsquo;s speech audio to replay
  offline or redistribute. And Polly is easy to use. You simply send the text you
  want converted into speech to the Polly API, and Polly immediately returns the audio
  stream to your application so your application can play it directly or store it
  in a standard audio file format, such as MP3.With Polly, you only pay for the number
  of characters you convert to speech, and you can save and replay Polly&rsquo;s generated
  speech. Polly&rsquo;s low cost per character converted, and lack of restrictions
  on storage and reuse of voice output, make it a cost-effective way to enable Text-to-Speech
  everywhere.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-polly.jpg
x-kinRank: "10"
x-alexaRank: "0"
tags: Regions
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/regions/master/_listings/aws-polly/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Polly API - Delete Lexicon
  x-api-slug: actiondeletelexicon-get
  description: Deletes the specified pronunciation lexicon stored in an AWS Region.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-polly.jpg
  humanURL: https://aws.amazon.com/polly/
  baseURL: :///
  tags: Amazon Web Services, Speech, Voice, Stack Network, API Service Provider, API
    Service Provider, API Provider, Texts, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/regions/master/_listings/aws-polly/actiondeletelexicon-get-openapi.md
- name: AWS Polly API - Get Lexicon
  x-api-slug: actiongetlexicon-get
  description: Returns the content of the specified pronunciation lexicon stored in
    an AWS Region.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-polly.jpg
  humanURL: https://aws.amazon.com/polly/
  baseURL: :///
  tags: Amazon Web Services, Speech, Voice, Stack Network, API Service Provider, API
    Service Provider, API Provider, Texts, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/regions/master/_listings/aws-polly/actiongetlexicon-get-openapi.md
- name: AWS Polly API - List Lexicons
  x-api-slug: actionlistlexicons-get
  description: Returns a list of pronunciation lexicons stored in an AWS Region.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-polly.jpg
  humanURL: https://aws.amazon.com/polly/
  baseURL: :///
  tags: Amazon Web Services, Speech, Voice, Stack Network, API Service Provider, API
    Service Provider, API Provider, Texts, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/regions/master/_listings/aws-polly/actionlistlexicons-get-openapi.md
- name: AWS Polly API - Put Lexicon
  x-api-slug: actionputlexicon-get
  description: Stores a pronunciation lexicon in an AWS Region.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-polly.jpg
  humanURL: https://aws.amazon.com/polly/
  baseURL: :///
  tags: Amazon Web Services, Speech, Voice, Stack Network, API Service Provider, API
    Service Provider, API Provider, Texts, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/regions/master/_listings/aws-polly/actionputlexicon-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.pinpoint.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.polly.stack.network
- type: x-authentication
  url: http://docs.aws.amazon.com/polly/latest/dg/authentication-and-access-control.html
- type: x-customers
  url: https://aws.amazon.com/polly/customers/
- type: x-documentation
  url: http://docs.aws.amazon.com/polly/latest/dg/API_Reference.html
- type: x-faq
  url: https://aws.amazon.com/polly/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/polly/getting-started/
- type: x-logging
  url: http://docs.aws.amazon.com/polly/latest/dg/logging-using-cloudtrail.html
- type: x-monitoring
  url: http://docs.aws.amazon.com/polly/latest/dg/cloud-watch.html
- type: x-pricing
  url: https://aws.amazon.com/polly/pricing/
- type: x-website
  url: https://aws.amazon.com/polly/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---