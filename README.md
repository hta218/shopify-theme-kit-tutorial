## Shopify Themekit Starter Instruction

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

	Add `--allow-live` flag to watch directory for changes and update remote theme
	```
  theme watch --allow-live
  ```

- Download changes from Shopify
	```
	theme download
	```

- Open live theme (store's preview)
	```
	theme open
	```


## More References

- [Liquid Cheat Sheet](http://cheat.markdunkley.com/)
- [Shopify Cheat Sheet](https://www.shopify.com/partners/shopify-cheat-sheet)

## License

Copyright © 2020 - Made by Leo @ [https://leohuynh.dev](https://leohuynh.dev)
