# Jupyter Bridge

##   For a Technology Literate World
---

<small>*The views expressed in this documentation are the creators own and do not refelect the view of the U.S. Government or Director of National Intelligence.*</small>


**What:** Jupyter Bridge believes that democracy is effective because it works on the premise that good ideas can come from anywhere. 

**Why:** Technologies, such as writing and the printing press have facilitated the sharing of ideas for thousands of years. Code is no different and in many ways it is more effective, as reapplying someone else's idea is much easier. Just as more humans becoming literate facilitated an explosion of knowledge and invention, Jupyter Bridge is intended to help increase technology literacy to allow more people access to coding technology so they can share their ideas.

**How:** Jupyter Bridge uses a multitude of learning theories to: 

1. Allow developers and data scientists to **bridge** the technical gap with users more effectively
2. Allow users to engage technology in a domain of comfort then explore the technology in a scaffolded approach

**Questions, Comments or Concerns?** Contact Us- thomas.d.pike@ni-u.edu or  melissa.c.laduke@ni-u.edu

---
## Organization

Jupyter Bridge is just getting started so take a look at our two analytics a Grade Dashboard and a Pandemic Model 

If you have an analytic you want to contribute please see below. 


## Requirements

- JupyterLab >= 4.0.0

## Install

To install the extension, execute:

```bash
pip install jupyter_bridge
```

## Uninstall

To remove the extension, execute:

```bash
pip uninstall jupyter_bridge
```

## Contributing
### Tool Contribution

1 - Build your tool
2 - Put in an appropriate domain
3 - [Submit a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)

### Development install

Note: You will need NodeJS to build the extension package.

The `jlpm` command is JupyterLab's pinned version of
[yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
`yarn` or `npm` in lieu of `jlpm` below.

```bash
# Clone the repo to your local environment
# Change directory to the jupyter_bridge directory
# Install package in development mode
pip install -e "."
# Link your development version of the extension with JupyterLab
jupyter labextension develop . --overwrite
# Rebuild extension Typescript source after making changes
jlpm build
```

You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.

```bash
# Watch the source directory in one terminal, automatically rebuilding when needed
jlpm watch
# Run JupyterLab in another terminal
jupyter lab
```

With the watch command running, every saved change will immediately be built locally and available in your running JupyterLab. Refresh JupyterLab to load the change in your browser (you may need to wait several seconds for the extension to be rebuilt).

By default, the `jlpm build` command generates the source maps for this extension to make it easier to debug using the browser dev tools. To also generate source maps for the JupyterLab core extensions, you can run the following command:

```bash
jupyter lab build --minimize=False
```

### Development uninstall

```bash
pip uninstall jupyter_bridge
```

In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
folder is located. Then you can remove the symlink named `jupyter_bridge` within that folder.

### Testing the extension

#### Frontend tests

This extension is using [Jest](https://jestjs.io/) for JavaScript code testing.

To execute them, execute:

```sh
jlpm
jlpm test
```

#### Integration tests

This extension uses [Playwright](https://playwright.dev/docs/intro) for the integration tests (aka user level tests).
More precisely, the JupyterLab helper [Galata](https://github.com/jupyterlab/jupyterlab/tree/master/galata) is used to handle testing the extension in JupyterLab.

More information are provided within the [ui-tests](./ui-tests/README.md) README.

### Packaging the extension

See [RELEASE](RELEASE.md)

```{toctree}
---
maxdepth: 0
hidden: true
---
Welcome <self>
Overview <overview>
Grade DashBoard <grade_dashboard/grade_dashboard>
Pandemic Model <pandemic_model/pandemic_model>
```

## Indices and tables

- {ref}`genindex`
- {ref}`modindex`
- {ref}`search`
