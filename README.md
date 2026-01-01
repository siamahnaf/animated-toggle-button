<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/siamahnaf/assets-kit/main/logo/logo-white.png">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/siamahnaf/assets-kit/main/logo/logo-black.png">
  <img alt="Siam Ahnaf" src="https://raw.githubusercontent.com/siamahnaf/assets-kit/main/logo/logo-black.png" height="auto" width="240">
</picture>

<div align="center">
  <h1>React Animated Toggle Button</h1>
</div>

> This is a fork of <a href="https://www.npmjs.com/package/react-toggle-dark-mode?activeTab=readme" target="_blank">react-toggle-dark-mode</a> fixing installation warning issues

![Interactive sun and moon transition](./demo.gif)

## Installation

```shell
npm i animated-toggle-button
```

or with Yarn:

```shell
yarn add animated-toggle-button
```

## Usage

```jsx
import { DarkModeSwitch } from 'animated-toggle-button';

const App = () => {
  const [isDarkMode, setDarkMode] = React.useState(false);

  const toggleDarkMode = (checked: boolean) => {
    setDarkMode(checked);
  };

  return (
    <DarkModeSwitch
      style={{ marginBottom: '2rem' }}
      checked={isDarkMode}
      onChange={toggleDarkMode}
      size={120}
    />
  );
};
```

## API

### DarkModeSwitch

#### Props

| Name                | Type                         | Default Value                   | Description                               |
| ------------------- | ---------------------------- | ------------------------------- | ----------------------------------------- |
| onChange            | \(checked: boolean\) => void |                                 | Event that triggers when icon is clicked. |
| checked             | boolean                      | false                           | Current icon state.                       |
| style               | Object                       |                                 | CSS properties object.                    |
| size                | number                       | 24                              | SVG size.                                 |
| animationProperties | Object                       | defaultProperties \(see below\) | Override default animation properties.    |
| moonColor           | string                       | white                           | Color of the moon.                        |
| sunColor            | string                       | black                           | Color of the sun.                         |

### Default Animation Properties

```javascript
const defaultProperties = {
  dark: {
    circle: {
      r: 9,
    },
    mask: {
      cx: '50%',
      cy: '23%',
    },
    svg: {
      transform: 'rotate(40deg)',
    },
    lines: {
      opacity: 0,
    },
  },
  light: {
    circle: {
      r: 5,
    },
    mask: {
      cx: '100%',
      cy: '0%',
    },
    svg: {
      transform: 'rotate(90deg)',
    },
    lines: {
      opacity: 1,
    },
  },
  springConfig: { mass: 4, tension: 250, friction: 35 },
};
```

## Show your support

Give a ⭐️ if this project helped you!

## Connect with me
<div style="display: flex; align-items: center; gap: 3px;">
<a href="https://wa.me/8801611994403"><img src="https://raw.githubusercontent.com/siamahnaf/assets-kit/main/icons/whatsapp.png" width="40" height="40"></a>
<a href="https://siamahnaf.com/" style="margin-right: 8px"><img src="https://raw.githubusercontent.com/siamahnaf/assets-kit/main/icons/web.png" width="40" height="40"></a>
<a href="https://www.linkedin.com/in/siamahnaf/" style="margin-right: 8px"><img src="https://raw.githubusercontent.com/siamahnaf/assets-kit/main/icons/linkedin.png" width="40" height="40"></a>
<a href="https://x.com/siamahnaf198" style="margin-right: 8px"><img src="https://raw.githubusercontent.com/siamahnaf/assets-kit/main/icons/x.png" width="40" height="40"></a>
<a href="https://www.facebook.com/siamahnaf198/" style="margin-right: 8px"><img src="https://raw.githubusercontent.com/siamahnaf/assets-kit/main/icons/facebook.png" width="40" height="40"></a>
<a href="https://t.me/siamahnaf198" style="margin-right: 8px"><img src="https://raw.githubusercontent.com/siamahnaf/assets-kit/main/icons/telegram.png" width="40" height="40"></a>
<a href="https://www.npmjs.com/~siamahnaf" style="margin-right: 8px"><img src="https://raw.githubusercontent.com/siamahnaf/assets-kit/main/icons/npm.png" width="40" height="40"></a>
</div>


------------

<p align="center" color="red"><a href="https://www.siamahnaf.com/">www.siamahnaf.com</a></p>