## Shopify themekit playground

Starter: [https://shopify.github.io/themekit/commands/#using-environments](https://shopify.github.io/themekit)

Tutorial: [https://www.shopify.com/partners/blog/95401862-3-simple-steps-for-setting-up-a-local-shopify-theme-development-environment](https://www.shopify.com/partners/blog/95401862-3-simple-steps-for-setting-up-a-local-shopify-theme-development-environment)

## Get started

- Create Shopify Private App and config permission correctly by following the [starter instruction](https://shopify.github.io/themekit)

- Install `theme-kit`
  - MacOS:
    ```
    brew tap shopify/shopify
    brew install themekit
    ```
  - Window:
    ```
    choco install themekit
    ```

- Use starter code by:
  - Create a new theme
    ```
    theme new --password=[your-password] --store=[your-store.myshopify.com] --name=[theme name]
    ```

  - Or configure an existing theme.
    ```
    theme get -p=[your-password] -s=[you-store.myshopify.com] -t=[your-theme-id]
    ```

    To get all theme's Ids:
    ```
    theme get --list -p=[your-password] -s=[you-store.myshopify.com]
    ```




- Start the developement server
  ```
  theme watch
  ```

## More Refs

- [Liquid cheatsheet](http://cheat.markdunkley.com/)
