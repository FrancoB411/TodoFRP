# TodoFRP – [live demo](http://evancz.github.io/TodoFRP)

This basic todo list demonstrates how FRP and Elm
can make writing traditional web apps easier.
Currently it is quite simple, but that makes it a
nice resource for learning more about making "traditional
webapps" with Elm.

### Build Locally

After installing the Elm compiler, follow these steps:

```bash
git clone https://github.com/evancz/TodoFRP.git
cd TodoFRP/src/
elm --make Todo.elm
```

Then open `build/Todo.html` in your browser.

If you want to be fancier, you can run `elm-server` in the `src/` directory.
Then navigate to [localhost:8000/Todo.elm](http://localhost:8000/Todo.elm).
The project will be recompiled whenever you refresh that page in your browser.

### Project Layout

All of the code for this project lives in the `src/` directory.

* [Model.elm](https://github.com/evancz/TodoFRP/blob/master/src/Model.elm):
  Representation of the todo list application.
* [Update.elm](https://github.com/evancz/TodoFRP/blob/master/src/Update.elm):
  Describes how to update the todo list based on user's actions.
* [Inputs.elm](https://github.com/evancz/TodoFRP/blob/master/src/Inputs.elm):
  Describe the UI input elements and the actions the user's actions.
* [Display.elm](https://github.com/evancz/TodoFRP/blob/master/src/Display.elm):
  How to display our model and inputs on screen.
* [Todo.elm](https://github.com/evancz/TodoFRP/blob/master/src/Todo.elm):
  Bring together the model, update, inputs, and display to create the todo list.
