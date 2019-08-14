# Reel Reviews

Find, rate, review and make a list of your favorite movies.

Come, visit the live [Reel Reviews](https://reelreviews.chrisgruber.com/) website.

You can fiddle around with the React UI project in this [CodeSandbox](https://codesandbox.io/s/github/gruberchris/reel-reviews-ui). Though you will need to fork it and configure it's environement variables yourself to see it work there.

## Technologies Used

- JavaScript and Node 10 LTS
- React with Hooks and Redux
- Mongo and Mongoose
- Docker

### Reel Reviews UI

GitHub: [Reel Reviews UI repository](https://github.com/gruberchris/reel-reviews-ui)
DockerHub: [chrisgruber/reel-reviews-ui](https://hub.docker.com/r/chrisgruber/reel-reviews-ui)

### Reel Reviews API

GitHub: [Reel Reviews API repository](https://github.com/gruberchris/reel-reviews-api)
DockerHub: [chrisgruber/reel-reviews-api](https://hub.docker.com/r/chrisgruber/reel-reviews-api)

## Known Issues/ToDo & What Needs To Be Improved For A Production Deployment

- Missing user authentication and authorization
- Unit and integration tests
- Tighten the CORS security policy between the UI client and it's API
- Implement caching of requests to query for movies
- Performance testing the UI. So far I have made not use of memoization or to do a better job of controlling when React needs to render particular components.
- The database does not enforce unique movies. While the UI won't let you create two identical favorite movies, the API and the database will allow it
- User tracking with Google Analytics or something else like it so I can seee who my audience is and how my website is being used
- Improve the UI styles. Its rather bland React Bootstrap styles right now
- Log error messages to some ELK stack
- Would be nice to make use of the movie plot description, but it's challenging the movie databse provider does not send the plot using their main search query API
- User profiles to allow the user an opportunity to configure the app and link their social network accounts
- Allow users to share their favorite movies and reviews with their social media network
- Implement games in Reel Reviews to allow users to compete with one another in their knowledge of movie trivia
- I am sure there are more than a couple opprtunities to take advantage of more caching and hash tables to keep the favorites list performant as it grows over time
- User input validation on the UI and also validate what the UI is sending the API also
- In short, lots to do and lets of opportunity to make a cool app out of Reel Reviews
