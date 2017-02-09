# Welcome – Here Is How This Shindig Will Go
<img align="left" src="http://i.imgur.com/cyEEJiw.png" width="240px">

By the end of this tutorial you will have built a web app which will allow you to add random memes, upvote and downvote them, all from React. It will look just like the image you see to the right :D

**Best part is, you don't need to install anything!** It doesn't matter what OS you have – all you need is a browser.

We have everything set up for you in a collection of CodePens. If you ever get lost or confused, you can take a look at the code pen with the solution for that step or just use it to go forward and follow along.

Here are the CodePens for **future** reference (keep following along for now): 
- [Step 0: Hello World!](http://codepen.io/noahpresler/pen/JEZdvz?editors=1010#0)
- [Step 1: My First Meme](http://codepen.io/noahpresler/pen/egKNbL?editors=1010)
- [Step 2: The Meme Component](http://codepen.io/noahpresler/pen/dNKYGG?editors=1010#0)
- [Step 3: The Mapping of the Memes](http://codepen.io/noahpresler/pen/YNvyGG?editors=1010#0)
- [Step 4: Upvotes and downvotes](http://codepen.io/noahpresler/pen/NdzbXd?editors=1010)
- [Step 5: Setting state, onclicks](http://codepen.io/noahpresler/pen/OWEbvX?editors=1010)
- [Step 6: Adding New Memes](http://codepen.io/noahpresler/pen/EZRNEd?editors=1010 )
- [Step 7: LifeCycle & Component Did Update](http://codepen.io/noahpresler/pen/QdxGZM?editors=1010)

# Quick Tour of Code Pen
<img align="right" src="http://i.imgur.com/WzcOh9d.png" width="350px">

Open up [Step 0: Hello World!](http://codepen.io/noahpresler/pen/JEZdvz?editors=1010#0) and have a look around.
It should look like the screenshot to the right.

On the left you'll see HTML, and on the right is Javascript – through this whole application you'll actually never change the HTML, we will create this all purely from Javascript.

In the JS side, click the chevron next to the line ```let memes = ....``` to collapse that variable so it takes up less space. It is a list of memes we will use later in the tutorial, but you will never edit it, so keep it collapsed for ease of coding.

Swag, that's the whole setup. Time for step 0! All the CSS is done for you, so just be sure to use our class names :)

# Step 0: Hello World

###Fork the Code Pen! 

Click on fork in the top right of the CodePen UI. This will create your own version of this pen for you to access later! Click on the title "Step 0: Hello World" to rename it. 

When you click run, you'll notice that the bottom portion of the window, the equivalent of a browser, is filled with grey and the words "Hello World". 

Let's go over how this works. 

### App Component

First, checkout our 'App Component'

```
class App extends React.Component {
  render() {
    return (
      <p>Hello World</p>
    );
  }
}
```

Componenets are the core of React. React components let you split the UI into independent, reusable pieces, and think about each piece in isolation. React components can be defined by subclassing ```React.Component``` as you see we do with ```extends React.Component```.

### The Component's Render Function

They key function for this step is the ```render``` function inside. This returns the HTML that will later get posted to the DOM and displayed in your borwser. 

The render function is called whenever the component is initially rendered and whenver state/props change (we will get into this part later!).

### Inserting the App into the DOM

So when does it actually get rendered and displayed to the browser? The very last line:

```
ReactDOM.render(<App />, document.getElementById('app'));
```

This renders the App component into the element with id 'app', the only tag we have for our HTML! 

_fun fact: look at how we tell the render call to render the App componenet. By create React Componenet, **you just defined a custom HTML tag ```<App />```**_

# Step 1: My First Meme

React handles data through the state variable.  Each React component has its own state.  We’ll add a constructor setting the initial state. Lets initialize it to the first element in the variable ```memes```.

```
//constructor just like in java!
  //sets up initial state in this.state = 
  constructor(props) {
    super(props)
    this.state = memes[0];
  }
```

We can now access the data in this component by typing “this.state” followed by the names of the values in the meme variable.  To access the image link, type “this.state.url” and to access the caption, type “this.state.caption”





# Step 2: The Meme Component
# Step 3: The Mapping of the Memes
# Step 4: Upvotes and Downvotes
# Step 5: Setting State & OnClick
# Step 6: Adding New Memes
# Step 7: React LifeCycle & ComponenetDidUpdate
