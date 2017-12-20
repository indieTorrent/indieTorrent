# Contributing to indieTorrent projects

The following is a set of guidelines for contributing to indieTorrent and its packages, which are hosted in the [indieTorrent Organization](https://github.com/indieTorrent) on GitHub. These are mostly guidelines, not rules. Use your best judgment, and feel free to propose changes to this document in a pull request.

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
* When only changing documentation, include `[ci skip]` in the commit description
* Consider starting the commit message with one of the following:

    * `chore:` => mainly related to build or env
    * `feat:` => when adding features
    * `fix:` => when fixing a bug
    * `ui:` => anything interface related
    * `refact:` => moving code around
    * `style:` => code style, linting...
    * `tests:` => When adding or changing tests
    * `doc:` => when adding or editing documentation
    
* Left this in here for comparison:
    * :art: `:art:` when improving the format/structure of the code
    * :racehorse: `:racehorse:` when improving performance
    * :non-potable_water: `:non-potable_water:` when plugging memory leaks
    * :memo: `:memo:` when writing docs
    * :penguin: `:penguin:` when fixing something on Linux
    * :apple: `:apple:` when fixing something on macOS
    * :checkered_flag: `:checkered_flag:` when fixing something on Windows
    * :bug: `:bug:` when fixing a bug
    * :fire: `:fire:` when removing code or files
    * :green_heart: `:green_heart:` when fixing the CI build
    * :white_check_mark: `:white_check_mark:` when adding tests
    * :lock: `:lock:` when dealing with security
    * :arrow_up: `:arrow_up:` when upgrading dependencies
    * :arrow_down: `:arrow_down:` when downgrading dependencies
    * :shirt: `:shirt:` when removing linter warnings

### JavaScript Styleguide

All JavaScript must adhere to [JavaScript Airbnb Style](https://github.com/airbnb/javascript/).



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
