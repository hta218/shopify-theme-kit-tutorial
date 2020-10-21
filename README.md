## Shopify Themekit Starter Instruction

Starter: [https://shopify.github.io/themekit/commands/#using-environments](https://shopify.github.io/themekit)

Tutorial: [https://www.shopify.com/partners/blog/95401862-3-simple-steps-for-setting-up-a-local-shopify-theme-development-environment](https://www.shopify.com/partners/blog/95401862-3-simple-steps-for-setting-up-a-local-shopify-theme-development-environment)

## Get started

Create **Shopify Private App** and config permission correctly by following the [starter instruction](https://shopify.github.io/themekit/#get-api-access):

1. In the store’s **Shopify admin**, click **Apps**.
2. Near the bottom of the page, click on **Manage private apps**.
3. If you see a notice that ***“Private app development is disabled”***, then click **“Enable private app development”**. (Note: Only the store owner can enable private app development)
4. Click **Create new private app**.
5. In the **App details** section, fill out the app name and your email address.
6. In the **Admin API** section, click **Show inactive Admin API permissions**.
7. Scroll to the **“Themes”** section and select **Read and write** from the dropdown.
8. Click **Save**.
9. Read the private app confirmation dialog, then click **Create app**.

You’ll return to the app detail page. Your new, unique access credentials are visible in the **Admin API** section. Copy the password. You’ll use it in the next step.



## Install `theme-kit`
  - MacOS:
    ```
    brew tap shopify/shopify
    brew install themekit
    ```
  - Window:
    ```
    choco install themekit
    ```

## Use starter code by:
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

## Start the developement server

Use the following command to start the development server
```
theme watch
```

Add `--allow-live` flag to watch directory for changes and update remote theme

```
theme watch --allow-live
```

**Other commands:**

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
