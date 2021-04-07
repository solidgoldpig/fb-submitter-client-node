# Deprecated/Unsupported! 
This package has been incorporated into its only dependant 
https://github.com/ministryofjustice/fb-submitter

<hr/>

# Form Builder Submitter Client (Node)

Client for making requests to Form Builder platform submitter endpoints

## Requirements

Node

## Installation

`npm install @solidgoldpig/fb-submitter-client-node`

## Usage

### Loading and initialising

```js
// load client
const FBSubmitterClient = require('@solidgoldpig/fb-submitter-client-node')

// initialise client
const submitterClient = new FBSubmitterClient(serviceSecret, serviceToken, submitterUrl, serviceSlug)
```

### Fetching and storing

```js
// get submission status
const status = await submitterClient.getStatus(submissionId)

// submit 
const status = await submitterClient.submit(userId, userToken, submissions)
```

