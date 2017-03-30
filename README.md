# A React Component that gives you simple, relevant placeholder images

This package integrates with [Unsplash](https://source.unsplash.com/) and gives you a React Component that allows you to add tailored placeholder images anywhere in your project.

Instead of a random image or a grayed out block, you'll get a photo that not only corresponds with your use case, but is also sized perfectly for your needs.

It includes linting with [ESLint](http://eslint.org/) and testing with [Mocha](https://mochajs.org/), [Enzyme](http://airbnb.io/enzyme/) and [JSDOM](https://github.com/tmpvar/jsdom).

## Installation

While inside your project, you can install the package with NPM:

`npm install --save react-quick-image`

Or Yarn:

`yarn add react-quick-image`

## Usage

1. Import the QuickImage Component into your current file.
2. Create a new instance of the component.
3. Use the **width** and **height** props to define the size of the image. *(Defaults to 800x600)*
4. Use the **find** prop to enter a keyword for your desired image. *(Defaults to undefined)*
5. Open up your browser and enjoy a customized placeholder image.

### Examples 
```javascript
 
import React from 'react';
import QuickImage from 'react-quick-image';
 
// Stateless Functional Component
 
const CoverPhoto = (props) => (
  <div>
    <QuickImage width="600" height="400" find="code" />
  </div>
);
 
// ES6 Class Component
 
class ProfilePicture extends React.Component {
  constructor(props) {
    super(props);
  }
  
  render() {
    return (
      <div>
        <QuickImage width="200" height="200" find="cats" />
      </div>
    );
  }
}

``` 
 
 Live Example:
<p data-height="265" data-theme-id="dark" data-slug-hash="WpYdZW" data-default-tab="js,result" data-user="cbeard" data-embed-version="2" data-pen-title="QuickImage React" class="codepen"><a href="http://codepen.io/cbeard/pen/WpYdZW/">QuickImage React</a> (<a href="http://codepen.io/cbeard">@cbeard</a>) on <a href="http://codepen.io">CodePen</a>.</p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>
## Planned Features

- [ ] Create functionality for customizing placeholder images *(i.e. darken, blur, greyscale)*
- [ ] Ability to use to permanent image sources in production, while retaining current functionality

## License

MIT
