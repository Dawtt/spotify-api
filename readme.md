Code based on walkthrough at:

https://github.com/jonnyk20/spotify-node-react-starter-kit

## Usage Notes
Client & server each have separate readme files with more build details.

###Running the application
Run the servers then go to localhost:3000

- Be aware there is a backend & frontend node server.
    - dependencies for each must be installed.
    - the javascript must be compiled / built into other style javascript for each. (server side is done actually?)
    - each server must be started for the application to work.
    - `localhost:3000` frontend UI / webapp address
    - `localhost:8888` backend address
- I put some scripts in each `package.json`. If you navigate to them in intellij, you can click the play button near the file line where code is displayed, then they should be saved on the top toolbar clickdown box to be easily selected and then ran.
    - /authserver/package.json
        - `installserverstuff`
        - `startserver`
    - /client/src/package.json
        - `installclientstuff`
        - `buildclient`
        - `startclient`
 1. Edit `/auth-server/authorization_code/app.js`. Set the secret variables there at the top of the file.
 1. Run all 5 of those scripts 
 1. Open `localhost:3000`, don't click anything yet
 1. Open spotify on same browser in different tab
 1. Log into spotify with your personal spotify account. (create one if needed.
 1. Go to spotify webplayer `https://open.spotify.com/`, play any arbitrary song
 1. On `localhost:3000`, click login to spotify. it will tak you to `localhost:8888` (the backend web server), with a prettier "login to spotify" button. Click that, it should take you to the real spotify login access request for the application.
 1. After logging in and returning to `localhost:3000`, with music playing, click the `check now playing` button. It should display the song you are listening to. If you click it again when the song is different it should update correctly as well.
    