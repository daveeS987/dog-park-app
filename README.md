# Dog Park App

An app that allows users to search for dog parks by location and show nearby foodtrucks, groomers, vets, and dog day care.

**https://davees-dogpark-app.herokuapp.com/**

**Contributors**: Davee Sok, Ryan Geddes, Chris Bortel, Michelle Salazar

![Version](https://img.shields.io/badge/version-1.0.0-brightgreen.svg)

## Links and Resources

- [Dog Park App Website](https://davees-dogpark-app.herokuapp.com/)
- [Domain Model](https://lucid.app/lucidchart/invitations/accept/inv_742b8657-d802-49a8-9915-ccb39ffe9817?viewport_loc=-1923%2C-3997%2C12881%2C7387%2CGmqYbyW5DRaf)
- [Trello Project Board](https://trello.com/b/AziNDkvf/dog-parks)
- [Our Team Agreement](https://docs.google.com/document/d/1Y4YqEGetRE68ka0oiSGRjK2Pk6_ijXd8kQBZpq8Xt2s/edit?usp=sharing)

## References

- [Yelp API Reference](https://docs.developer.yelp.com/docs/getting-started)
- [How to use Google API](https://www.youtube.com/watch?v=8NUqDc1bQ84)

## Overview

**User Story:**  
As a dog owner, I want to be able to find a list of dog parks in the seattle area. I’d like to be able to filter these parks by different criteria such as dog size, terrain (i.e. beach, forest) off-leash, and other useful criteria. I also want to be able to find nearby dog-friendly businesses I can take my dogs to on doggy dates after the park! I would also like to be able to save a list of my favorite parks and be able to reference them later.

## Architecture

This application uses an express framework and ejs templating. Park information and ratings are stored in a PostgreSQL database. Superagent is used to make API calls to Yelp and Google Maps API. This application is deployed through Heroku.

## Dependencies and Tools

<img align="left" alt="JavaScript" width="26px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/javascript/javascript.png"/>
<img align="left" alt="Node.js" width="26px" src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.ict.social%2Fimages%2F5728%2Fnodejs_logo.png&f=1&nofb=1"/>
<img align="left" alt="Express.js" width="26px" src="https://expressjs.com/images/express-facebook-share.png"/>
<img align="left" alt="PostgreSQL" width="26px" src="https://cdn.icon-icons.com/icons2/2415/PNG/512/postgresql_original_wordmark_logo_icon_146392.png"/>
<img align="left" alt="EJS" width="26px" src="https://cdn.icon-icons.com/icons2/2107/PNG/512/file_type_ejs_icon_130626.png"/>

</br>
<br>
<pre>
<b>Javascript ➡ NodeJS ➡ ExpressJS ➡ PostgreSQL ➡ EJS ➡ SuperAgent</b>
</pre>

## Getting Started

- Make sure PostgreSQL is installed on your computer
- Clone down this repo
- Install Dependencies: `npm install`
- Go to [yelp.com](https://www.yelp.com/developers/)
  - create a new app
  - grab the API Key
- Go to [developers.google.com](https://developers.google.com/maps/gmp-get-started)
  - get an API key from Google Maps JavaScript API
- Add the following to an .env file in the root of the repository

```
PORT=3000
DATABASE_URL = postgres:localhost:5432/dogpark_app
YELP_API_KEY = << Get from Yelp website >>
GOOGLE_API_KEY = << Get from Google developer console >
```

- Run `nodemon server.js`
