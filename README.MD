### Add Bootstrap to your ionic project.

#### Step 1: Install Ionic

Install bootstrap:

`npm install bootstrap`

### Step 2: Add Configs

Edit package.json:

```json{
    ....
    "description": "An Ionic project",
    "config": {
        "ionic_sass": "./sass.config.js" // <- Add This**
    }
}
```

### Step 3: Create sass.config.js

Create new file sass.config.js in home folder

```js
module.exports = {
  includePaths: [
    "node_modules/ionic-angular/themes",
    "node_modules/ionicons/scss",
    "node_modules/ionic-angular/fonts",
    "node_modules/bootstrap/scss",
  ],
};
```

### Step 4: Import Bootstrap

Edit variables.scss

```scss
@import "noto-sans";
......
@import "bootstrap";
```


### test your installation

Add your bootstrap code:
```html
<button type="button" class="btn btn-primary">Primary</button> 
<button type="button" class="btn btn-secondary">Secondary</button> 
<button type="button" class="btn btn-success">Success</button>
```

### Run your app

```sh
run ionic app
ionic serve
```