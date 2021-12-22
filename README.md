# Assetz Progression Framework V1

This is an archive of version 1 of the Assetz progression framework, to see the current version visit [this repo](https://github.com/AssetzSMECapital/progression-framework) or [this url](progression.assetz.capital) (correct at time of writing).

View this version [here](https://maweeks.github.io/assetz-progression-framework-v1/).

Site created with `gatsby build --prefix-paths` - [gatsby path prefix](https://www.gatsbyjs.com/docs/how-to/previews-deploys-hosting/path-prefix/)

```js
module.exports = {
  pathPrefix: `/assetz-progression-framework-v1`,
  siteMetadata: {
    title: "Assetz Progression",
  },
  plugins: [
    `gatsby-plugin-styled-components`,
    "gatsby-plugin-flow",
    "gatsby-plugin-eslint",
    {
      resolve: `gatsby-source-filesystem`,
      options: {
        path: `${__dirname}/frameworks`,
        name: "frameworks",
      },
    },
    `gatsby-transformer-remark`,
    `gatsby-transformer-yaml`,
    `gatsby-plugin-react-helmet`,
    "gatsby-transformer-sharp",
    "gatsby-plugin-sharp",
    {
      resolve: `gatsby-plugin-nprogress`,
      options: {
        color: `#2991cc`,
        showSpinner: true,
      },
    },
    {
      resolve: `gatsby-plugin-manifest`,
      options: {
        name: "progression-framework",
        short_name: "progression-framework",
        start_url: "/",
        background_color: "#33276B",
        theme_color: "#33276B",
        display: "minimal-ui",
        icon: "src/images/favicon.svg",
      },
    },
  ],
};
```
