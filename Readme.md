# Venture Club - Server

This repository is a [json-server](https://github.com/MaelOE/crowdfunding-server) created to feed data into the React Application below.

#### [Client Repo here](https://github.com/MaelOE/crowdfunding-client)

# Server Structure

## Collections

### startups

```javascript
{
  id,
    name,
    description,
    amountRaised,
    sectorId,
    contact,
    firstImage,
    secondImage,
    thirdImage,
    likes;
}
```

### sectors

```javascript
{
  id,
  name,
  slug,
}
```

## Used API Endpoints in the App

| HTTP Method | URL             | Request Body                                          | Description                                   |
| ----------- | --------------- | ----------------------------------------------------- | --------------------------------------------- |
| GET         | `/startups`     |                                                       | Sends all startups                            |
| POST        | `/startups`     | {name, description, amountRaised, sectorId, contact}  | Creates a new startup                         |
| GET         | `/startups/:id` |                                                       | Sends all details of a specific startup       |
| PUT         | `/startups/:id` | {name, description, amountRaised, sectorId, contact}  | Edits a startup object                        |
| DELETE      | `/startups/:id` |                                                       | Deletes a startup object                      |
| PATCH       | `/startups/:id` | {likes} or {firstImage, secondImage, thirdImage, ...} | Updates part of a startup (likes, images etc) |
| GET         | `/sectors`      |                                                       | Sends all sectors                             |
| GET         | `/sectors/:id`  |                                                       | Sends details of a specific sector            |

## Links

### Collaborators

[MaelOE](https://github.com/MaelOE)

### Project

[Repository Link Client](https://github.com/MaelOE/crowdfunding-client)

[Repository Link Server](https://github.com/MaelOE/crowdfunding-server)

[Deploy Link](https://crowdfunding-server-32r5.onrender.com)

### Slides

[Slides Link](https://gamma.app/docs/Venture-Club-usll4gc2jo1stq3)
