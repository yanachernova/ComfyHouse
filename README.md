<h1 align="center">Welcome to ComfyHouse 👋</h1>
<p>
  <img alt="Version" src="https://img.shields.io/badge/version-0.1.0-blue.svg?cacheSeconds=2592000" />
</p>

> This is a thin wrapper around the [Contentful Delivery SDK](https://github.com/contentful/contentful.rb) and [Contentful Management SDK](https://github.com/contentful/contentful-management.rb) api client libraries.

It allows you to inherit from `ContentfulModel::Base` and specify the content type id, and optionally, fields to coerce in a specific way.

Note that this library doesn't allow you to save changes to your models back to Contentful. We need to use the Contentful Management API for that. Pull requests welcome!

### 🏠 [Homepage](https://github.com/yanachernova/ComfyHouse)

# What is Contentful? 

[Contentful](https://www.contentful.com) provides a content infrastructure for digital teams to power content in websites, apps, and devices. Unlike a CMS, Contentful was built to integrate with the modern software stack. It offers a central hub for structured content, powerful management and delivery APIs, and a customizable web app that enable developers and content creators to ship digital products faster.

## Table of content

- [Usage](#usage)
- [Install](#install)
- [Author](#author)

## Usage

```javascript
const client = contentful.createClient({
    // This is the space ID. A space is like a project folder in Contentful terms
    space: "your_key",
    // This is the access token for this space. Normally you get both ID and the token in the Contentful web app
    accessToken: "your_key"
});


 let contentful = await client.getEntries({
                content_type: "your_name"
            })
```

## Install

```html
<script src="https://cdn.jsdelivr.net/npm/contentful@latest/dist/contentful.browser.min.js"></script>
```

## Author

👤 **Yana**

* Website: codeme.cl
* Github: [@yanachernova](https://github.com/yanachernova)
* LinkedIn: [@https:\/\/www.linkedin.com\/in\/yana-chernova\/](https://linkedin.com/in/https:\/\/www.linkedin.com\/in\/yana-chernova\/)

## Show your support

Give a ⭐️ if this project helped you!

***
