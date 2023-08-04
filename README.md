# Infor Animations

A small library (starting with the first one) of animations that can be used in Infor applications. The animations are build in [Adobe After Effects](https://www.adobe.com/products/aftereffects/). Because of that they require a player to run called [Lottie](https://github.com/airbnb/lottie-web).

## Running the examples in this repo

Clone the Repo and cd into the cloned folder then start up any web server that can serve the folder as the files must be served from a URL. For example

```sh
python3 -m http.server
```

Then open http://localhost:8000/index.html or http://localhost:8000/tests.html in your favorite browser.

## Online example (stackblitz)


## Running the examples in your code

 - in web components
 - in enterprise

## Other Options

1. (Recommended) Using https://github.com/dotlottie/player-component/tree/master/packages/player-component works with the `.lottie` file, so this is the smallest and highest quality and is the recommended option.
1. Using https://github.com/airbnb/lottie-web with the JSON. Fully open source. Bigger files due to JSON and needs dependencies. Good Quality.
1. Using https://github.com/LottieFiles/lottie-player with the JSON. Fully open source. Bigger files due to JSON and needs dependencies. Good Quality.
1. Convert to gif using https://lottiefiles.com/lottie-to-gif lowest quality, huge file but easy to implement and no plugins needed. Not recommended because of poor quality.

## Os Approvals Needed

https://github.com/dotlottie/player-component/tree/master/packages/player-component 

## List of animations

- {logo-animation (320px)} Shows the Infor logo and animates. This animation could be shown directly after logging in to add a nice visual effect, like a splash screen and be centered in the page.