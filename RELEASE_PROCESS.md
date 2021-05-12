# Release Process

This documents the steps required for making a release of the syntax
highlighter.

1. Change the version field in package.json and commit.
2. Create a tag for the version.
3. Push changes and the tag and merge to master.
4. Run "npm run package" in the root, this will create you a .vsix.
5. Distribute that .visx release as appropriate.
