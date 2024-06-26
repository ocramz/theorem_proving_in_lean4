Theorem Proving in Lean 4
-----------------------

This manual is generated by [mdBook](https://github.com/rust-lang/mdBook). We are currently using a
[fork](https://github.com/leanprover/mdBook) of it for the following additional features:

* Add support for hiding lines in other languages [#1339](https://github.com/rust-lang/mdBook/pull/1339)
* Replace calling `rustdoc --test` from `mdbook test` with `./test`

To build this manual, first install the fork via
```bash
cargo install --git https://github.com/leanprover/mdBook mdbook
```

To build a PDF, we use [mdbook-pdf](https://github.com/HollowMan6/mdbook-pdf), which requires Chrome (or Edge on Windows) to be installed first. See the README of mdbook-pdf.

```bash
cargo install --git https://github.com/HollowMan6/mdbook-pdf.git
```

and add the appropriate incantations to `book.toml` (as per the mdbook-pdf README).


Then use e.g. [`mdbook watch`](https://rust-lang.github.io/mdBook/cli/watch.html) in the root folder:
```bash
mdbook watch --open  # opens the output in `out/` in your default browser
```

Run `mdbook test` to test all `lean` code blocks.

## How to deploy

```
./deploy.sh
```
