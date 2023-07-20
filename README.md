# React Twemoji (SVG)

Provides standard Unicode emoji support across all platforms for [ReactJS][react].

This library simply allows to parse a string and wrap emoji characters in a span element with a font such that all emojis are properly displayed.

- RegEx Pattern — <https://github.com/mathiasbynens/emoji-test-regex-pattern>
- Twemoji — <https://www.jsdelivr.com/package/npm/twemoji-colr-font>
- Noto Emoji — <https://fonts.google.com/noto/specimen/Noto+Color+Emoji>

## Installation

```
npm install flipeador/react-twemoji
```

## Example

```js
/* eslint-disable react-refresh/only-export-components */

import React from 'react';
import ReactDOM from 'react-dom/client';
import twemoji from '@flipeador/react-twemoji';

const root = ReactDOM.createRoot(
    document.getElementById('root')
);

const App = () => {
    return (
        <div>
            <p>{ twemoji.parse('👋 Hello  🌐 World!') }</p>
            <p>{ twemoji.parse('Emoji 15.0 (2022): 🫸🫨🫷') }</p>
        </div>
    );
};

root.render(
    <React.StrictMode>
        <App/>
    </React.StrictMode>
);
```

## License

This project is licensed under the **GNU General Public License v3.0**. See the [license file](LICENSE) for details.

<!-- REFERENCE LINKS -->
[react]: https://react.dev
