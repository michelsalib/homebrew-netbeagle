# Homebrew tap for netbeagle

[netbeagle](https://github.com/michelsalib/netbeagle) shows which process (or container) listens on each
port, who can reach it, who is connected to it, and how everything on your machine connects.

```sh
brew install michelsalib/netbeagle/netbeagle
```

This installs the standalone binary from the GitHub release (macOS and Linux, arm64 and x64), with bash
and fish completion: commands, options, and for `who` and `kill` the ports listening now. For zsh, add
`eval "$(netbeagle completion zsh)"` to `~/.zshrc`, after `compinit`. Update with `brew upgrade netbeagle`.
Without root, other users' sockets show no process: `sudo netbeagle` shows them all.

`Formula/netbeagle.rb` is generated for each release by `scripts/packages.ts` in the netbeagle
repository, from the release's `SHA256SUMS`.
