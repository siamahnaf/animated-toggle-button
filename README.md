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

## Stay in touch

- Author - [Siam Ahnaf](https://www.siamahnaf.com/)
- Website - [https://www.siamahnaf.com/](https://www.siamahnaf.com/)
- Twitter - [https://twitter.com/siamahnaf198](https://twitter.com/siamahnaf198)
- Github - [https://github.com/siamahnaf198](https://github.com/siamahnaf198)