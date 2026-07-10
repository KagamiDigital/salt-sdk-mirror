# salt-sdk-mirror

`salt-sdk-mirror` is a restricted pre-release of the next major version of `salt-sdk`. While it is in closed testing, it is available only on Github packages. When a public version is available, it will be on npm, just like before

## Using Github packages
After passing your Github username to a member of the Salt team, and confirming they have granted you access to the repository, you need to configure npm to install `salt-sdk-mirror` from Github. See [Github's instructions here](https://docs.github.com/en/packages/working-with-a-github-packages-registry/working-with-the-npm-registry#authenticating-with-a-personal-access-token)

1. Have a salt team member add you do the `salt-sdk-mirror` repository as an external collaborator with `read` access
2. Create your own **classic [Personal Access Token](https://github.com/settings/tokens/new)** with `package:read` permission
3. Add this to `.npmrc` in your project route:
```
 @kagamidigital:registry=https://npm.pkg.github.com
  //npm.pkg.github.com/:_authToken=YOUR_CLASSIC_PAT
```
4. `npm install @kagamidigital/salt-sdk-mirror`

# Documentation
https://kagamidigital.github.io/salt-sdk-mirror/

# Beta Status
Salt is in Beta. By using Salt, you acknowledge that you understand the software's Beta status and will not hold the Salt team, platform, builders or affiliates responsible for any losses incurred.

You also acknowledge that you have read and understood the [Terms of Use](https://salt.space/terms/app/).
