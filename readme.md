# Fullstack Fizzbuzz

[Fizzbuzz](http://en.wikipedia.org/wiki/Fizz_buzz) meet the internet. For this interview question, you'll be proving yourself as a full stack developer. Read below to continue.


## Getting Started / Rules

The following challenge can be done in ruby or python, using any framework you would like.
You're welcome to use jquery for the frontend work to simplify the AJAX calls.


## The challenge

Write a series of endpoints to show your mastery of getting data from a database to a web browser and back.
The theme of this drill will be a todo list (single list, no need to handle a list of lists).

1. The first endpoint we'll need is for the default (root/index) action.
This route should render out the initial page (a list of items.) In addition, this page should contain a form with a
textarea that when submitted sends a JSON request to the server to create a new item.

2. The next endpoint we'll need is one to accept a JSON request and if given a valid todo item, insert it into the db. If inserted, the endpoint should return a created HTTP status code and the json representation of the newly created record(include the ID, text, and associated timestamps). If it's not able to delete an item, it should send back the appropriate status code.

3. Next, create an endpoint that we can use to delete a todo item. Also, add a delete button (and functionality) to the page.  If deleted, return a no content status code. If unsuccessful with deleting, return a status code that reflects that.

4. Next, create an endpoint we can poll to get a list of items in JSON (To test, open a second browser window. Create a couple todo items. They should appear in the first browser without having to refresh). Add functionality to the page to poll the server every 5 seconds and refresh the list of items on the page without refreshing the entire page.
