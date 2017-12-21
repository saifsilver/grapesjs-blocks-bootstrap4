# GrapesJS Bootstrap v4 Blocks Plugin

<!--<span><a href="https://david-dm.org/z1lk/grapesjs-plugin-boilerplate#info=devDependencies" title="View the status of this project's development dependencies on DavidDM"><img src="https://img.shields.io/david/dev/artf/grapesjs-plugin-boilerplate.svg" alt="Dev Dependency Status" /></a></span>-->

<!--<a rel="nofollow" href="https://app.codesponsor.io/link/nb9nPYf2XqCE1PbgcQj6gf4D/artf/grapesjs-plugin-boilerplate">
  <img alt="Sponsor" width="888" height="68" src="https://app.codesponsor.io/embed/nb9nPYf2XqCE1PbgcQj6gf4D/artf/grapesjs-plugin-boilerplate.svg"/>
</a>-->

## Summary

* Plugin name: `grapesjs-blocks-bootstrap4`
* Components
  * `container`
  * `row`
  * `column`
  * `column_break`
  * `text`
  * `header`
* Blocks
  * `container`
  * `row`
  * `column`
  * `column_break`
  * `text`
  * `header`





## Options

```js
{
  blocks: {
    ...
  }
  labels: {
    ...
  }
  ...
}
```

### Blocks

|Option|Description|Default|
|-|-|-
|`container`|Containers (fixed/fluid)|true|
|`row`|Row|true|
|`column`|Columns of all sizes|true|
|`column_break`|Column-break (`div.w-100`)|true|
|`text`|Default text component with utility traits|true|
|`header`|H1-H6|true|

### Labels

Same keys as blocks, but value is the label for the block.

|Option|Description|Default|
|-|-|-
|`text`||'Text'|
|`header`||'Header'|

etc.

### Other

|Option|Description|Default|
|-|-|-
|`gridDevices`|Add devices based on BS grid breakpoints|true|
|`gridDevicesPanel`|Build a panel in the top-left corner with device buttons (use with editor `showDevices`=`false`)|false|

## Download

<!--* CDN
  * `https://unpkg.com/grapesjs-blocks-bootstrap4`
* NPM
  * `npm i grapesjs-blocks-bootstrap4`-->
* GIT
  * `git clone https://github.com/z1lk/grapesjs-blocks-bootstrap4.git`





## Usage

```html
<link href="https://unpkg.com/grapesjs/dist/css/grapes.min.css" rel="stylesheet"/>
<script src="https://unpkg.com/grapesjs"></script>
<script src="path/to/grapesjs-blocks-bootstrap4.min.js"></script>

<div id="gjs"></div>

<script type="text/javascript">
  var editor = grapesjs.init({
      container : '#gjs',
      ...
      plugins: ['grapesjs-blocks-bootstrap4'],
      pluginsOpts: {
        'grapesjs-blocks-bootstrap4': {
          blocks: {
            // ...
          },
          labels: {
            // ...
          },
          // ...
        }
      },
      canvas: {
        styles: [
          'https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-beta.2/css/bootstrap.min.css'
        ],
        scripts: [
          'https://code.jquery.com/jquery-3.2.1.slim.min.js',
          'https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.3/umd/popper.min.js',
          'https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-beta.2/js/bootstrap.min.js'
        ],
      }
  });
</script>
```





## Development

Clone the repository

```sh
$ git clone https://github.com/z1lk/grapesjs-blocks-bootstrap4.git
$ cd grapesjs-blocks-bootstrap4
```

Install dependencies

```sh
$ npm i
```

The plugin relies on GrapesJS via `peerDependencies` so you have to install it manually (without adding it to package.json)

```sh
$ npm i grapesjs --no-save
```

Start the dev server

```sh
$ npm start
```





## License

BSD 3-Clause
