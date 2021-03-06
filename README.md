# Gridsome ButterCMS Starter

* Demo: [https://buttercms-gridsome-starter.netlify.app/](https://buttercms-gridsome-starter.netlify.app/)


### 1. Install/Update Gridsome CLI tool

`npm install --global @gridsome/cli`

### 2. Run from your CLI

`gridsome create my-gridsome-site https://github.com/ButterCMS/gridsome-starter-buttercms`

### 3. Create a ButterCMS account

1. Create a free account on ButterCMS - https://buttercms.com/.
3. Copy and save off your AuthToken from the welcome screen or Profile >> settings (it looks like this: a985f3f782f2005...)
4. Add a second Blog Post to your ButterCMS account by going to Blog Posts, then click the green “Write New Post” button at the top and write and Publish your post.


### 4. In gridsome.config.js, replace the test Auth token (0126997a0f359dffdf0a4200b9c229161c7610ec) with the Auth token from your ButterCMS account

```
module.exports = {
  siteName: 'Gridsome',
  plugins: [{
    use: "gridsome-source-buttercms",
    options: {
      authToken: '0126997a0f359dffdf0a4200b9c229161c7610ec', // Auth token belongs to a test account with test data
      collections: [''],
      pages: '',
      pageTypes: 'customer_case_study'
    }
  }
  ]
}
```

### 4. CD into the project and run it
`cd gridsome-starter-buttercms`
`gridsome develop`

# Learn more

ButterCMS can be used as a [gridsome cms](https://buttercms.com/gridsome-cms/) and [gridsome blog engine](https://buttercms.com/gridsome-blog-engine/). This starter project demonstrates how to use Butter with Gridsome.
