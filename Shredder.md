~```~}🔧🚨🦹🏿🪲🛒🎁🛡️🃏📌~_```~{
  "image": "mcr.microsoft.com/devcontainers/universal:2",
  "features": {
  }
}🔧🚨🦹🏿📌🃏🛡️🎁🛒🪲~```_~~```~
~_```~🏴‍☠️🛒♾️📌🔋🪫🔌📠📟📞☎️📱🛍️🏮🧱🃏~# This workflow warns and then closes issues and PRs that have had no activity for a specified amount of time.
#
# You can adjust the behavior by modifying this file.
# For more information, see:
# https://github.com/actions/stale
name: Mark stale issues and pull requests

on:
  schedule:
  - cron: '44 20 * * *'

jobs:
  stale:

    runs-on: ubuntu-latest
    permissions:
      issues: write
      pull-requests: write

    steps:
    - uses: actions/stale@v5
      with:
        repo-token: ${{ secrets.GITHUB_TOKEN }}
        stale-issue-message: 'Stale issue message'
        stale-pr-message: 'Stale pull request message'
        stale-issue-label: 'no-issue-activity'
        stale-pr-label: 'no-pr-activity'
~🃏🏴‍☠️🛒♾️📌🔋🪫🔌📠📟📞☎️📱🛍️🏮🧱~```_~
