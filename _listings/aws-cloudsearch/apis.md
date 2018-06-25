---
name: AWS CloudSearch
x-slug: aws-cloudsearch
description: Amazon CloudSearch is a managed service in the AWS Cloud that makes it
  simple and cost-effective to set up, manage, and scale a search solution for your
  website or application.Amazon CloudSearch supports 34 languages and popular search
  features such as highlighting, autocomplete, and geospatial search. For more information,
  see Benefits.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonCloudSearch.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Options
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/options/master/_listings/aws-cloudsearch/apis.md
specificationVersion: "0.14"
apis:
- name: AWS CloudSearch Describe Availability Options
  x-api-slug: aws-cloudsearch
  description: Gets the availability options configured for a domain.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonCloudSearch.png
  humanURL: https://aws.amazon.com/cloudsearch/
  baseURL: https://///?Action=DescribeAvailabilityOptions
  tags: Availability Options
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/options/master/_listings/aws-cloudsearch/actiondescribeavailabilityoptions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/options/master/_listings/aws-cloudsearch/actiondescribeavailabilityoptions-get-openapi.md
- name: AWS CloudSearch Update Availability Options
  x-api-slug: aws-cloudsearch
  description: Configures the availability options for a domain.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonCloudSearch.png
  humanURL: https://aws.amazon.com/cloudsearch/
  baseURL: https://///?Action=UpdateAvailabilityOptions
  tags: Availability Options
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/options/master/_listings/aws-cloudsearch/actionupdateavailabilityoptions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/options/master/_listings/aws-cloudsearch/actionupdateavailabilityoptions-get-openapi.md
- name: AWS CloudSearch
  x-api-slug: aws-cloudsearch
  description: Amazon CloudSearch is a managed service in the AWS Cloud that makes
    it simple and cost-effective to set up, manage, and scale a search solution for
    your website or application.Amazon CloudSearch supports 34 languages and popular
    search features such as highlighting, autocomplete, and geospatial search. For
    more information, see Benefits.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonCloudSearch.png
  humanURL: https://aws.amazon.com/cloudsearch/
  baseURL: https:///
  tags: Options
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/options/master/_listings/aws-cloudsearch/openapi.md
x-common:
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/cloudsearch/latest/developerguide/cloudsearch-command-line-tools.html
- type: x-console
  url: https://console.aws.amazon.com/cloudsearch
- type: x-documentation
  url: http://docs.aws.amazon.com/cloudsearch/latest/developerguide/api-ref.html *
    hard to find
- type: x-faq
  url: https://aws.amazon.com/cloudsearch/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/cloudsearch/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/cloudsearch/pricing/
- type: x-testimonials
  url: https://aws.amazon.com/cloudsearch/testimonials/
- type: x-website
  url: https://aws.amazon.com/cloudsearch/
- type: x-whats-new
  url: https://aws.amazon.com/cloudsearch/whats-new/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---