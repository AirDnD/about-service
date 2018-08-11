
# about-service for Airpnp

> About-service module allows user to view the location of the airbnb hotels on google map and some reviews about the host in general. 
## Related Projects

  - https://github.com/fullstakreaktor/hero-photo-service
  - https://github.com/fullstakreaktor/Review-service
  - https://github.com/fullstakreaktor/about-service
  - https://github.com/fullstakreaktor/kony-proxy

## Table of Contents

1. [Usage](#Usage)
1. [Requirements](#requirements)
1. [Development](#development)

## Usage

> Some usage instructions

## Requirements

- Node 6.13.0
- Mysql 5.7.22 

## Development

### Setting Up 

To create database of mock data
From within root directory:

```sh
mysql -h localhost -u root 
source db/schema.sql
use reservation
source mock-data/mock_data.sql
```


To install dependencies
From within the root directory:

```sh
npm install -g webpack
npm install
npm run build
npm start
```

### API

### To READ host information from database by id

```sh
curl -H "Content-Type: application/json" -X GET -d '{"host_id: 100"}' http://localhost:3003/api/about/hosts/:id
```
### To READ review information from database by id

```sh
curl -H "Content-Type: application/json" -X GET -d '{"review_id: 1234"}' http://localhost:3003/api/about/reviews/:listingid
```

### To READ neighborhood information from database by id

```sh
curl -H "Content-Type: application/json" -X GET -d '{"neighborhood_id: 1234"}' http://localhost:3003/api/about/neighborhood/:listingId
```





