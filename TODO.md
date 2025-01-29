## Knowledge Base

In this section, I will document some useful information about Sideberry, and the zen Sidebar (that Sidebery is rendered in).

### Useful IDs, attributes, and classes

- `#sidebar-box` - The `#sidebar-box` element is the element containing the sidebar, in this case Sidebery.
- `#sidebar-header` - The `#sidebar-header` element is the element containing the sidebar header, which displays the name of the active sidebar, and the sidebar switcher arrow.
- `#sidebar-switcher-arrow` - The `#sidebar-switcher-arrow` element is the element containing the sidebar switcher arrow. (Important for the bottom header layout)

- `#navigator-toolbox` - The `#navigator-toolbox` element is the element containing the native Zen tab toolbar.
- `#tabbrowser-tabbox` - The `#tabbrowser-tabbox` element is the element containing the active tab.
- `#navigator-toolbox[zen-user-show]` - `zen-user-show` is a boolean attribute on `#navigator-toolbox` that indicates whether the user has toggled the native Zen tab toolbar to be floating in compact mode. [See also](https://github.com/zen-browser/desktop/blob/32c001d06da833a12fab1054486977ed304c9ebb/src/browser/base/zen-components/ZenCompactMode.mjs#L267-L269)
- `#zen-appcontent-navbar-container[zen-user-show]` - `zen-user-show` is a boolean attribute on `#zen-appcontent-navbar-container` that indicates whether the user has toggled the Zen navbar (also: urlbar) to be floating in compact mode. [See also](https://github.com/zen-browser/desktop/blob/32c001d06da833a12fab1054486977ed304c9ebb/src/browser/base/zen-components/ZenCompactMode.mjs#L395-L398)
- `:root[inFullscreen=true]` - `inFullscreen` is an attribute on `:root` that indicates whether the browser is in full-screen mode.

### Useful queries

- `@-moz-document url-prefix("chrome:")` - This query is used to apply styles to the browser chrome (UI) only.
- `@media (-moz-bool-pref: "path.to.pref")` - This query is used to apply styles only when a certain preference is enabled in `about:config`. Note: user settings configured with `preferences.json` are applied to `about:config`.
