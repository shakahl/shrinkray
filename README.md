### Shrinkray
Create desktop apps in Javascript. Lightweight alternative to Electron because of only supporting macOS (for now).

*Features*
 - [ ] CLI for converting static website into a macOS app.
 - [x] Tiny App sizes (macOS: < 100K, Windows: N/A)
 - [x] Debuggable (Right-click window, select "Inspect Element")
 - [ ] Fullscreen API
 - [ ] File Read/Write
 - [ ] Menu

#### Example Apps

<table>
    <tr>
        <td>
            <a href="https://github.com/francoislaberge/regulex/releases/download/v1.0.0/regulex.app.zip">
                <img src="http://francoislaberge.com/shrinkray/images/regulex-app.png"/>
            </a>
        </td>
        <td>
            <a href="https://github.com/francoislaberge/mini-paint/releases/download/v1.0.0/mini-paint.app.zip">
                <img style="float:left;" src="http://francoislaberge.com/shrinkray/images/mini-paint-app.png"/>
            </a>
        </td>
    </tr>
    <tr>
        <td>https://github.com/francoislaberge/regulex</td>
        <td>https://github.com/francoislaberge/mini-paint</td>
    </tr>
</table>



#### Installation

```
npm install -g shrinkray
```

#### Usage
The input path must be to a folder that has an index.html in it, everything in the folder
will be copied into the generated app and accessible.

```
shrinkray -i <project>/html -o example.app
```

### Contributing

 1. Required Tools
     - [XCode](https://developer.apple.com/xcode/)
     - [Node/NPM](https://nodejs.org/en/download/)
 2. Clone the project

        git clone git@github.com:francoislaberge/shrinkray.git
        cd shrinkray

 3. Install Dependencies

        npm install

 4. Build App Template

        npm run build:app

 5. Publish to npm

        npm run publish:patch
