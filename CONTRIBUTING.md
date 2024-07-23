# Contribution Guidelines

Thank you for your interest in contributing to [dwave-examples](https://github.com/dwave-examples)! Before getting
started, we encourage you to take a look at this document of guidelines.

## What We're Looking For

While we have a preference for application-oriented examples, we welcome all
examples that demonstrate use of Ocean&#8482; SDK tools.

To see our categorized collection of demos, create a free account on the
[Leap&#8482; Quantum Cloud Service](https://cloud.dwavesys.com/leap/signup/) and take a look at
[our library of examples](https://cloud.dwavesys.com/leap/examples/) or
go through the demo code repositories in [dwave-examples](https://github.com/dwave-examples).

## Steps for Contributing

1. Follow GitHub's instructions on [creating a repository from a template](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template).
   Alternatively, clone this repository (or one of our [existing examples](https://github.com/dwave-examples)) as a
   starting point from which to implement your example.

2. [Open an issue](https://github.com/dwave-examples/template-dash/issues/new/choose) in the
   [dwave-examples/template-dash](https://github.com/dwave-examples/template-dash) repository with a link to your example.

3. To add your example, D-Wave will fork your repository. We may make a pull
   request if we would like your approval for certain code changes.

## Guidelines

### Files

Please make sure that your example includes the following:

* `README.md`:
    * Should be written in Markdown (and not reStructuredText).
    * See this repository's [README](README.md).

* `requirements.txt`:
    * `dwave-ocean-sdk` should be unpinned and lower bounded.
    * Add requirements for running your example and make sure they are either pinned to a version supported by the latest Ocean&#8482; SDK release or lower bounded.

* `LICENSE`:
    * Examples should comply with the Apache 2.0 License. Please make sure that:
        * All source and test files include a license header.
        * The [`LICENSE`](LICENSE) file is included in your root directory.

* Tests that are discoverable through `python -m unittest discover`.

Our examples are tested using CircleCI. For a list of operating systems and
Python versions we currently test our examples with, please take a look at [our
documentation](https://docs.ocean.dwavesys.com/en/stable/overview/install.html).
For more information, visit [orb-examples](https://circleci.com/developer/orbs/orb/dwave/orb-examples).

The example repository should contain the [`.circleci/`](.circleci/) directory to support running tests in CI.
Once approved, we will make sure that your example is set up on our CircleCI account.

To ensure that your example runs in [GitHub Codespaces](https://docs.github.com/en/codespaces/overview),
make sure to include the [`.devcontainer/`](.devcontainer/) directory into your example's root directory.

### Code

We use the [PEP 8](https://www.python.org/dev/peps/pep-0008/) style guide as a baseline.

If your example is lengthy, we encourage modularity for ease of testing.

### Documentation

We use the [Google docstrings convention](https://google.github.io/styleguide/pyguide.html#38-comments-and-docstrings).

Take a look at our [How to Contribute](https://docs.ocean.dwavesys.com/en/latest/contributing.html#documentation-and-comments)
guide for more details.
