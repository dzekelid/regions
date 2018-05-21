---
name: Etsy
x-slug: etsy
description: Etsy is a website that focuses on handmade and vintage items, as well
  as art and craft supplies. The items include art, photography, clothing, jewelry,
  edibles, quilts, and toys. Etsy is modeled after open craft fairs that give sellers
  personal storefronts where they can list their goods. The company charges users
  a flat listing fee (of 20 cents per items), and takes a commission of 3.5% off all
  items sold. Since its launch in June 2005, the site has continually added new widgets
  and features, and has seen corresponding growth.
image: http://pbs.twimg.com/profile_images/613742962095341568/VGmQvBw8_normal.png
x-kinRank: "9"
x-alexaRank: ""
tags: Regions
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/regions/master/_listings/etsy/apis.md
specificationVersion: "0.14"
apis:
- name: Etsy Get Regions Region
  x-api-slug: etsy
  description: Retrieves a Region by id.
  image: http://pbs.twimg.com/profile_images/613742962095341568/VGmQvBw8_normal.png
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//regions/{region_id}
  tags: Regions,Region
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/regions/master/_listings/etsy/regionsregion-id-get-openapi.md
- name: Etsy Get Regions
  x-api-slug: etsy
  description: Finds all Region.
  image: http://pbs.twimg.com/profile_images/613742962095341568/VGmQvBw8_normal.png
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private//regions
  tags: Regions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/regions/master/_listings/etsy/regions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/regions/master/_listings/etsy/regions-get-openapi.md
- name: Etsy
  x-api-slug: etsy
  description: Etsy is a handmade marketplace. The Etsy API lets developers tap into
    the Etsy community, building their own Etsy-powered applications for the web,
    desktop and mobile devices. Applications built on the API will connect buyers
    with sellers, promote the handmade lifestyle, and support the craftspeople who
    sell on Etsy.
  image: http://pbs.twimg.com/profile_images/613742962095341568/VGmQvBw8_normal.png
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private
  tags: Regions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/regions/master/_listings/etsy/openapi.md
x-common:
- type: x-apijson--authoritative
  url: http://apis.io/apisdef/etsy.json
- type: x-application-gallery
  url: https://www.etsy.com/apps/
- type: x-base
  url: https://openapi.etsy.com/
- type: x-blog
  url: http://www.etsy.com/blog/en/
- type: x-blog-rss
  url: https://blog.etsy.com/en/feed/
- type: x-copyright
  url: https://www.etsy.com/help/article/482/?ref=ftr
- type: x-crunchbase
  url: http://www.crunchbase.com/company/etsy
- type: x-developer
  url: https://www.etsy.com/developers/
- type: x-forum
  url: https://www.etsy.com/developers/discussion
- type: x-github
  url: https://github.com/etsy
- type: x-privacy
  url: https://www.etsy.com/help/article/480/?ref=ftr
- type: x-terms-of-service
  url: https://www.etsy.com/help/article/479/?ref=ftr
- type: x-transparency-report
  url: http://blog.etsy.com/news/files/2015/07/Etsy_TransparencyReport_2014.pdf
- type: x-twitter
  url: https://twitter.com/Etsy
- type: x-website
  url: http://www.etsy.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---