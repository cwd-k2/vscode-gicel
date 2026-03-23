# GICEL for Visual Studio Code

Syntax highlighting for
[GICEL](https://github.com/cwd-k2/gicel) (Go's Indexed Capability
Effect Language) — a Haskell-like embedded typed effect language for Go.

## Features

- Syntax highlighting via TextMate grammar
- All 9 keywords: `case`, `do`, `data`, `type`, `impl`, `import`,
  `infixl`, `infixr`, `infixn`
- Built-in functions: `pure`, `bind`, `thunk`, `force`, `assumption`,
  `rec`, `fix`
- Type constructors, data constructors, module paths
- Type variables in quantifier scopes `\a.` (including kinded variables
  `\(a : Type -> Type).`)
- Function names in type annotations (`::`) and definitions (`:=`)
- Special operators: `->`, `=>` (case alternatives, evidence injection),
  `<-`, `.#`, `@` (type application, grade annotation), `\`
- String, rune, and integer literals with escape sequences
- Line comments (`--`) and nestable block comments (`{- ... -}`)
- Bracket pairing, auto-closing, and indentation support

## Installation

### From VSIX

```sh
git clone https://github.com/cwd-k2/vscode-gicel.git
cd vscode-gicel
npx @vscode/vsce package
code --install-extension gicel-*.vsix
```

### From Source (development)

Open this directory in VS Code and press `F5` to launch an Extension
Development Host.

## Related

- [tree-sitter-gicel](https://github.com/cwd-k2/tree-sitter-gicel) —
  Tree-sitter grammar (Neovim, Zed, Helix, Emacs)
- [gicel](https://github.com/cwd-k2/gicel) — GICEL language implementation

## License

MIT
