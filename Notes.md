## Turorial notes

#### Sections

- To add new **section**, create a **folder** with exactly name `sections` (then add `your-section.liquid`)

- Sections can be dynamically added to the theme's home page if they have [presets](https://shopify.dev/tutorials/develop-theme-use-sections#presets) defined in their respective `{% schema %}` tags

- `presets` must contains `name` and `category`

- To add a section to home page:
  - add `content_for_index` in `index.liquid`
  - Define the data in `config/settings_data.json`

- Config `settings_schema.json` for general settings of your theme