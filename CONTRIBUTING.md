# Core Flight System Contributing Guide

So you'd like to contribute to cFS? Below are some guidelines for contributors to follow. Contributions come in all shapes and sizes. We appreciate your help with documentation, unit tests, framework code, continuous-integration, or simply reporting bugs and improvement ideas. We can't promise that we'll accept every suggestion or fix every bug in a timely manner but at the very least we'll respond to you.

## Did you find a bug or want to request a new feature?
First, search through the open issues in each submodule to ensure that your ticket is relevant, not redundant, nor in conflict with other tickets:
- [cFE Issues](https://github.com/nasa/cfe/issues)
- [osal Issues](https://github.com/nasa/osal/issues)
- [PSP Issues](https://github.com/nasa/psp/issues)
- [sample_app Issues](https://github.com/nasa/sample_app/issues)
- [sample_app Issues](https://github.com/nasa/sample_lib/issues)
- [cFS-GroundSystem](https://github.com/nasa/cFS-GroundSystem/issues)
- [cFS Bundle Issues](https://github.com/nasa/cfs/issues)

If your bug or feature hasn't been reported or requested before, create a new issue in the appropriate repository. If it you find a similar issue, please add a comment on it with your experience or input.


## Ready to add your code?

Follow GitHub's fork-branch-pull request pattern.
1. Fork the relevant cFS component (eg. cfe, osal, psp),
2. Create a new branch in your fork to work on your fix. Please name your branch `fix-ISSUE_NUMBER-<FIX_SUMMARY>`.
3. Submit a pull request to the nasa `main` branch. Follow a similar naming pattern with your We recommend creating your pull-request as a "draft" and to commit early and often so the community can give you feedback at the beginning of the process as opposed to asking you to change hours of hard work at the end.
4. Add commits to your branch. Please follow commit message convention: `Fix ISSUE_NUMBER, 50-ish-character-long summary of commit content`
5. Download print, sign, and email our [contributor license agreement]() to FIXME

## Writing high-quality code

1. Follow cFS code conventions (formatting, symbol naming, file naming, etc) but do *not* change/reformat existing code except to address your changes.

2. For any new API's, add unit tests to cover nominal and off-nominal conditions.

3. Add/edit stubs to the unit test codebase for any new/modified functions.

4. For any changes to existing API's, alter the unit tests to cover the changes (and remove tests made irrelevant due to your changes).

5. Test your code, on a Linux platform (at minimum) --
    _TODO:_ Specific distros/versions/CPU architectures of Linux?

6. Build your code, including unit tests.
    _TODO:_ need "standard" build process.

6. Run the unit tests (all passed, yes?)
    _TODO:_ need "standard" test procedure.

7. Run the main cfs executable (no errors reported, yes?)
    _TODO:_ need "standard" test procedure, including targets.cmake recommendations.

8. ?? Do we expect contributors to run coverage ?? Guessing no.
