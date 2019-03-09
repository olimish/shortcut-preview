# Shortcut Preview

A React component to preview iOS Shortcuts.

See a preview of the component on https://xalien95.github.io/shortcut-preview/.

## Usage

```tsx
import React from 'react';
import ShortcutPreview from 'shortcut-preview';

// JSON file containing a Shortcut converted using 'pblist-parser'
import shortcutData from './shortcut-data.json';

export default class App extends React.Component {
  render() {
    return <ShortcutPreview data={shortcutData} />;
  }
}
```

You can optionally add a `debug` property: each action block will then show a **LOG** button to `console.log` the contents stored in its state.

```tsx
export default class App extends React.Component {
  render() {
    return <ShortcutPreview debug data={shortcutData} />;
  }
}
```

### Similar Projects

- [shcuts.app](https://github.com/pNre/shcuts.app)
- [Apple Shortcuts Viewer](https://github.com/BobRazowsky/shortcuts)
