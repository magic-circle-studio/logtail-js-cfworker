### Fork of [logtail/logtail-js](https://github.com/logtail/logtail-js) to support Cloudfare Workers

### Contributors: how to keep this up to date

1. Clone this repo
2. Merge upstream/master into master
3. You'll get merge commits in package.json, namely the versions not matching.
   Resolve the commits, and bump this package's version to match upstream.
4. Commit and push
5. `cd packages/node` (this is the package we modified to support Workers)
6. `yarn publish`. Don't input a new version when prompted, just hit enter to use the version
	 in package.json.
7. Go [here](https://www.npmjs.com/package/@magiccircle/logtail-cfworker) to
	 make sure the new version is published.
8. Now you can use the new version in your Workers project!