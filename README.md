# philips hue spotify connector

This piece of software will match your philips hue lights to the album cover of the current song playing in your spotify account.

# How to get going
* Create a spotify api client at https://beta.developer.spotify.com/dashboard/applications.
	* Make sure to set the correct redirectUri for the service. If you're going default use `http://localhost:3000/`
* Copy the client id and client secre
* Use the script `connectHueBridge.sh` to aquire a brige username or use the web-ui once you started everything.
* Set clientId, clientSecret, bridge username and ip in the docker-compose file or pass the environment variables to the service if you start it directly.
* Start the service and web with `docker-compose -f docker-compose.yml up --build`
* Open your browser and go to http://localhost:3000
* Click `Connect Spotify` to authenticate the service
* Let the light matching begin


# Run on raspberry pi
* Use the docker-compose file located in `compose/arm`
