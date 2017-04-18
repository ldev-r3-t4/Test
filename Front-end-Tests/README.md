## Description of front-end server tests
The [front-end server](https://github.com/ldev-r3-t4/frontend-server) is responsible for handling the management of messages for our project.
For the sake of this document messages will be known as posts. Posts are stored in channels. A channel can contain as many posts as possible.

The testing for the front-end server is done through [Newman](https://github.com/postmanlabs/newman). Newman is a command-line tool for the popular [Postman application](https://www.getpostman.com/).  
The tests perform the following actions:
- Creating a new channel.
- Getting a channel.
- Creating a new post.
- Getting a post.
- Updating a post.
- Deleting a post.
- Deleting a channel.

These tests cover the main functionally of the API.
As the API continues to develop more tests will need to be created.

All the tests are containerized in a docker image.
Running the docker image displays the results of the tests.
Instructions for running the image are located below.
## The following commands run the tests for the front-end server portion.
**Note:** Docker must be installed

```sh
docker pull mattg13/round3team4-frontend-server-tests:1.0
```
```sh
docker run mattg13/round3team4-frontend-server-tests:1.0
```  
