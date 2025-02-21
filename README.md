[![crates.io](https://img.shields.io/crates/v/mdbook-callouts.svg)](https://crates.io/crates/mdbook-callouts)
[![docs.rs](https://docs.rs/mdbook-callouts/badge.svg)](https://docs.rs/mdbook-callouts)
[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](./LICENSE)
[![Build](https://github.com/GrayJack/rs-mdbook-callouts/actions/workflows/build.yml/badge.svg)](https://github.com/GrayJack/rs-mdbook-callouts/actions/workflows/build.yml)
[![Test](https://github.com/GrayJack/rs-mdbook-callouts/actions/workflows/test.yml/badge.svg)](https://github.com/GrayJack/rs-mdbook-callouts/actions/workflows/test.yml)
[![Audit](https://github.com/GrayJack/rs-mdbook-callouts/actions/workflows/audit.yml/badge.svg)](https://github.com/GrayJack/rs-mdbook-callouts/actions/workflows/audit.yml)

# mdbook-callouts


[mdBook] preprocessor to add [Obsidian Flavored Markdown's Callouts](https://help.obsidian.md/Editing+and+formatting/Callouts) to your book like:

```markdown
> [!INFO]
> Highlights information of additional information that users should take into
> account, even when skimming.

> [!NOTE]
> Highlights information that users should take into account, even when skimming.

> [!ABSTRACT]
> A summary or abstract of the information the user is reading.

> [!TODO]
> A reminder of an action to take at a later time.

> [!TIP]
> Optional information to help a user be more successful.

> [!IMPORTANT]
> Crucial information necessary for users to succeed.

> [!SUCCESS]
> Success information to a user.

> [!QUESTION]
> Question for the user to consider.

> [!WARNING]
> Critical content demanding immediate user attention due to potential risks.

> [!CAUTION]
> Negative potential consequences of an action.

> [!FAILURE]
> Information about a failure.

> [!DANGER]
> Information about a danger or a hazardous situation that users need to avoid.

> [!BUG]
> Information about a bug or an issue that users need to be aware of.

> [!EXAMPLE]
> Example of a point or solution that users can apply.

> [!QUOTE]
> Quoted information that is particularly relevant or insightful.

> [!QUOTE] Custom title example
> You can set a custom title by adding the title in the same line as the tag.
```

into

![Rendered example](https://github.com/GrayJack/rs-mdbook-callouts/blob/main/example/example-light.png?raw=true)

![Rendered example 2](https://github.com/GrayJack/rs-mdbook-callouts/blob/main/example/example-rust.png?raw=true)

![Rendered example 3](https://github.com/GrayJack/rs-mdbook-callouts/blob/main/example/example-coal.png?raw=true)

![Rendered example 4](https://github.com/GrayJack/rs-mdbook-callouts/blob/main/example/example-navy.png?raw=true)

![Rendered example 5](https://github.com/GrayJack/rs-mdbook-callouts/blob/main/example/example-ayu.png?raw=true)

[mdBook]: https://github.com/rust-lang/mdBook

## Usage

First, install the preprocessor:

```bash
cargo install mdbook-callouts
```

Then, add the preprocessor to your `book.toml`:

```toml
[book]
authors = ["Alisue"]
language = "en"
multilingual = false
src = "src"
title = "mdBook Alerts preprocessor"

# ADD THIS
[preprocessor.callouts]
```

## License

The code follows the MIT license written in [LICENSE](./LICENSE). Contributors
need to agree that any modifications sent to this repository follow the license.
