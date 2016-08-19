# react-grid-system
A pure JS bootstrap-like responsive grid system for React.

[![npm version](https://badge.fury.io/js/react-grid-system.svg)](https://badge.fury.io/js/react-grid-system)

## Installation

```
npm install react-grid-system --save
```

## Responsive grid components

Three components are provided for creating responsive grids: `Container`, `Row`, and `Col`.

An example on how to use these:

```javascript
<Container>
  <Row>
    <Col xs={12} md={8}>xs=12 md=8</Col>
    <Col xs={6} md={4}>xs=6 md=4</Col>
  </Row>
</Container>
```

## Responsive utilities

Three components are provided for creating responsive grids: `Visible` and `Hidden`.

An example on how to use these:

```javascript
<Visible xs sm><div>Visible on extra small and small</div></Visible>
<Visible md lg><div>Visible on medium and large</div></Visible>
```

## Documentation

Live examples and documentation can be found at the GitHub pages: https://zoover.github.io/react-grid-system/

## React context types

The following child context types can be provided to the grid components, to alter their responsive behavior:

| Context Type      | Default Value      | Description |
| ----------------- | ------------------ | ------------------------------ |
| `phone`           | `false`            | When set to `true`, a default viewport width of 375 pixels will be used, if the viewport width cannot be determined by using the `window` object. This is useful for server-side rendering. |
| `tablet`          | `false`            | When set to `true`, a default viewport width of 768 pixels will be used, if the viewport width cannot be determined by using the `window` object. This is useful for server-side rendering. |
| `breakpoints`     | `[768, 992, 1200]` | The breakpoints (minimum width) of devices in class `sm`, `md`, and `lg`. |
| `containerWidths` | `[750, 970, 1170]` | The container widths in pixels of devices in class `sm`, `md`, and `lg`. |

For more information on using the user-agent to determine server-side whether a device is a phone or tablet, see for example https://github.com/hgoebl/mobile-detect.js.

For more information about context in React, see https://facebook.github.io/react/docs/context.html.
