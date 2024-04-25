Paloma Checker
This project is a simple Node.js script that periodically checks the status of a Paloma server and reports its validation status over HTTP.

Prerequisites
Install Node.js (>= v14.17.3)
A running Paloma network node
Set up a .env file with the necessary environment variables:
DISABLE_VOTE_POWER:set to true if you don't want validator voting power to impact validation
START_IN_PAUSED_STATE: set to true if you want the validating flag set to true at startup
PORT: set the server's listening port
Getting Started
Clone the repository: git clone <https://github.com/username/paloma-checker.git>
Navigate to the project's root folder cd paloma-checker
Install the dependencies: npm install
Modify the .env file based on the prerequisites
Start the server: node index.js
The Paloma Checker will report the validating status over HTTP at http://<host>:<port>/. Use the following endpoints to control validating:

/pause: Sets the validating flag to true.
/unpause: Performs the original functionality.
Configuration
Configuration is done through the .env file with the following environment variables:

DISABLE_VOTE_POWER: set to true if you don't want validator voting power to impact validation (default: false)
START_IN_PAUSED_STATE: set to true if you want the validating flag set to true at startup (default: false)
PORT: port for the server to listen on (default: 3000)
