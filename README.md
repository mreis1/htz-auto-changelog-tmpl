# Templates for auto-changelog




Checkout the project at https://www.npmjs.com/package/auto-changelog

```
Usage: auto-changelog [options]
 
Options:
 
  -o, --output [file]                 # output file, default: CHANGELOG.md 
  -c, --config [file]                 # config file location, default: .auto-changelog 
  -t, --template [template]           # specify template to use [compact, keepachangelog, json], default: compact 
  -r, --remote [remote]               # specify git remote to use for links, default: origin 
  -p, --package                       # use version from package.json as latest release 
  -v, --latest-version [version]      # use specified version as latest release 
  -u, --unreleased                    # include section for unreleased changes 
  -l, --commit-limit [count]          # number of commits to display per release, default: 3 
  -b, --backfill-limit [count]        # number of commits to backfill empty releases with, default: 3 
      --commit-url [url]              # override url for commits, use {id} for commit id 
      --issue-url [url]               # override url for issues, use {id} for issue id 
      --merge-url [url]               # override url for merges, use {id} for merge id 
      --compare-url [url]             # override url for compares, use {from} and {to} for tags 
      --issue-pattern [regex]         # override regex pattern for issues in commit messages 
      --breaking-pattern [regex]      # regex pattern for breaking change commits 
      --merge-pattern [regex]         # add custom regex pattern for merge commits 
      --ignore-commit-pattern [regex] # pattern to ignore when parsing commits 
      --tag-pattern [regex]           # override regex pattern for release tags 
      --tag-prefix [prefix]           # prefix used in version tags, default: v 
      --starting-commit [hash]        # starting commit to use for changelog generation 
      --sort-commits [property]       # sort commits by property [relevance, date, date-desc], default: relevance 
      --include-branch [branch]       # one or more branches to include commits from, comma separated 
      --release-summary               # display tagged commit message body as release summary 
      --handlebars-setup [file]       # handlebars setup file 
      --append-git-log [string]       # string to append to git log command 
      --stdout                        # output changelog to stdout 
  -V, --version                       # output the version number 
  -h, --help                          # output usage information 
 
 
# Write log to CHANGELOG.md in current directory 
auto-changelog
 
# Write log to HISTORY.md using keepachangelog template 
auto-changelog --output HISTORY.md --template keepachangelog
 
# Disable the commit limit, rendering all commits for every release 
auto-changelog --commit-limit false
```
