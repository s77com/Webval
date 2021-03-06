# webval.vim

HTML and CSS validation plugin for Vim using the W3C Validator API.
## How to install

### Using Vim Plug:

Add the **following** to your `.vimrc` file:
``
Plug 'arunsahadeo/webval'
``

### Using Vundle:

Add the **following** to your `.vimrc` file:
``
Plugin 'arunsahadeo/webval'
``

### Installing manually:

Place the plugin file somewhere under your `~/.vim` folder and add the **following** to your `.vimrc` file:

`set rtp+=~/.vim/
runtime /path/to/webval.vim`

Note: you will also need `jq` installed and available on your `$PATH` variable.

### Commands:

```bash
:ValiHTML - Validates any HTML contained in the file currently open in the buffer if it corresponds to one of the whitelisted filetypes
:ValiCSS - Validates any CSS contained in the file currently open in the buffer if it has a .css extension
:PurgeFiles - Deletes the JSON file generated by the ValiCSS command, or the JSON / HTML files generated by the ValiHTML command (a HTML file will be generated if you use :ValiHTML on a whitelisted PHP file)
```
