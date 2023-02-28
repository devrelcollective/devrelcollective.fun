# DevRel Collective Homepage

[![Netlify Status](https://api.netlify.com/api/v1/badges/c9dbbb4a-5ea3-4214-bb24-3d45a83ff2d0/deploy-status)](https://app.netlify.com/sites/devrelcollective/deploys)

The DevRel Collective is a collaborative effort of friendly people who want to empower each other to build a stronger, more inclusive community. For the full schpeel, [read about the project](https://github.com/devrelcollective/getting-started).

## Code of Conduct

DevRel Collective exists to facilitate sharing information, resources, and encouragement among the Developer Relations community. We believe our mission is best served in an environment that is friendly, safe, and accepting; free from intimidation or harassment. You can find our Code of Conduct [here](https://github.com/devrelcollective/getting-started/blob/main/CodeOfConduct.md).

## Contributing

Pull Requests are more than welcome as we coordinate efforts. Here are a few notes to help you along the way.

### Editing The Site

This is a Hugo site, which means that most changes can be made via configuration files.

#### Adding new Admins

If you need to add a new admin's contact to the site, create a new file in the `/data/admins` directory with the new admin's name as the name of the file. So if sally is a new admin, add `sally.yaml` to the `/data/admins` directory with the following fields:

```yaml
name: Sally Admin
twitter: supersally
airport: Timbuk 3
```

Notice that the twitter entry is *just* their username, no `@` or URL, etc.

To remove an admin, simply delete the corresponding file from the `/data/admins` directory.

#### Adding new Resources

If you wish to add a new link to the `Resources` page, you can edit the files in `/data/resources/` directory:

```yaml
category: "Foo and Bar"
links:
  - link: "https://your.link.to.add"
    value: "The text you want the link to display"
```

If this is a new category you're adding, add a new file called `bar.yaml` with the above structure. The `category` field will become the sub-heading, and all the `link:value` pairs will be the links and their linked-text values.

#### Adding new job listing resources

For the Jobs listing page, add to (or delete lines from) `/data/jobs/jobs.yaml`

## Credits

We rock a [MIT License](https://opensource.org/licenses/MIT). The Hugo theme is Avocado, which is based on [Dimension](https://github.com/your-identity/hugo-theme-dimension/). [David Simmons](https://github.com/davidgs) made the site.
