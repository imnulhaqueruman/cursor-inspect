# rg-strings.txt

Clap argument definition strings extracted from the Cursor-bundled `rg`
binary (ripgrep 15.1.0-cursor5).

These are the short / long flag aliases and their clap help summaries
emitted before each flag's description in `rg --help`. Useful for:

- Confirming Cursor's ripgrep fork still uses the upstream flag surface
- Spotting any Cursor-only flag aliases (none present here beyond what
  `rg-help.txt` already showed)
- Cross-referencing the `rg --help` rendering with the binary's
  embedded definitions

## Raw content

```text
        with a dash, use the -e/--regexp flag.
      auto\:"identical to --auto-hybrid-regex"
      pcre2\:"identical to --pcre2"
    "(--no-ignore-global --no-ignore-parent --no-ignore-vcs --no-ignore-dot)--no-ignore[don't respect ignore files]"
    "(1 stats)--files[show each file that would be searched (but don't search)]"
    "(pretty-vimgrep)--no-heading[don't show matches grouped by file name]"
    "--binary[search binary files, don't print binary data]"
    "--no-config[don't load configuration files]"
    "--no-ignore-dot[don't respect .ignore files]"
    "--no-ignore-exclude[don't respect local exclude (ignore) files]"
    "--no-ignore-files[don't respect --ignore-file flags]"
    "--no-ignore-global[don't respect global ignore files]"
    "--no-ignore-messages[don't show ignore-file parse error messages]"
    "--no-ignore-parent[don't respect ignore files in parent directories]"
    "--no-ignore-vcs[don't respect version control ignore files]"
    "--no-mmap[don't search using memory maps]"
    "--no-require-git[don't require git repository to respect gitignore rules]"
    "--one-file-system[don't descend into directories on other file systems]"
    # (--[imnp]* => --ignore*, --messages, --no-*, --pcre2-unicode)
    $no"(--no-multiline)--no-multiline-dotall[don't allow \".\" to match newline (with -U)]"
    $no"(--null-data)--no-text[don't search binary files as if they were text]"
    $no"--messages[don't suppress error messages affected by --no-messages]"
    $no"--no-auto-hybrid-regex[DEPRECATED: don't dynamically use PCRE2 if necessary]"
    $no"--no-binary[don't search binary files]"
    $no"--no-block-buffered[don't force block buffering]"
    $no"--no-byte-offset[don't show byte offsets for each matching line]"
    $no"--no-column[don't show column numbers for matches]"
    $no"--no-context-separator[don't print context separators]"
    $no"--no-crlf[don't use CRLF as line terminator]"
    $no"--no-fixed-strings[don't treat pattern as literal string]"
    $no"--no-follow[don't follow symlinks]"
    $no"--no-hidden[don't search hidden files and directories]"
    $no"--no-include-zero[don't include files with zero matches in summary]"
    $no"--no-invert-match[do not invert matching]"
    $no"--no-json[don't output results in JSON Lines format]"
    $no"--no-line-buffered[don't force line buffering]"
    $no"--no-max-columns-preview[don't show preview for long lines (with -M)]"
    $no"--no-search-zip[don't search in compressed files]"
    $no"--no-sort-files[DEPRECATED: do not sort results]"
    $no"--no-stats[don't show search statistics]"
    $no"--no-trim[don't trim ASCII whitespace prefix from each line]"
    $no'(--ignore-global --ignore-parent --ignore-vcs --ignore-dot)--ignore[respect ignore files]'
    $no'(--no-pcre2 --no-pcre2-unicode)--pcre2-unicode[DEPRECATED: enable PCRE2 Unicode mode (with -P)]'
    $no'(multiline-dotall)--no-multiline[restrict matches to at most one line each]'
    $no'(pcre2-unicode)--no-pcre2[disable matching with PCRE2]'
    $no'--ignore-dot[respect .ignore files]'
    $no'--ignore-exclude[respect local exclude (ignore) files]'
    $no'--ignore-files[respect --ignore-file files]'
    $no'--ignore-global[respect global ignore files]'
    $no'--ignore-messages[show ignore-file parse error messages]'
    $no'--ignore-parent[respect ignore files in parent directories]'
    $no'--ignore-vcs[respect version control ignore files]'
    $no'--no-encoding[use default text encoding]'
    $no'--no-glob-case-insensitive[treat -g/--glob patterns case sensitively]'
    $no'--no-ignore-file-case-insensitive[process ignore files case sensitively]'
    $no'--no-one-file-system[descend into directories on other file systems]'
    $no'--no-pre[disable preprocessor utility]'
    $no'--require-git[require git repository to respect gitignore rules]'
    $no'--unicode[enable Unicode mode]'
    '!--maxdepth=:number of directories'
    '(--files --type-list file regexp)1: :_guard "^-*" pattern'
    '(--files file-match)--stats[show search statistics]'
    '(--no-ignore-messages)--no-messages[suppress some error messages]'
    '(--no-multiline)--multiline-dotall[allow "." to match newline (with -U)]'
    '(--no-pcre2 --pcre2-unicode)--no-pcre2-unicode[DEPRECATED: disable PCRE2 Unicode mode (with -P)]'
    '(--pre)'{-z,--search-zip}'[search in compressed files]'
    '(--type-list)*: :_files'
    '(--vimgrep)--passthrough[alias for --passthru]'
    '(--vimgrep)--passthru[show both matching and non-matching lines]'
    '(-0 --null)'{-0,--null}'[print NUL byte after file names]'
    '(-M --max-columns)'{-M+,--max-columns=}'[specify max length of lines to print]:number of bytes'
    '(-b --byte-offset)'{-b,--byte-offset}'[show 0-based byte offset for each matching line]'
    '(-m --max-count)'{-m+,--max-count=}'[specify max number of matches per file]:number of matches'
    '(-q --quiet)'{-q,--quiet}'[suppress normal output]'
    '(-v --invert-match)'{-v,--invert-match}'[invert matching]'
    '(-z --search-zip)--pre=[specify preprocessor utility]:preprocessor utility:_command_names -e'
    '(1 file)*'{-e+,--regexp=}'[specify pattern]:pattern'
    '(1)*'{-f+,--file=}'[specify file containing patterns to search for]: :_files'
    '(: * -)'--pcre2-version'[print the version of PCRE2 used by ripgrep, if available]'
    '(: * -)'{-V,--version}'[display version information]'
    '(: * -)'{-h,--help}'[display help information]'
    '(: *)--type-list[show all supported file types and their associated globs]'
    '(context-a context-b)'{-C+,--context=}'[specify lines to show before and after each match]:number of lines'
    '(context-c)'{-A+,--after-context=}'[specify lines to show after each match]:number of lines'
    '(context-c)'{-B+,--before-context=}'[specify lines to show before each match]:number of lines'
    '(heading passthru)--vimgrep[show results in vim-compatible format]'
    '(heading)'{-p,--pretty}'[alias for --color=always --heading -n]'
    '(pretty-vimgrep)--heading[show matches grouped by file name]'
    '(sort)'{-j+,--threads=}'[specify approximate number of threads to use]:number of threads'
    '(stats)'{-l,--files-with-matches}'[only show names of files with matches]'
    '(stats)--files-without-match[only show names of files without matches]'
    '(text)--null-data[use NUL as line terminator]'
    '(threads)--sort-files[DEPRECATED: sort results by file path (buffers results; higher memory)]'
    '(threads)--sort=[sort results in ascending order (buffers results; higher memory)]:sort method:((
    '(threads)--sortr=[sort results in descending order (buffers results; higher memory)]:sort method:((
    '*'{-T+,--type-not=}"[don't search files matching specified file type]: :_rg_types"
    '*'{-g+,--glob=}'[include/exclude files matching specified glob]:glob'
    '*'{-t+,--type=}'[only search files matching specified type]: :_rg_types'
    '*'{-u,--unrestricted}'[reduce level of "smart" searching]'
    '*--colors=[specify color and style settings]: :->colorspec'
```
