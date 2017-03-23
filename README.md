
# elm-select

 [![Support me on Patreon][badge_patreon]][patreon] [![Buy me a book][badge_amazon]][amazon] [![PayPal][badge_paypal_donate]][paypal-donations] [![Version](https://img.shields.io/npm/v/elm-select.svg)](https://www.npmjs.com/package/elm-select) [![Downloads](https://img.shields.io/npm/dt/elm-select.svg)](https://www.npmjs.com/package/elm-select)

> Select DOM elements and optionally call a function.

## :cloud: Installation

```sh
$ npm i --save elm-select
```


## :clipboard: Example



```js
const elmSelect = require("elm-select");

// Some examples
let myElm = elmSelect("#my-id")[0]
  , myElms = elmSelect(".some-class")
  ;

function foo(elm, some, args) {
    /*
     *  - elm is the current element
     *  ...and other arguments
     * */
}

// Take all the li elements from already selected element (#my-id)
let liElms = elmSelect("ul > li", foo, [2, 3], myElm);
```

## :question: Get Help

There are few ways to get help:

 1. Please [post questions on Stack Overflow](https://stackoverflow.com/questions/ask). You can open issues with questions, as long you add a link to your Stack Overflow question.
 2. For bug reports and feature requests, open issues. :bug:
 3. For direct and quick help from me, you can [use Codementor](https://www.codementor.io/johnnyb). :rocket:


## :memo: Documentation


### `elmSelect(elm, fn, args, parent)`
Select DOM elements and optionally call a function.

#### Params
- **String|Element|NodeList** `elm`: A stringified query selector, an element or a node list.
- **Function** `fn`: If this function is provided, it will be called with the current element and additional arguments passed in `args`.
- **Array** `args`: An array of arguments used in the `fn` function call (default: `[]`).
- **String|Element** `parent`: The parent element where to search the elements (default: `document`). This makes sense only when a query selector is used.

#### Return
- **NodeList** A node list containing the selected elements.



## :yum: How to contribute
Have an idea? Found a bug? See [how to contribute][contributing].


## :sparkling_heart: Support my projects

I open-source almost everything I can, and I try to reply everyone needing help using these projects. Obviously,
this takes time. You can integrate and use these projects in your applications *for free*! You can even change the source code and redistribute (even resell it).

However, if you get some profit from this or just want to encourage me to continue creating stuff, there are few ways you can do it:

 - Starring and sharing the projects you like :rocket:
 - [![PayPal][badge_paypal]][paypal-donations]—You can make one-time donations via PayPal. I'll probably buy a ~~coffee~~ tea. :tea:
 - [![Support me on Patreon][badge_patreon]][patreon]—Set up a recurring monthly donation and you will get interesting news about what I'm doing (things that I don't share with everyone).
 - **Bitcoin**—You can send me bitcoins at this address (or scanning the code below): `1P9BRsmazNQcuyTxEqveUsnf5CERdq35V6`

    ![](https://i.imgur.com/z6OQI95.png)

Thanks! :heart:


## :dizzy: Where is this library used?
If you are using this library in one of your projects, add it in this list. :sparkles:


 - [`crossy`](https://github.com/IonicaBizau/crossy.js)—Modify cross-browser CSS properties with one JavaScript call.
 - [`css-cross-transform`](https://github.com/IonicaBizau/css.cross-transform.js)—Modify CSS transform properties with one JavaScript call.
 - [`donate.js`](https://github.com/IonicaBizau/donate.js)—A JavaScript library for creating a friendly way to send money donations.
 - [`match`](https://github.com/IonicaBizau/match.js#readme)—Simplest way to create match memory games.
 - [`showalicense.com`](https://github.com/IonicaBizau/showalicense.com#readme)—A site to provide an easy way to show licenses and their human-readable explanations.
 - [`timer-app`](https://github.com/IonicaBizau/timer-app#readme)—A simple timer application.
 - [`validate5`](https://github.com/IonicaBizau/validate5#readme)—Form validations made easy.

## :scroll: License

[MIT][license] © [Ionică Bizău][website]

[badge_patreon]: http://ionicabizau.github.io/badges/patreon.svg
[badge_amazon]: http://ionicabizau.github.io/badges/amazon.svg
[badge_paypal]: http://ionicabizau.github.io/badges/paypal.svg
[badge_paypal_donate]: http://ionicabizau.github.io/badges/paypal_donate.svg
[patreon]: https://www.patreon.com/ionicabizau
[amazon]: http://amzn.eu/hRo9sIZ
[paypal-donations]: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=RVXDDLKKLQRJW
[donate-now]: http://i.imgur.com/6cMbHOC.png

[license]: http://showalicense.com/?fullname=Ionic%C4%83%20Biz%C4%83u%20%3Cbizauionica%40gmail.com%3E%20(https%3A%2F%2Fionicabizau.net)&year=2015#license-mit
[website]: https://ionicabizau.net
[contributing]: /CONTRIBUTING.md
[docs]: /DOCUMENTATION.md
