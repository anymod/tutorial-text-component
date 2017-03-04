# Text web component tutorial

*This tutorial takes 5-10 minutes.*

In this tutorial you will use a web component to render text on a webpage. Once the component is in place, you'll be able to edit the text without touching your code.

### [Demo here](http://component-io-tutorials.s3-website-us-east-1.amazonaws.com/tutorial-text-component/dist/)

## Getting Started

There are 2 ways to view the file: by downloading or by cloning this repository.

#### Option A: direct download

Download the code as a .zip file using the above [![Clone or download](https://res.cloudinary.com/component/image/upload/v1484267460/clone_or_download.png)](https://github.com/component-io/tutorial-text-component#) button. Unzip the package and view the web page by opening `index.html` with your browser.

#### Option B: `git clone` and run with node

* In your terminal window, run
```
git clone https://github.com/component-io/tutorial-text-component.git
cd tutorial-text-component
npm install
npm start
```
* Visit `http://localhost:3000` in your browser

## The web page

We have a basic landing page that needs some content to describe the main product.

[![The web page](dist/img/tutorial-1.png)](http://component-io-tutorials.s3-website-us-east-1.amazonaws.com/tutorial-text-component/dist/)

We could simply hard-code a description, but this is a great example of where the marketing team or a client might want to make changes later. So instead, we can use a text component, which will make it easy to change the content later if we want.

Find the text in line 68 of `index.html`

```html
Need some content!
```

and replace it with the following

```html
<component text></component>
```

Also paste the Component IO script on line 263 of `index.html`:

```js
<!-- Component IO script -->
<script project="tutorial" src="https://cdn.component.io/v1"></script>
```

The project called `tutorial` already has some content we can use. If you want to create your own content, you can [sign up for an account](https://component.io/auth) and use your own project instead.

Now when you reload the page, you get the content from the component.

[![The improved web page](dist/img/tutorial-2.png)](http://component-io-tutorials.s3-website-us-east-1.amazonaws.com/tutorial-text-component/dist/)

It's that simple -- your component is working, and you can now edit its content in the Component IO dashboard.

Sign up to create your own component and edit it with the dashboard.

[![Sign up](dist/img/sign-up.png)](https://component.io/auth)

## Extra: behind the scenes

When the Component IO script runs, it changes the component from

```html
<component text></component>
```
to
```html
<div component text>New Age is an app that will help you save time, money, or anything else!</div>
```
And because it's ultimately just HTML, you can style it however you want.

## Other

#### Credit where it's due

This project is based on [Start Bootstrap](http://startbootstrap.com/template-overviews/new-age/), which is based on the [Bootstrap](http://getbootstrap.com/) framework.

#### Bugs and Issues

Have a bug or an issue with this template? [Open a new issue](https://github.com/component-io/tutorial-text-component/issues) here on GitHub.

#### Copyright and License

Copyright 2017 Component IO. Code released under the [MIT](https://github.com/component-io/tutorial-text-component/blob/master/LICENSE) license.
