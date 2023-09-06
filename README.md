# Infor Animations

A small library (starting with one) of complex animations that can be used in Infor applications. The animations are built using [Adobe After Effects](https://www.adobe.com/products/aftereffects/). They require a special JS player component to run and a file that is loaded in it with the animations. We recommend using the `lottie` file format and the [lottie player](https://github.com/dotlottie/player-component/tree/master/packages/player-component) plugin.

## List of animations

- `logo-animation (320px)` Shows the Infor logo and animates. This animation would be shown directly after logging in to add a visual effect. Use it on something like a splash screen and centered in the page.

## Running the examples in this repo

Clone the Repo and `cd` into the cloned folder then start up any web server that can serve the folder as the files must be served from a URL for the example to work. 

Example:

```sh
python3 -m http.server
```

Then open http://localhost:8000/index.html or http://localhost:8000/tests.html in your favorite browser.

## Online code example (stackblitz)

https://stackblitz.com/edit/ids-animation

## Running the examples in your code

In web components or angular or enterprise these steps are the same.  

1. Install the player `npm install --save @dotlottie/player-component`
2. Import [lottie player](https://github.com/dotlottie/player-component/tree/master/packages/player-component)

```html
<script src="node_modules/@dotlottie/player-component/dist/dotlottie-player.js"></script>`
```

2. Serve the file `animations/logo/logo-animation.lottie` with your application files to any location
3. Add the following code to your page, correcting the path to the `.lottie` file

```js
<dotlottie-player autoplay loop mode="normal" src="animations/logo/logo-animation.lottie" style="width: 320px">
</dotlottie-player>
```

4. Add any needed css to place the animation
5. Run your page and test

## Online hosted file at lottiefiles.com

https://app.lottiefiles.com/animation/8b5f0d63-468d-4cac-ac6c-2917bad82a34

## Os Approvals (Possibly Needed)

https://github.com/dotlottie/player-component/tree/master/packages/player-component 

## Other Options and Tests

See tests.html

1. (Recommended) Using https://github.com/dotlottie/player-component/tree/master/packages/player-component works with the `.lottie` file, so this is the smallest and highest quality and is the recommended option.
1. Using https://github.com/airbnb/lottie-web with the JSON. Fully open source. Bigger files due to JSON and needs dependencies. Good Quality.
1. Using https://github.com/LottieFiles/lottie-player with the JSON. Fully open source. Bigger files due to JSON and needs dependencies. Good Quality.
1. Convert to gif using https://lottiefiles.com/lottie-to-gif lowest quality, huge file but easy to implement and no plugins needed. Not recommended because of poor quality.
