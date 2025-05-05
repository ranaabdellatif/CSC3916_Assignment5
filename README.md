# Assignment Five

[<img src="https://run.pstmn.io/button.svg" alt="Run In Postman" style="width: 128px; height: 32px;">](https://god.gw.postman.com/run-collection/41313426-96ea2105-380e-4a8a-8a46-e015f608bc16?action=collection%2Ffork&source=rip_markdown&collection-url=entityId%3D41313426-96ea2105-380e-4a8a-8a46-e015f608bc16%26entityType%3Dcollection%26workspaceId%3D117894c0-5ee8-4657-84a7-a74aa363e899#?env%5Babdellatif_hw4%5D=W3sia2V5IjoiUmFuZG9tX05hbWUiLCJ2YWx1ZSI6IiIsImVuYWJsZWQiOnRydWUsInR5cGUiOiJhbnkiLCJzZXNzaW9uVmFsdWUiOiIiLCJjb21wbGV0ZVNlc3Npb25WYWx1ZSI6IiIsInNlc3Npb25JbmRleCI6MH0seyJrZXkiOiJyYW5kb21fdXNlcm5hbWUiLCJ2YWx1ZSI6IiIsImVuYWJsZWQiOnRydWUsInR5cGUiOiJhbnkiLCJzZXNzaW9uVmFsdWUiOiJyYW5hIiwiY29tcGxldGVTZXNzaW9uVmFsdWUiOiJyYW5hIiwic2Vzc2lvbkluZGV4IjoxfSx7ImtleSI6InJhbmRvbV9wYXNzd29yZCIsInZhbHVlIjoiIiwiZW5hYmxlZCI6dHJ1ZSwidHlwZSI6ImFueSIsInNlc3Npb25WYWx1ZSI6InBhc3N3b3JkIiwiY29tcGxldGVTZXNzaW9uVmFsdWUiOiJwYXNzd29yZCIsInNlc3Npb25JbmRleCI6Mn0seyJrZXkiOiJKV1QiLCJ2YWx1ZSI6IiIsImVuYWJsZWQiOnRydWUsInR5cGUiOiJhbnkiLCJzZXNzaW9uVmFsdWUiOiIiLCJjb21wbGV0ZVNlc3Npb25WYWx1ZSI6IiIsInNlc3Npb25JbmRleCI6M30seyJrZXkiOiJtb3ZpZUlkIiwidmFsdWUiOiIiLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoiZGVmYXVsdCIsInNlc3Npb25WYWx1ZSI6IiIsImNvbXBsZXRlU2Vzc2lvblZhbHVlIjoiIiwic2Vzc2lvbkluZGV4Ijo0fSx7ImtleSI6ImZha2VNb3ZpZUlkIiwidmFsdWUiOiIiLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoiYW55Iiwic2Vzc2lvblZhbHVlIjoiYWFhYWFhYWFhYWFhYWFhYWFhYWFhYWFhIiwiY29tcGxldGVTZXNzaW9uVmFsdWUiOiJhYWFhYWFhYWFhYWFhYWFhYWFhYWFhYWEiLCJzZXNzaW9uSW5kZXgiOjV9XQ==)

## Frontend React App: https://csc3916-react19-jq09.onrender.com
## Frontend Github: https://github.com/ranaabdellatif/CSC3916_REACT19
## Backend Github: https://github.com/ranaabdellatif/CSC3916_Assignment4

## Purpose

The purpose of this assignment is to create a React Single Page App over your developed API.  The interface will allow the users to search for movies, display information about the movie, see stored ratings, and allow the user to enter a rating.

## Pre-Requirements
- Assignment 3 deployed REACT app that supports SignUp and Logon
- Assignment 4 that supports reviews

## Requirements
- Update your API to support storing an image (or image URL) for the movies you have stored.  You will use the image URL in your React application to show the image of movies
    - New Attribute on the movie collection
- For this assignment all your endpoints should be protected by JWT authentication
- Implement the following interfaces
    - User SignUp and User Logon
        - Leverage your User mongoDB collection to store new users of the application
    - Main screen should show the top rated movies (show at least 5)
        - Your GET /movies endpoint should sort by rating (server side)
            - Update your /movies (with reviews=true) endpoint to sort by average rating descending
    - Movie Detail screen, shows the Movie, Image, Actors that were in the movie, aggregated rating for the movie and grid that shows the reviews (username, rating, review)
    - Extra Credit: (7 points) - chapter 25 of (https://www.amazon.com/dp/B0979MGJ5J?_encoding=UTF8&psc=1&ref_=cm_sw_r_cp_ud_dp_M9YGPJNZWB3BK0P59QX3) Movie Search – show results in a grid, accordion or other list control
        - Add Search API (HTTP POST) to the API that can take partial movie names or partial actor names

## Submissions
- User is able to Sign-up (name, username, password)
- User is able to Logon to the application (username, password)
- User is able to see list of movies and select a movie to see the detail screen (top rated movies displayed)
- User is able to enter a review on the detail page (enter a rating and comment) – the logged in user’s username will be associated with the review (as captured from the JSON Web Token)

## Rubic
- -3 Not able to add comments
- -2 Not aggregating rating (average rating)
- -3 if not pointed to correct end point (e.g Hw4 endpoint)
- -5 if you don’t have a react web site deployed 

## Resources
- https://github.com/facebook/create-react-app
- https://github.com/mars/create-react-app-buildpack#user-content-requires

