# MERN Lab - Album Collector

For this activity we're going to get a chance to practice taking all the concepts learned today and build out a full stack MERN application. You'll be using React on the frontend, and Express, Node, and Mongo DB on the backend.

Have the app we built out today open and refer back to often as a reference. You'll be building something very similar only this time on your own.

---

## What We'll be Storing

For this activity you're model will be Albums. We'll be storing a collection of your favorite Albums in MongoDB.

For each Album you'll store
- artist (a string)
- releaseDate (a string, you can also expirement with the date type in mongo and mongoose)
- favoriteTrack (a string)
- coverArtUrl (a string with the url for the cover art image)
- listenedTo (a boolean indicating if you've listened to the whole album)

---

## User Specifications

A user will be able to visit the app and
- View a page showing all Albums in the collection
- Click on an Album and view the show page for that particular ablum
- Navigate to a create page where they can enter information to add a new album to the collection.

---

## Set up the Backend
1. Start up your Express server
1. Create the routes in your album controller
  - index
  - show
  - create
1. Set up your Album model with the fields specified above
1. Add the mongoose code in your controllers to
  - send JSON for all Albums in your index route
  - send JSON for one Album by its id in your show route
  - create a new Album for your create route
1. Remember to add cors to your API with the [cors middleware](https://www.npmjs.com/package/cors).This will allow us to hit the API from the React app.
1. Test out your API, either in the browser or with [Postman](https://www.postman.com/downloads/)

---

## Set up the Frontend
1. Add a navigation and React Router to your application
1. Build the Album index page that will make a request to your API to get all of the Albums and display them on the page.
1. Add a link to each Album, so when clicked it will take the user to a show page for that Album.
1. The Album show page show show the details for just a single Album.
1. Add a link in the navigation taking the user to the create Album page.
1. The create Album page should display a form allowing a user to enter information for a new Album to add to their collection.
1. Submitting the form should make a request to the API to add a new Album, and then redirect to the index page to view all Albums.

