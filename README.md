# Contentful Editable Table UI Extension

An editable table to handle tabular data as a [Contentful UI Extension](https://www.contentful.com/developers/docs/concepts/uiextensions/).

![figure](https://raw.githubusercontent.com/contentful-developer-relations/ui-editable-table/master/demo.gif "Editable table as Contentful UI Extension demo")

## Note

This is a fork of the original [Contentful Table UI
Extension](https://github.com/contentful-labs/ui-editable-table) from
Contentful Labs. It includes a few changes:
* Merges @dmcb's [Pull Request](https://github.com/contentful-labs/ui-editable-table/pull/2) that adds controls to alter table dimensions.
* Uses the modern [contentful extension CLI](https://github.com/contentful/contentful-cli/tree/master/docs/extension). The [previous one](https://github.com/contentful/contentful-extension-cli) is already deprecated.
* Allows input of the Environment ID via the `CONTENTFUL_ENVIRONMENT`
    environment variable.

## Installation

```sh
git clone git@github.com:ljvmiranda921/ui-editable-table.git
cd ui-editable-table
npm install
```

### Configure

Create a configuration file with your credentials for Contentful.

```sh
cp .env.example .env
```

Open `.env` in a editor of your liking and add your Contentful space ID, and management token. [Learn how to obtain a token](https://www.contentful.com/developers/docs/references/authentication/#getting-an-oauth-token).

Load environment variables

```sh
source .env
```

### Create

```sh
npm run create
```

Create task will register the extension in your space on Contentful.

### Update

```sh
npm run update
```

Update task will upload the extension to your space on Contentful.

## License

Copyright &copy; Contentful Developer Relations

Licensed under the [MIT license](https://github.com/contentful-labs/ui-editable-table/blob/master/LICENSE).
