# Contributing

## Questions

If you have issues with the APIs or have a question about the Watson services, see [Stack Overflow](https://stackoverflow.com/questions/tagged/ibm-watson+python).

## Issues

If you encounter an issue with the Python SDK, you are welcome to submit a [bug report](https://github.com/watson-developer-cloud/python-sdk/issues).
Before that, please search for similar issues. It's possible somebody has encountered this issue already.

## Pull Requests

If you want to contribute to the repository, here's a quick guide:

1. Fork the repository
1. Install `virtualenv` and `tox`
1. Develop and test your code changes with [pytest].
   - Respect the original code [style guide][styleguide].
   - Only use spaces for indentation.
   - Create minimal diffs - disable on save actions like reformat source code or organize imports. If you feel the source code should be reformatted create a separate PR for this change.
   - Check for unnecessary whitespace with `git diff --check` before committing.
   - Make sure your code supports Python 3.9, 3.10, 3.11. You can use `pyenv` and `tox` for this
1. Make the test pass
1. Commit your changes

- Commits should follow the [Angular commit message guidelines](https://github.com/angular/angular/blob/master/CONTRIBUTING.md#-commit-message-guidelines). This is because our release tool uses this format for determining release versions and generating changelogs. To make this easier, we recommend using the [Commitizen CLI](https://github.com/commitizen/cz-cli) with the `cz-conventional-changelog` adapter.

1. Push to your fork and submit a pull request to the `dev` branch

## Running the tests

You probably want to set up a [virtualenv].

1. Clone this repository:
   ```sh
   git clone https://github.com/watson-developer-cloud/python-sdk.git
   ```
1. Install the sdk as an editable package using the current source:
   ```sh
   pip install --editable .
   ```
1. Install the test dependencies with:
   ```sh
   pip install -r requirements-dev.txt
   ```
1. Run the test cases with:
   ```sh
   py.test test
   ```

## Bug Bounty Hunters Notice
API keys found from commit bec3ae23b53782370851e28cbda5033a596b58b5 have already been revoked and will not be accepted for bug bounties.

## Additional Resources

- [General GitHub documentation](https://help.github.com/)
- [GitHub pull request documentation](https://help.github.com/send-pull-requests/)

[dw]: https://developer.ibm.com/answers/questions/ask/?topics=watson
[stackoverflow]: http://stackoverflow.com/questions/ask?tags=ibm-watson
[styleguide]: http://google.github.io/styleguide/pyguide.html
[pytest]: http://pytest.org/latest/
[virtualenv]: http://virtualenv.readthedocs.org/en/latest/index.html
