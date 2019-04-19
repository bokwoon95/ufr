[![asciicast](https://asciinema.org/a/w5Dw52mj2dupFGMnOGfWRxIr1.svg)](https://asciinema.org/a/w5Dw52mj2dupFGMnOGfWRxIr1)

## Search only
```
   Usage: grepf <pattern> [INCLUDED...] [:: EXCLUDED...] [--OPTIONS...]

   Search for <pattern> within [INCLUDED] files, ignoring [EXCLUDED] files.
   [INCLUDED] files are separated from [EXCLUDED] files by a '::'.
   By default, [INCLUDED] is the current directory.

   Examples:
      grepf pattern
      grepf pattern '*.py'
      grepf pattern file1.txt folder1/ :: folder1/file2.txt
      grepf pattern :: file1.txt '**/*.log'

   Options:
      --help       Show this help
      --list       List the files that are affected
      --describe   Show the full command that grepf transforms into
      --raw        Raw unfiltered searches i.e. .git/ is filtered by default, this
                   turns it off

   Note:
      Any [--OPTIONS] you can pass to grep, you can pass to grepf as well.
      If in doubt, wrap it in single quotes 'like this'
```

## Search and Replace
```
   Usage: rgrepf <old> <new> [INCLUDED...] [:: EXCLUDED...] [--OPTIONS...]

   Search and replace <old> with <new> in [INCLUDED] files, ignoring [EXCLUDED] files.
   [INCLUDED] files are separated from [EXCLUDED] files by a '::'.
   By default, [INCLUDED] is the current directory.

   Examples:
      rgrepf old new
      rgrepf old new '*.py'
      rgrepf old new file1.txt folder1/ :: folder1/file2.txt
      rgrepf old new :: file1.txt '**/*.log'

   Options(only for rgrepf):
      --help       Show this help
      --list       List the files that are affected
      --describe   Show the full command that grepf transforms into
      --raw        Raw unfiltered searches i.e. .git/ is filtered by default, this
                   turns it off

   Note:
      Any [--OPTIONS] you can pass to grep, you can pass to grepf as well.
      If in doubt, wrap it in single quotes 'like this'
```
