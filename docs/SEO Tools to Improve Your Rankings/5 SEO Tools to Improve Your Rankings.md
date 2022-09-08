---
sidebar_position: 1
---

# 5 SEO Tools to Improve Your Rankings

Any niche marketer worth his/her salt will tell you that search engine optimization (SEO) is hard work and youíll need to play the long game. Trying to win at SEO without tools is achievableÖ but extremely arduous.
The right tools will save you a ton of time and be able to dig out data that would take you ages to compile and collate. Considering that things online change rapidly, by the time youíre done compiling your data, it might be outdated.
So it goes without saying that you need a couple of the tools to compete with the big boys. Letís look at what you should getÖ and why you need to get them.

1. SEMRush

Release a version 1.0 of your project:

```bash
npm run docusaurus docs:version 1.0
```

The `docs` folder is copied into `versioned_docs/version-1.0` and `versions.json` is created.

Your docs now have 2 versions:

- `1.0` at `http://localhost:3000/docs/` for the version 1.0 docs
- `current` at `http://localhost:3000/docs/next/` for the **upcoming, unreleased docs**

## Add a Version Dropdown

To navigate seamlessly across versions, add a version dropdown.

Modify the `docusaurus.config.js` file:

```js title="docusaurus.config.js"
module.exports = {
  themeConfig: {
    navbar: {
      items: [
        // highlight-start
        {
          type: 'docsVersionDropdown',
        },
        // highlight-end
      ],
    },
  },
};
```

The docs version dropdown appears in your navbar:

![Docs Version Dropdown](./img/docsVersionDropdown.png)

## Update an existing version

It is possible to edit versioned docs in their respective folder:

- `versioned_docs/version-1.0/hello.md` updates `http://localhost:3000/docs/hello`
- `docs/hello.md` updates `http://localhost:3000/docs/next/hello`
