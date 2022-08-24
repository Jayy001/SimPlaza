# SimPlaza CLI
Unofficial CLI of the SimPlaza website for flightsimmers 
Current version: 1.1.5

# How to install?

Install via pip:

```
pip install simplaza
```

...or download the complied executable file from the release page (made with auto-py-to-exe)

# How to use?

```
> simplaza --help
Usage: simplaza [OPTIONS] [QUERY]

  SimPlaza CLI - Query and download files from SimPlaza directly from your
  terminal

  GitHub:

          https://github.com/Jayy001/SimPlaza

  Usage:

          simplaza <query>

Options:
  --magnet   Opens magnet link
  --json     Returns search results
  --default  Gets first option automatically
  --help     Show this message and exit.
 ```

By default the CLI will download the torrent file for the addon you want, you can use the `--magnet` option to change this into a magneturi which will then automatically open with the registered application (for example, when installing picotorrent by default the webbrowser will open it for any given magnet links)

If you only want to view the results from the search query, and not download them use the `--json` option instead. Futhermore, if you want to completley skip over choosing what addon you want from the table you can use the `--default` option will use the first avaliable option from the search query

Finally, you can also give a file path (i.e C:\..\..\addons.txt) in the format of addon you want to download per line, for example;

```
eglk
crj
heathrow
```

Note: Using the file option also works with `--magnet` and `--default` option, so if you want to automate it all from one command I would use `simplaza --default --magnet file.txt` to automatically send every addon to your torrent client without any user interaction




