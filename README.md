<p align="center">
  <img id="logo" alt="Github Autocompletion" src="./public/github.png" height="128" />
</p>

# 📣 Git Autocompletion

![MIT License][license-badge]
![Coverage Status][coverage-badge]

_Git Autocompletion_ allows you to install git autocomplete in one simple step!,
inspired by https://www.oliverspryn.com/blog/adding-git-completion-to-zsh

## Contents

1. [Requirements](#requirements)
2. [How it works](#how-it-works)
3. [Command](#command)
4. [Permissions](#permissions)
5. [License](#license-mit)

## Requirements

- deno 1.36.4

## How it works

_git autocompletion_ downloads two scripts from github

- A git completion script:
  `https://raw.githubusercontent.com/git/git/master/contrib/completion/git-completion.bash`
- And a zsh completion wrapper for git
  `https://raw.githubusercontent.com/git/git/master/contrib/completion/git-completion.zsh`

Once this two files are downloaded in your homedir, a new `.zshrc` will be
created (in case of non existance, if not some lines will get appended), and
then it will proceed to clear out the shell’s autocompletion cache.

After that, you can just refresh your terminal and that's it!

## Command

Run

```bash
deno task start
```

then reload your shell and you are good to go!

## Permissions

When executing `deno task start`, following permissions will be granted

- `--allow-env=HOME`: Allows `home` environment variable
- `--allow-read=/Users`: Allows read access to `/Users` folder
- ` --allow-write=/Users`: Allows write access to `/Users` folder
- `--allow-net=raw.githubusercontent.com`: Allows network access to `raw.githubusercontent.com` in order to download scripts

## Useful links

- ⏳ [Changelog][changelog]: List of changes between versions.
- ✅ [Tests Coverage][coverage]: Coveralls page with tests coverage.

## License MIT

Project License can be found [here](LICENSE.md).

[changelog]: https://github.com/RisingSquad/git-autocompletion/blob/main/CHANGELOG.md
[coverage]: https://coveralls.io/github/RisingSquad/git-autocompletion
[license-badge]: https://img.shields.io/badge/license-MIT-007EC7.svg
[coverage-badge]: https://coveralls.io/repos/github/RisingSquad/git-autocompletion/badge.svg?

##### [Back to Contents](#contents)
