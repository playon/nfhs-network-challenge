# NFHS Network - Code Challenge

## Project setup
To get started with the challenge, pull the `main` branch to your local environment then run the following:

```
# install project dependencies
npm install

# serve with hot-reload for development at localhost:8080
npm run serve
```
<br>

## Instructions
The following API accepts a GET request and returns JSON that represents upcoming events for a particular state association.

https://challenge.nfhsnetwork.com/v2/search/events/upcoming?card=true&state_association_key=542bc38f95&size=5&start=0

The challenge is to utilize this endpoint to create a mobile-friendly, client application that closely matches the provided UI and does the following:


* Shows a total count of upcoming events.
* Displays a list of the returned events with the following fields:
  * `headline`, `subheadline`, `date`, `icon_path` (as an image), `city`, `state`, and `publisher_short_name`
* Includes a `Load more` button, if there are more events to fetch, that appends to the list on each click. Utilize the `size` and `start` query params for paging.
* Allows filtering by `state_association_key`. If no key is provided, then return all of the upcoming events.

<br>

### User Interface
Use the provided [design file](https://www.figma.com/file/nouZGv6iIBNonDynso5MgV/Untitled?type=design&node-id=0%3A1&t=UeI1IamFDszizWo6-1) and the screenshot below for reference.

![screenshot](/src/assets/mockup.png)

<br>

## Submission
When finished, please upload your code to GitHub or zip it and email it back.
