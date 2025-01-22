# Canvas Theme Template

## Component settings

The theme installs a set of theme components by default. The following settings need to be adjusted manually.

- **Category Banners**: plugin outlet -> above-main-container
- **Tag Banners**: plugin outlet -> above-main-container

## Custom properties

The theme uses CSS custom properties (variables) for consistent styling across the application.

### Theme-specific

Custom properties added by the theme.

| Property Name                   | Description                                   | Undeclared Value               |
| ------------------------------- | --------------------------------------------- | ------------------------------ |
| **Layout**                      |
| `--theme-nav-space`             | Vertical spacing for navigation-bar items     | `0.75rem`                      |
| `--theme-content-padding`       | Top and bottom padding for main content       | `1.5rem`                       |
| `--theme-topic-list-padding`    | Top and bottom padding for topic list items   | `0.8em`                        |
| **Base Styles**                 |
| `--theme-background`            | Main background color of the theme            | `var(--secondary)`             |
| `--theme-border`                | Default border style                          | `1px solid var(--primary-500)` |
| `--theme-border-light`          | Lighter border style for subtle separators    | `1px solid var(--primary-200)` |
| **Button Styles**               |
| `--theme-button-padding`        | Default padding for buttons                   | `0.5em 0.65em`                 |
| `--theme-button-pop-padding`    | Padding for prominent buttons                 | `0.5em 0.65em`                 |
| **Header**                      |
| `--theme-header-height`         | Height of the main header                     | `4rem`                         |
| `--theme-header-border`         | Header bottom border style                    | `none`                         |
| `--theme-header-position`       | Header position                               | `sticky`                       |
| `--theme-header-background`     | Header background color\[^1]                  | `var(--header_background)`     |
| **Sidebar**                     |
| `--theme-sidebar-border`        | Sidebar border style                          | `1px solid var(--primary-low)` |
| `--theme-sidebar-scrollbar`     | Sidebar scrollbar width, can be set to `none` | `var(--scrollbarWidth)`        |
| **Panels**                      |
| `--theme-panel-background`      | Panel background color                        | `var(--secondary)`             |
| `--theme-panel-padding`         | Padding for panels                            | `1rem 2rem`                    |
| `--theme-panel-radius`          | Border radius for panels                      | `var(--d-border-radius-large)` |
| `--theme-panel-border`          | Panel border style                            | `none`                         |
| `--theme-panel-shadow`          | Panel shadow effect                           | `var(--shadow-card)`           |
| **Banners**                     |
| `--theme-banner-background`     | Banner background style                       | `var(--secondary)`             |
| `--theme-banner-color`          | Banner text color                             | `var(--primary)`               |
| `--theme-banner-padding`        | Banner padding                                | `1rem 2rem 1.5rem`             |
| `--theme-banner-radius`         | Banner border radius                          | `var(--d-border-radius-large)` |
| `--theme-banner-border`         | Banner border style                           | `none`                         |
| `--theme-banner-shadow`         | Banner shadow effect                          | `var(--shadow-card)`           |
| **Header Search**               |
| `--theme-header-search-border`  | Border style for header search                | `1px solid var(--primary-400)` |
| `--theme-header-search-padding` | Padding for header search                     | `0.5em`                        |

[^1]: Can be set as an alternative to the color scheme value `var(--header_background)` as it won't affect color calculations like `var(--header-primary-low-mid)`

### Discourse Core

You can override any custom properties from Discourse core. Below is a small selection of common properties.

| Property Name                      | Description                                    | Default Value                   |
| ---------------------------------- | ---------------------------------------------- | ------------------------------- |
| **Layout**                         |
| `--d-max-width`                    | Maximum width of the main content area         | `1110px`                        |
| **Border Radius**                  |
| `--d-border-radius`                | Default border radius for elements             | `2px`                           |
| `--d-border-radius-large`          | Larger border radius for bigger elements       | `2px`                           |
| `--d-button-border-radius`         | Border radius for buttons                      | `2px`                           |
| `--d-input-border-radius`          | Border radius for input fields                 | `var(--d-button-border-radius)` |
| `--d-nav-pill-border-radius`       | Border radius for navigation pills             | `var(--d-button-border-radius)` |
| **Header**                         |
| `--shadow-header`                  | Header shadow effect                           | `0 0 0 1px var(--primary-low)`  |
| **Sidebar**                        |
| `--d-sidebar-width`                | Width of the sidebar                           | `17em`                          |
| `--d-sidebar-background`           | Sidebar background color                       | `var(--secondary)`              |
| `--d-sidebar-row-height`           | Height of sidebar rows                         | `2.2em`                         |
| `--d-sidebar-highlight-background` | Background color for highlighted sidebar items | `var(--primary-low)`            |
