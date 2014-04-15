Comic Site API
==============

There are currently api endpoints for listing all comics a user has
access to, as well as editing certain properties of those comics. Check
back here for info about changing endpoints.

The api is authenticated with username and password (for now).

Endpoints:

* https://www.inkpebble.com/comic/api/list/ - gets a list of all comics the user can access
* https://www.inkpebble.com/comic/api/{comic_id} - gets details about the specified comic, or allows users to PUT new info into the comic.

Examples:
::
    curl https://www.inkpebble.com/comic/api/list/ -u {username}:{password}

    curl https://www.inkpebble.com/comic/api/1/ -u {username}:{password}

    curl -X PUT https://www.inkpebble.com/comic/api/1/ -u {username}:{password} -d '{"alt_text":"Testing the api"}'

Eventually, these endpoints will probably change, and grow. If you want 
more features, ping Philip.