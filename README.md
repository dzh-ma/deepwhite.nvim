<p align="center">
  <h2 align="center">DeepWhite</h2>
</p>

![screenshot](https://github.com/dzh-ma/deepwhite.nvim/assets/145275422/d9b6c410-c2d4-454f-a36a-7762581cecc5)

## About

DeepWhite is a light colorscheme inspired by [flatwhite-syntax](https://github.com/biletskyy/flatwhite-syntax) and [elegant-emacs](https://github.com/rougier/elegant-emacs).
This fork of [DeepWhite](https://github.com/Verf/deepwhite.nvim) serves to add [Neorg](https://github.com/nvim-neorg/neorg) syntax highlighting for added readability.

## Installation

```lua
-- for packer.nvim
use {
    'dzh-ma/deepwhite.nvim',
    config = function()
        vim.cmd.colorscheme("deepwhite")
    end,
}

-- for lazy.nvim
{
    'dzh-ma/deepwhite.nvim',
    lazy = false,
    priority = 1000,
    config = function()
        vim.cmd.colorscheme("deepwhite")
    end,
}
```

## Configuration

```lua
require('deepwhite').setup({
    -- If you have some anti-blue light setting (f.lux, light bulb, or low blue light mode monitor),
    -- turn it on, this will set the background color to a cooler color to prevent the background from being too warm.
    low_blue_light = true
})
