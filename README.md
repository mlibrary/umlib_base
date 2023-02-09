# umlib_base

## This is the base drupal theme for um library sites. ##

**Please add this theme to your drupal full stack project as a submodule in your *themes* directory using:**

```
cd themes
git submodule add git@github.com:mlibrary/umlib_base.git
```

or

```
cd themes
git submodule add https://github.com/mlibrary/umlib_base.git
```

//TODO - get relevant parts and document
For relevant submodule commands see https://opensource.com/article/20/5/git-submodules-subtrees


You can then add a custom theme for your project based on this theme using the *base theme:* in your themes *info.yml* file. For example:

```
vi themes/umlib_blogs/umlib_blogs.info.yml
```
```
name: UM Library Blogs
type: theme
description: "A theme for UM Library Blogs."
core_version_requirement: ^9 || ^10
base theme: umlib_base
regions:
  header: "Header"
  banner: "Banner"
  content: "Content"
  sidebar_first: "Sidebar first"
  footer_first: "Footer First"
  ```

All um_base styles will then be inherited to your project.

For an example visit https://github.com/mlibrary/blogs.lib/tree/main/themes
