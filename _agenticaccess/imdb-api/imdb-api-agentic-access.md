---
acting_count: 0
action_class_counts:
  connected: 37
api_specs:
- filename: imdb-api-openapi.yml
  format: yaml
  label: IMDb-API
  slug: imdb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imdb-api/refs/heads/main/openapi/imdb-api-openapi.yml
consequence_counts:
  read: 37
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Imdb Api Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 37
overview: 'IMDb-API exposes 37 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 37 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: IMDb-API
provider_slug: imdb-api
slug: imdb-api-agentic-access
source_filename: imdb-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/imdb-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    connected: 37\n  by_consequence:\n    read: 37\n  human_in_the_loop_required: 0\noperations:\n- path: /{lang}/API/Search/{apiKey}/{expression}\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/SearchMovie/{apiKey}/{expression}\n  method: get\n  operationId: searchMovie\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/SearchSeries/{apiKey}/{expression}\n\
  \  method: get\n  operationId: searchSeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/SearchName/{apiKey}/{expression}\n  method: get\n  operationId: searchName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/SearchEpisode/{apiKey}/{expression}\n  method: get\n  operationId: searchEpisode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/SearchCompany/{apiKey}/{expression}\n  method: get\n  operationId: searchCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/AdvancedSearch/{apiKey}\n  method: get\n  operationId:\
  \ advancedSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/Title/{apiKey}/{id}\n  method: get\n  operationId: getTitle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/FullCast/{apiKey}/{id}\n  method: get\n  operationId: getFullCast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/Posters/{apiKey}/{id}\n  method: get\n  operationId: getPosters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/Images/{apiKey}/{id}\n  method: get\n  operationId: getImages\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/Trailer/{apiKey}/{id}\n  method: get\n  operationId: getTrailer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/YouTubeTrailer/{apiKey}/{id}\n  method: get\n  operationId: getYouTubeTrailer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/Ratings/{apiKey}/{id}\n  method: get\n  operationId: getRatings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/UserRatings/{apiKey}/{id}\n  method: get\n  operationId: getUserRatings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /{lang}/API/SeasonEpisodes/{apiKey}/{id}/{seasonNumber}\n  method: get\n  operationId: getSeasonEpisodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/Wikipedia/{apiKey}/{id}\n  method: get\n  operationId: getWikipedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/ExternalSites/{apiKey}/{id}\n  method: get\n  operationId: getExternalSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/Reviews/{apiKey}/{id}\n  method: get\n  operationId: getReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /{lang}/API/MetacriticReviews/{apiKey}/{id}\n  method: get\n  operationId: getMetacriticReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/IMDbList/{apiKey}/{id}\n  method: get\n  operationId: getIMDbList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/FAQ/{apiKey}/{id}\n  method: get\n  operationId: getFAQ\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/Name/{apiKey}/{id}\n  method: get\n  operationId: getName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/NameAwards/{apiKey}/{id}\n  method: get\n  operationId:\
  \ getNameAwards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/Company/{apiKey}/{id}\n  method: get\n  operationId: getCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/Keyword/{apiKey}/{id}\n  method: get\n  operationId: getKeyword\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/Top250Movies/{apiKey}\n  method: get\n  operationId: getTop250Movies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/Top250TVs/{apiKey}\n  method: get\n  operationId: getTop250TVs\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/MostPopularMovies/{apiKey}\n  method: get\n  operationId: getMostPopularMovies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/MostPopularTVs/{apiKey}\n  method: get\n  operationId: getMostPopularTVs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/InTheaters/{apiKey}\n  method: get\n  operationId: getInTheaters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/ComingSoon/{apiKey}\n  method: get\n  operationId: getComingSoon\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /{lang}/API/BoxOffice/{apiKey}\n  method: get\n  operationId: getBoxOffice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/API/BoxOfficeAllTime/{apiKey}\n  method: get\n  operationId: getBoxOfficeAllTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /API/Usage/{apiKey}\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /API/ResizeImage\n  method: get\n  operationId: resizeImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /API/ResizePoster\n  method: get\n  operationId: resizePoster\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imdb-api/refs/heads/main/agentic-access/imdb-api-agentic-access.yml
summary_line: 37 operations
tags:
- Video
- Movies
- TV
- Entertainment
- Metadata
- Ratings
- Public APIs
---
