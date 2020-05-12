# Using A Local Dependency

Actually using a local dependency as a module can be tricky. This is because of historic issues with both NPM and Yarn. 

In this repo, we demonstrate how to use a local dependency for Factor plugin development. 

There are some caveats however. 

- The module must have `factor` in the name. This is to let Factor know it needs to transpile it. 
- You have to use npm or Yarn `link` which will create a symbolic link from your app's `node_modules` to the local module.
  - Run the link command in the local module (my-factor-plugin-example) to make the reference
  - Run the link command in the app directory to the module to set the reference in the root

The process of using a local dependency as a module can be confusing. This is due to issues with `node_modules`. 

If you have any questions, please file an issue on the [core Factor repo](https://github.com/fiction-com/factor/).