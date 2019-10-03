<p align="center">
  <img src="search_members.svg" alt="Kids First Search Members" width="660px">
</p>

# kf-api-search-member

[![CircleCI](https://circleci.com/gh/kids-first/kf-api-search-members.svg?style=svg)](https://circleci.com/gh/kids-first/kf-api-search-members)

This service requires a REST API query request of the form: 
```
/searchmembers?queryString=mytext&start=0&end=50
```
These environment variables can be used to override default configuration:
- ES_HOST : Elastic Search cluster Host
- ES_PORTS : Elastic Search cluster Port List (ex. : ES_PORTS.0=9200, ES_PORTS.1=9300 )
- JWT_PUBLIC_KEY_URL : URL of the public key used to decrypt JWT token
- APPLICATION_SECRET : secret of the play application 

## Build

To build the application, run the following from the command line in the root directory of the project

```bash
sbt ";clean;assembly"
```

