# Portfolio

This is a reinforcement

## Iteration 0 - Setup

Clone the repository, and install `express` library.

NB: Don't forget the `package.json`

## Iteration 1 - `app`

Make an express server listening on port 3000

## Iteration 2 - Homepage

Define a `/` route. The route-handler should display `"hey coucou"` into the terminal.

## Iteration 3 - `<h1>`

Now, on that same route, make your server serve a `<h1>` with your name.

## Iteration 4

Now, add a `<img>` with your photo next to the `<h1>`.

Clue: do you remember `express.public`?

## Iteration 5

Make your homepage a `index.hbs` template and add a stylesheet to the homepage.
Make the `body` background `#eee`.

Clue: remember the ideal place for a stylesheet is in the `<head>`

## Iteration 6

Into the homepage, add a hyperlink to a 2nd page `/projects`.

Create that route and serve a new `projects.hbs` template, with a `<h1>My projects</h1>` inside.

## Iteration 7

Make a common `layout` so the 2 pages share the same "page structure".

NB: your 2 pages should now be background grey.

## Iteration 8

Onto your 2nd page, add 4 `<li>`s, each one containing a different `img` representing a project.

NB: Go on unsplash.com to grab some art

## Iteration 9

Pass a array to your `projects.hbs` containing 4 objects, like: `{id: '1234', name: 'Age of Empire', picture: 'https://...'}`

Use `{{#each}}` inside your template to print as many objects as passed into the array.

NB: Choose whatever `id` you want in your 4 objects.

## Iteration 10

Move the array passed in the previous step in a separate `data.json` file.

Import that file into a `json` variable and replace your array with.

## Iteration 11

Onto the PROJECTS page, make the each project's image clickable. It should brings us to `/projects/XXXXXX`, `XXXXXX` being the `id` of the project, eg: `1234`.

Create that new route, and a new `details.hbs` template.

## Iteration 12

In that route, retreive from `json` the object whose `id` matches the `XXXXXX` parameter in the URL.

Pass it to the `details.hbs` template

## Iteration 13

In the `details.hbs` template, print out the `name` and `picture` from the passed object.

