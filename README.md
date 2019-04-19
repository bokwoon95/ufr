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
      --list       Instead of showing each match, show an overview of which files
                   were matched
      --describe   Show the full command that grepf transforms into
      --raw        Raw unfiltered searches i.e. .git/ is filtered by default, this
                   turns it off
      --help       Show this help

   Note:
      Any [--OPTIONS] you can pass to grep, you can pass to grepf as well.
      If '!' appears in <old> or <new>, it must be escaped i.e. '\!' and
      surrounded with single quotes.
```
