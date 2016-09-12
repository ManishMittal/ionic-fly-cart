# ionic-fly-cart
Ionic Fly Cart is an IONIC framework animated plugin based on SASS for fly cart effect.

## Features
* Fly the product image to cart container after add to cart.
* Dynamic position for cart container.
* Manage the click events of cart container.

## Scrrens
![Alt ion-circular-menu](/screens/screen_01.jpg)
![Alt ion-circular-menu](/screens/screen_02.gif)

## Usage

[Download](http://www.opensourcetechnologies.com/product/ionic-fly-cart) the files .

If you haven’t set up sass the set it using `ionic setup sass` .

Include `speed-dial.scss` in your ionic.app.scss:
`@import "where-you-put-folder/ionic-fly-cart/css/fly";`

Include `fly.js` in your index.html:
`<script type="text/javascript" src="where-you-put-folder/ionic-fly-cart/js/fly.js"></script>`

Add the module `ionic-fly-cart` to your application dependencies in your `app.js`:
`angular.module('starter', ['ionic', 'ionic-speed-dial'])`

And you're ready to go.

## Directives
There are two directives which are used in this template .

### add-to-cart-fly-btn
E.g. <add-to-cart-fly-btn>Add to cart</add-to-cart-fly-btn>
By clicking on this you can fly the image element of its parent .

### add-to-cart-fly-container
The cart container to which the image will fly .
E.g. `<add-to-cart-fly-container top="" right="" funhandler="cartClick();"></add-to-cart-fly-container>` 
You can dynamically set the position by passing top and right value of directive.
Also you can handle the container click event in your controller by defining `cartClick` Function. 

**Example of template object and event handler of cart in controller :**
```javascript
$scope.products = [
    { title: 'Samsung G5', id: 1, price:100, img:"img/products/1.jpg"},
    { title: 'Dell Series', id: 2, price:200, img:"img/products/2.jpg"},
    { title: 'Kelvinator', id: 3, price:300, img:"img/products/3.jpg"},
    { title: 'Whirlpool', id: 4, price:400, img:"img/products/4.jpg"},
    { title: 'HP Pavilion', id: 5, price:500, img:"img/products/5.jpg"},
    { title: 'Accer 100', id: 6, price:600, img:"img/products/6.jpg"},
    { title: 'LG 1115', id: 7, price:700, img:"img/products/7.jpg"}
];
$scope.cartClick=function(){
  console.log("Cart Click Event")	;  
}
```

Feel Free To Contact Us at [sales@opensourcetechnologies.com](mailto:sales@opensourcetechnologies.com?Subject=Ionic%20Fly%20Cart%20plugin)
