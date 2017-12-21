# Contributing to indieTorrent projects

The following is a set of rules for contributing to indieTorrent and its packages, which are hosted in the [indieTorrent Organization](https://github.com/indieTorrent) on GitHub. These rules are considered when approving submitted contributions. Feel free to propose changes to this document in a pull request.

#### Table Of Contents

[Organization name](#organization-name)

[Styleguides](#styleguides)
  * [Git Commit Messages](#git-commit-messages)
  * [JavaScript Styleguide](#javascript-styleguide)

## Organization name

When using the name of the organization, make sure it is one of the following:
  * `indieTorrent` => generally acceptable
  * `indieTorrent.org` => generally acceptable
  * `indieTorrent.org, LLC` => required in every legal context (such as in copyright notices)
## Styleguides

### Git Commit Messages

* Use the present tense ("Add feature" not "Added feature")
* Use the imperative mood ("Move cursor to..." not "Moves cursor to...")
* Limit the first line to 72 characters or less
* Reference issues and pull requests liberally after the first line

* Commit conventions follow this pattern:
    ```bash
    type(scope?): subject
    body?
    footer?
    ```
    *`?` means its optional*
 
* The accepted types are:

    * `build:`  *Related to Build or Environment*
    * `chore:`  *Also Accepted for Build or Environment*
    * `ci:`     *Related to TravisCI*
    * `docs:`   *Related to Documentation*
    * `feat:`   *Related to Features*
    * `fix:`    *Related to Bug Fixes*
    * `perf:`   *Related to Performance*
    * `refact:` *Related to Refactoring or moving code around*
    * `revert:` *Related to reverting a previous commit (this is discouraged)*
    * `style:`  *Related to Coding Style or Linting (not to be confused with `ui` styles)*
    * `tests:`  *Related to tests*
    * `ui:`     *Related to UI (Web/Interface)*

### JavaScript Styleguide

All JavaScript must adhere to [JavaScript Airbnb Style](https://github.com/airbnb/javascript/), including additional custom rules, which are defined in the `rules` object in the [.eslintrc.js file](https://github.com/indieTorrent/website-ui/blob/master/.eslintrc.js).

* Prefer the object spread operator (`{...anotherObj}`) to `Object.assign()`

* Inline `export`s with expressions whenever possible

  ```js
  // Use this:
  export default class ClassName {

  }

  // Instead of:
  class ClassName {

  }
  export default ClassName
  ```
