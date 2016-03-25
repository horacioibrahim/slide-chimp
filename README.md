# &lt;slide-chimp&gt;

> Web Component that allows you to pass forward/backward slides using Speech Recognition API.


## Demo

[Check it live!](http://horacioibrahim.github.io/slide-chimp)

## Install

Install the component using [Bower](http://bower.io):

```sh
$ bower install slide-chimp --save
```

Or [download a ZIP](https://github.com/horacioibrahim/slide-chimp/archive/gh-pages.zip)

## Usage

1. Import Web Components polyfill:

    ```html
    <script src="bower_components/webcomponentsjs/webcomponents-lite.min.js"></script>
    ```

2. Import Custom Element:

    ```html
    <link rel="import" href="bower_components/slide-chimp/slide-chimp.html">
    ```

3. Start using it!

    ```html
    <slide-chimp auto forward="next, go, change, forward" backward="back, previous, back one slide"></slide-chimp>
    ```
  
### Options

Attribute   | Options   | Default   | Description
---         | ---       |---        |---  
`auto`      | *boolean* | `false`   | Specifies if the API speech should started when page loads.
`forward`   | *string*  | `undefined`| Specifies the list of the words *separated by comma* to pass slides forward.
`backward`   | *string*  | `undefined`| Specifies the list of the words *separated by comma* to pass slides backward.
`text`   | *string*  | `undefined`| Stores the string of the recognized text.
`language` | *string* | `en_US` | Specifies the language to be reconized. 


### Methods

Method  | Parameters    | Returns   | Description
---     |---            |---        |---
`start()`| None.        |Nothing    | Triggers the voice-elements to be played.
`stop()`| None.        |Nothing    | Triggers the voice-elements to be stoped.

### Events
Event   | Description
---     | ---
`forward`| Triggers when the slide-chimp matchs word(s) defined in `foward` with speech recognition.
`backward`| Triggers when the slide-chimp matchs word(s) defined in `backward` with speech recognition.

## Development

In order to run it locally you'll need to fetch some dependencies and a basic server setup.

1. Install [Bower](http://bower.io/) & [polyserve](https://github.com/PolymerLabs/polyserve/):

    ```sh
    $ [sudo] npm install -g bower polyserve
    ```

2. Install local dependencies:

    ```sh
    $ bower install && npm install
    ```

3. Polyserve:
    ```sh
    $ polyserver
    Starting Polyserve on port 8080
    Files in this directory are available under http://localhost:8080/components/slide-chimp/
    ```

## Contributing 
1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature-or-fix`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature-or-fix`
5. Submit a pull request :P

## History

For detailed changelog, check [Releases](https://github.com/horacioibrahim/slide-chimp/releases).


## License
[MIT License](http://horacioibrahim.mit-license.org)