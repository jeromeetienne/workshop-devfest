title: WebGL Workshop 
author:
  name: "Jerome Etienne"
  twitter: "@jerome_etienne"
  url: "http://jetienne.com"
output: index.html

--

# Flying Spaceships 
## A Game in THREE.js
  
--

### Using Yeoman ?

* Optional
* Much Faster with it tho
* and time is limited!

--

### Installing yeoman

```
sudo npm install -g yo
```

### Installing three.js Generator

```
sudo npm install -g generator-threejs-boilerplate
```

--

### Project Directory

#### create it

```
mkdir workshop-devfest
```

#### go in

```
cd workshop-devfest
```

--

### Generate Three.js Boilerplate

```
yo threejs-boilerplate
```

<img src="images/yeoman-threejs-boilerplate.png" style="width: 80%;"/>


--

### Try Three.js Boilerplate

* Just a bunch of static files 

```
make server
```

<img src="images/yeoman-threejs-boilerplate.png" style="width: 80%;"/>

--

### What is threex ?

* ultra light extension system for [three.js](http://mrdoob.github.io/three.js/)
* [threex](http://jeromeetienne.github.io/threex/) on github

--

### threex spaceships

* threex extensions for basic spaceships
* on github: [repo](https://github.com/jeromeetienne/threex.spaceships/) / 
[demo](http://jeromeetienne.github.io/threex.spaceships/examples/basic.html)

<iframe src='http://jeromeetienne.github.io/threex.spaceships/examples/basic.html' width='640px' height='480px'></iframe>

--

### Import threex spaceships

```javascript
bower install threex.spaceships
```

<img src="images/bower-install-threex-spaceships.png" style="width: 100%;"/>


--

### include threex spaceships

* using require.js (optional, only for rapidity)
  * META explain how to include it manually
  * META do that for all included threex
* using bower (optional only for rapidity)
  * META all available on github
  * META so can use zip or git itself, as you wish


--

### threex spaceships with bower

```
bower install threex.spaceships
```

<img src="images/bower-install-threex-spaceships.png" style="width: 100%;"/>

--

### threex.planets

* META Why ? what does it provide for us
  * same for other threex
* META 
  * same for other threex
* META what is it ? from threex page
* META url for repo + demo
* META iframe of earth demo

--

### Meta

* do the code step by steps

1. run boilerplate
1. add the stars
1. add the spaceships
1. where is it ?
1. remove the cube
1. add the moon
1. why is it black ?
1. add the lights
1. ok we got the moon but where is the spaceship ?
1. put the spaceship in the proper place
   * rotate it
   * on the left
1. nice... how to move the ships
1. add threex.keyboardstate
1. add a function in rendering loop
   * what is a rendering loop
1. use keyboard to make it move up and down
1. oh an error... 
1. lets wait until the spaceship is loaded
1. lets use keyboard up/down arrow to make it move
1. duh the spaceship can go out of the screen
1. lets add limits
1. nice... well the moon is kinda static.
1. move the moon
   * another function in the rendering loop
1. make it warp
1. yep too static
1. make a random y for the moon on warp
1. well...  cool but the spaceship and the moon
1. lets have spaceship and moon to collide
   * simple one based on distance
   * no time for a explosion effect
   * lets simply use color


-- 
### Whats next ?

* add sound with web audio api

--

### A textual example

Content can be written in **Markdown!** New lines no longer need two angle brackets.

This will be in a separate paragraph.


--

### A list of things

* Item 1
* Item B
* Item gamma

No need for multiple templates!

--

### Unicode

* 林花謝了春紅 太匆匆
* 胭脂淚 留人醉 幾時重
* Matching Pairs «»‹› “”‘’「」〈〉《》〔〕
* Greek αβγδ εζηθ ικλμ νξοπ ρςτυ φχψω
* currency  ¤ $ ¢ € ₠ £ ¥

--

### A code example

    // cool looking code
    var func = function (arg1) {
        return function (arg2) {
            return "arg1: " + arg1 + "arg2: " + arg2;
        };
    };

    console.log(func(1)(2)); // result is three