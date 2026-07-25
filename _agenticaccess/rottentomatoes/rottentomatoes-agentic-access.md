---
acting_count: 0
action_class_counts:
  connected: 18
api_specs:
- filename: rottentomatoes-detailed-info-api-openapi.yml
  format: yaml
  label: Rotten Tomatoes Detailed Info API
  slug: rottentomatoes-detailed-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rottentomatoes/refs/heads/main/openapi/rottentomatoes-detailed-info-api-openapi.yml
- filename: rottentomatoes-dvd-lists-api-openapi.yml
  format: yaml
  label: Rotten Tomatoes DVD Lists API
  slug: rottentomatoes-dvd-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rottentomatoes/refs/heads/main/openapi/rottentomatoes-dvd-lists-api-openapi.yml
- filename: rottentomatoes-movie-lists-api-openapi.yml
  format: yaml
  label: Rotten Tomatoes Movie Lists API
  slug: rottentomatoes-movie-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rottentomatoes/refs/heads/main/openapi/rottentomatoes-movie-lists-api-openapi.yml
- filename: rottentomatoes-search-api-openapi.yml
  format: yaml
  label: Rotten Tomatoes Search API
  slug: rottentomatoes-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rottentomatoes/refs/heads/main/openapi/rottentomatoes-search-api-openapi.yml
- filename: rottentomatoes-top-level-lists-api-openapi.yml
  format: yaml
  label: Rotten Tomatoes Top Level Lists API
  slug: rottentomatoes-top-level-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rottentomatoes/refs/heads/main/openapi/rottentomatoes-top-level-lists-api-openapi.yml
consequence_counts:
  read: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Rottentomatoes Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'Rotten Tomatoes exposes 18 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Rotten Tomatoes
provider_slug: rottentomatoes
slug: rottentomatoes-agentic-access
source_filename: rottentomatoes-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 18\n  by_consequence:\n    read: 18\n  human_in_the_loop_required: 0\noperations:\n- path: /lists.json\n  method: get\n  operationId: ListsDirectoryTopLevelLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/dvds.json\n  method: get\n  operationId: DVDListsDirectoryTopLevelLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/dvds/current_releases.json\n  method:\
  \ get\n  operationId: CurrentReleaseDVDsDVDLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/dvds/new_releases.json\n  method: get\n  operationId: NewReleaseDVDsDVDLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/dvds/top_rentals.json\n  method: get\n  operationId: TopRentalsDVDLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/dvds/upcoming.json\n  method: get\n  operationId: UpcomingDVDsDVDLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/movies.json\n  method: get\n  operationId: MovieListsDirectoryTopLevelLists\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/movies/box_office.json\n  method: get\n  operationId: BoxOfficeMovieLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/movies/in_theaters.json\n  method: get\n  operationId: InTheatersMovieLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/movies/opening.json\n  method: get\n  operationId: OpeningMoviesMovieLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/movies/upcoming.json\n  method: get\n  operationId: UpcomingMoviesMovieLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /movie_alias.json\n  method: get\n  operationId: MoviesAliasDetailedInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /movies.json\n  method: get\n  operationId: MoviesSearchSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /movies/{id}.json\n  method: get\n  operationId: MoviesInfoDetailedInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /movies/{id}/cast.json\n  method: get\n  operationId: CastInfoDetailedInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /movies/{id}/clips.json\n\
  \  method: get\n  operationId: MovieClipsDetailedInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /movies/{id}/reviews.json\n  method: get\n  operationId: MoviesReviewsDetailedInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /movies/{id}/similar.json\n  method: get\n  operationId: MoviesSimilarDetailedInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rottentomatoes/refs/heads/main/agentic-access/rottentomatoes-agentic-access.yml
summary_line: 18 operations
tags:
- Movies
- Television
- Reviews
- Ratings
- Tomatometer
- Audience Score
- Entertainment
- Media
---
