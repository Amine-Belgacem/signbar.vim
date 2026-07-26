# vim-scrollsign.vim

vim-scrollsign.vim is a lightweight Vim plugin that adds a visual scrollbar-like indicator to the sign column. It helps you quickly understand where the current viewport sits inside a long buffer without relying on a GUI scrollbar.

## Features

- Renders a scrollbar-style marker using Vim signs
- Updates automatically when you move the cursor, resize the window, or switch buffers
- Supports basic customization for the marker character and redraw frequency
- Works well for navigating large files in Vim

## Installation

Using vim-plug:

```vim
call plug#begin()
Plug 'Amine-Belkacem/visual-scroll.vim'
call plug#end()
```

Then run:

```vim
:PlugInstall
```

## Configuration

The plugin works out of the box, but you can tweak a couple of options:

```vim
" Change the scrollbar marker (default: |)
let g:scrollbarFG = '▌'

" Redraw interval in milliseconds (default: 300)
let g:sbUpdate = 250
```

## Usage

Once installed, the scrollbar appears automatically as you navigate buffers and windows. No extra commands are required.

## Notes

- The plugin uses Vim signs, so it is best suited to environments with sign support.
- Very short buffers do not show a scrollbar because there is no need for one.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
