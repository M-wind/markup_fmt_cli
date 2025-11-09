# Markup Fmt Cli

Based on [markup_fmt](https://github.com/g-plane/markup_fmt) lib. All credits to the markup_fmt project.

## Getting Started

### Usage

#### Build

```bash
git clone https://github.com/M-wind/markup_fmt_cli.git
cargo build --release
```

#### With conform.nvim

```bash
require("conform").setup({
    formatters = {
        markup_fmt = {
            inherit = false,
            command = "markup_fmt",
            args = { "-c", "your config path", "format", "$FILENAME" },
        }
    },
    formatters_by_ft = {
        html = { "markup_fmt" },
        ...
    } 
})
```

## Configuration

Please refer to [Configuration](https://markup-fmt.netlify.app/).

