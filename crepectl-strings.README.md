# crepectl-strings.txt

Raw `strings` output extracted from the `crepectl` binary shipped inside
`/Applications/Cursor.app/Contents/Resources/app/resources/helpers/crepectl`.

This dump contains:

- Self-description and CLI help text from `clap` (the binary's argument parser)
- Rust panic / `assertion failed` strings from `regex-automata`, `gix-*`,
  `aho-corasick`, `clap_builder`, `bstr`, and other crate dependencies
- Build-machine paths under `/Users/runner/.cargo/...` that leak the upstream
  crate versions (gitoxide `4cac37e`, aho-corasick `1.1.4`, clap_builder
  `4.6.0`, regex_lex `1.1.0`, anstyle `1.0.14`, anstream `1.0.0`,
  anyhow `1.0.102`, arc-swap `1.9.1`, bstr `1.12.1`, bytesize `2.3.1`)
- `Crepe` crate source paths: `crates/crepe/src/bin/crepectl.rs`
- Key flags such as `WORKTREE` and `COMMIT` and the `Build a fresh index from
  a git commit` help blurb

## Raw content

```text
       ' existsAnyValueargument'; only  (bytes segment_resourceRefStoreDiscoverFullNamecrepectlWORKTREErequiredx-cp1250ksc_5601x-cp1251iso88591csgb2312x-cp1252iso88592x-cp1253iso88593ecma-114x-cp1254iso88594x-cp1255iso88595x-x-big5x-cp1256csibm866iso88596x-cp1257iso88597asmo-708ecma-118elot_928x-cp1258iso88598iso88599utf-16beutf-16leus-asciims_kanjix-euc-jpUTF-16BEUTF-16LEinteger externalskipHashNO_PROXYMetadatauseStdevallProxyno_proxypathspecgitoxideworktreefileModesymlinkssafecrlfautocrlfWorktreeBranch 'value_idutf8_err@
  AZ09AFaftried to unwrap expr from HirFrame, got: tried to unwrap group from HirFrame, got: tried to unwrap repetition from HirFrame, got: tried to unwrap byte class from HirFrame, got: tried to unwrap Unicode class from HirFrame, got: tried to unwrap alt pipe from HirFrame, got: multi_linedot_matches_new_lineswap_greedunicodeFlagsLiteralClassUnicodeClassBytesRepetitionGroupold_flagsConcatAlternationAlternationBranch (exhausted)
 ( (MW)SN/A/assertion failed: self.state.uncompiled[last].last.is_none()non-empty nodesassertion failed: prefix_len < ranges.len()assertion failed: self.state.uncompiled[0].last.is_none()Allinternal error: entered unreachable code: found impossible error in meta engine: assertion failed: stack.is_empty()could not find NUL terminated label at start of serialized objectcould not find properly sized label at start of serialized objectversionno quit in start without look-behindassertion failed: id.is_match()no in-progress search to finishno in-progress search to updateinternal error: entered unreachable code: sid being unknown is a bugerror parsing pattern error building NFAStateIDErrorGenericmsgBufferTooSmallInvalidUsizeVersionMismatchfoundEndianMismatchAlignmentMismatchalignmentaddressLabelMismatchArithmeticOverflowUnicodeWordBoundaryErroraccelerators lengthacceleratorsaccelerator bytes cannot have length more than 3acceleratoraccelerator already contains Finderneedlebyte slice lengths must be less than usize MAXslot table length doesn't overflowinternal error: entered unreachable code: expected literal, got internal error: entered unreachable code: expected literal or concat, got  exceeds capacity of ParseTranslateDFAEngineReverseDFAHybridEnginePikeVMEngineOnePassEngineReverseHybridEngineBoundedBacktrackerEngineexpected number of patterns to match pattern IDinvalid accelerator index cannot find with empty needlesinvalid needles length: unrecognized start kindinvalid match spaninternal error: entered unreachable code: suffix match plus reverse match implies there must be a matchreverse search must match if forward search doesforward and reverse search must match same patternassertion failed: start.offset() <= end.offset()internal error: entered unreachable code: ReverseInner always has a DFAinternal error: entered unreachable code: ReverseSuffix always has a DFAinternal error: entered unreachable code: ReverseAnchored always has a DFAinvalid span  for haystack of length Ownedrabinkarpsearch_kindminimum_lennfarevpikevmbacktrackonepasshybriddfaTeddyRabinKarpRegexInfoHybridPikeVMOnePassMatchErrorbucketshash_2powPrefilteris_fastmax_needle_lenPregroup_infoReverseInnerReverseSuffixReverseHybridanchored_acGroupInfoErrorReverseAnchoredMemchrMemmemfinderMemchr2Memchr3BoundedBacktrackerAhoCorasickacshould find a matchcannot create iterator for StateID when number of elements exceed cannot create iterator for PatternID when number of elements exceed sparse set capacity cannot exceed 
 cannot be represented as integer cannot be represented as `usize`cannot use sign for unsigned integerthreadsGIT_PROTOCOL_FROM_USER is either unset or as the value '1'GIT_SSH_VARIANTvariantGIT_EXTERNAL_DIFFGIT_SSL_VERSIONsslVersionlowSpeedTimelowSpeedLimitGIT_SSL_CAINFOsslCAInfoalso used to skip the hash when reading, even if a hash exists in the index fileGIT_HTTP_LOW_SPEED_LIMITGIT_HTTP_LOW_SPEED_TIMEGIT_HTTP_USER_AGENThttps_proxyALL_PROXYGIT_COMMITTER_DATEcommitterDateGIT_AUTHOR_DATEauthorDatestatically known valid section namestatically known to be validfrom 
 commitsIncludeshome dir as UTF8encodingRealpathReadLinkLoadPackTooShort' failednon zeroOverflowNotExistOutdatedRelativereftableReftableAsteriskReservedSUDO_UIDasciidoc*.ceylon*.coffee*.config*.[ch]pp*.[ch]xx*.creole*.cshtml*.csproj*.ebuild*.eclass*.livemdgprbuild*.gradle*.groovy*.jinja2gpl[.-]*lilypondmarkdownminified*.min.js*.fsproj*.nimble*.prologprotobuf*.ps1xmlreasonmlrescriptRakefile.profile*.bashrc.zlogoutzprofilesolidity*.svelte*.device*.socket*.target*.thrift*.webidlWithPathancestorAllocErrlook_setcapacityoriginalPatterns, group=CapturesImplicitexpectedCowBytesBorrowedSearcherpatternshash_lenpreinnersearcher
 values required for '' but the argument '' cannot be used with' cannot be used multiple times ' one or more of the other specified argumentsthe following required arguments were not provided:' requires a subcommand but one was not providedsubcommands
 { .. }attempted to finish a map with a partial entryattempted to begin a new map entry without completing the previous one0000000000000000000000000000000000000000000000000000000000000000assertion failed: other > 0assertion failed: noborrowassertion failed: digits < 40NaNinf0.assertion failed: !buf.is_empty()assertion failed: buf[0] > b'0'assertion failed: buf.len() >= maxlen
()reentrant initoverflow in Duration::newWouldBlockassertion failed: edge.height == self.height - 1internal error: entered unreachable code: empty internal nodeassertion failed: self.height > 0assertion failed: src.len() == dst.len()assertion failed: edge.height == self.node.height - 1assertion failed: old_right_len + count <= CAPACITYassertion failed: old_left_len >= countassertion failed: old_left_len + count <= CAPACITYassertion failed: old_right_len >= countassertion failed: match track_edge_idx {
-assertion failed: self.buf.is_empty() || self.buf.len() >= Self::padding()in bounds
-lz--show-origin--name-onlyGIT_CONFIGGIT_DISCOVERY_ACROSS_FILESYSTEMGIT_OBJECT_DIRECTORYGIT_ALTERNATE_OBJECT_DIRECTORIESGIT_COMMON_DIRGIT_DIR/dev/nullGIT_WORK_TREEwe just pushed a componentInvalid escaped value internal error: entered unreachable code: cannot find character that we didn't search forInput must be surrounded by double quotesUnderflowParseIntegerErrorValidationErrorinputUnexpected end of inputInvalid octal escape valueUnexpected end of input when fetching two more octal bytesIsAbsoluteContainsInvalidComponentIllegalUtf8Illegal use of reserved Windows device name in "HEAD is valid namepacked-refsoperationApiEmptyTableRefnameEntryTooBig
..debug_abbrev.dwo.debug_cu_index.debug_info.dwo.debug_line.dwo.debug_loc.dwo.debug_loclists.dwo.debug_rnglists.dwo.debug_str.dwo.debug_str_offsets.dwo.debug_tu_indexfailed to create whole treestream did not contain valid UTF-8internal error: entered unreachable codeOsErrorCustomerrorpermission deniedconnection refusednetwork unreachableconnection abortednot connectedaddress in useaddress not availablenetwork downbroken pipeentity already existsoperation would blocknot a directoryis a directorydirectory not emptyread-only filesystem or storage mediumfilesystem loop or indirection limit (e.g. symlink loop)stale network file handleinvalid input parameterinvalid datatimed outwrite zeroseek on unseekable filequota exceededfile too largeresource busyexecutable file busycross-device link or renametoo many linksargument list too longoperation interruptedunsupportedunexpected end of fileout of memoryin progressother erroruncategorized errorstdoutstderrfailed printing to failed to write the buffered datafatal runtime error: initialization or cleanup bug, aborting
/Users/runner/.cargo/git/checkouts/gitoxide-c5184609f4b57c0c/4cac37e/gix-chunk/src/file/index.rs
/Users/runner/.cargo/git/checkouts/gitoxide-c5184609f4b57c0c/4cac37e/gix-index/src/access/mod.rs
/Users/runner/.cargo/git/checkouts/gitoxide-c5184609f4b57c0c/4cac37e/gix-index/src/decode/entries.rs
/Users/runner/.cargo/git/checkouts/gitoxide-c5184609f4b57c0c/4cac37e/gix-index/src/decode/mod.rs
/Users/runner/.cargo/git/checkouts/gitoxide-c5184609f4b57c0c/4cac37e/gix-index/src/entry/mod.rs
/Users/runner/.cargo/git/checkouts/gitoxide-c5184609f4b57c0c/4cac37e/gix-index/src/extension/decode.rs
/Users/runner/.cargo/git/checkouts/gitoxide-c5184609f4b57c0c/4cac37e/gix-index/src/extension/index_entry_offset_table.rs
/Users/runner/.cargo/git/checkouts/gitoxide-c5184609f4b57c0c/4cac37e/gix-index/src/extension/link.rs
/Users/runner/.cargo/git/checkouts/gitoxide-c5184609f4b57c0c/4cac37e/gix-index/src/extension/resolve_undo.rs
/Users/runner/.cargo/git/checkouts/gitoxide-c5184609f4b57c0c/4cac37e/gix-index/src/extension/tree/decode.rs
/Users/runner/.cargo/git/checkouts/gitoxide-c5184609f4b57c0c/4cac37e/gix-index/src/extension/untracked_cache.rs
/Users/runner/.cargo/git/checkouts/gitoxide-c5184609f4b57c0c/4cac37e/gix-index/src/file/init.rs
/Users/runner/.cargo/git/checkouts/gitoxide-c5184609f4b57c0c/4cac37e/gix-index/src/lib.rs
/Users/runner/.cargo/git/checkouts/gitoxide-c5184609f4b57c0c/4cac37e/gix-odb/src/store_impls/dynamic/load_index.rs
/Users/runner/.cargo/git/checkouts/gitoxide-c5184609f4b57c0c/4cac37e/gix-pack/src/index/access.rs
/Users/runner/.cargo/git/checkouts/gitoxide-c5184609f4b57c0c/4cac37e/gix-pack/src/multi_index/access.rs
/Users/runner/.cargo/git/checkouts/gitoxide-c5184609f4b57c0c/4cac37e/gix-pack/src/multi_index/chain.rs
/Users/runner/.cargo/git/checkouts/gitoxide-c5184609f4b57c0c/4cac37e/gix-pack/src/multi_index/chunk.rs
/Users/runner/.cargo/git/checkouts/gitoxide-c5184609f4b57c0c/4cac37e/gix-pack/src/multi_index/init.rs
/Users/runner/.cargo/git/checkouts/gitoxide-c5184609f4b57c0c/4cac37e/gix-pack/src/multi_index/mod.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/aho-corasick-1.1.4/src/ahocorasick.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/aho-corasick-1.1.4/src/automaton.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/aho-corasick-1.1.4/src/dfa.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/aho-corasick-1.1.4/src/nfa/contiguous.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/aho-corasick-1.1.4/src/nfa/noncontiguous.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/aho-corasick-1.1.4/src/packed/api.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/aho-corasick-1.1.4/src/packed/pattern.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/aho-corasick-1.1.4/src/packed/rabinkarp.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/aho-corasick-1.1.4/src/packed/teddy/generic.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/aho-corasick-1.1.4/src/util/alphabet.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/aho-corasick-1.1.4/src/util/debug.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/aho-corasick-1.1.4/src/util/prefilter.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/aho-corasick-1.1.4/src/util/primitives.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/aho-corasick-1.1.4/src/util/remapper.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/aho-corasick-1.1.4/src/util/search.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/anstream-1.0.0/src/adapter/strip.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/anstyle-1.0.14/src/color.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/anyhow-1.0.102/src/error.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/anyhow-1.0.102/src/fmt.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/arc-swap-1.9.1/src/debt/helping.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/arc-swap-1.9.1/src/debt/list.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/bstr-1.12.1/src/ext_slice.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/bstr-1.12.1/src/ext_vec.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/bstr-1.12.1/src/impls.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/bstr-1.12.1/src/unicode/fsm/whitespace_anchored_fwd.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/bstr-1.12.1/src/unicode/fsm/whitespace_anchored_rev.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/bstr-1.12.1/src/unicode/whitespace.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/bstr-1.12.1/src/utf8.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/bytesize-2.3.1/src/display.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/clap_builder-4.6.0/src/builder/arg.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/clap_builder-4.6.0/src/builder/arg_group.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/clap_builder-4.6.0/src/builder/command.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/clap_builder-4.6.0/src/builder/ext.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/clap_builder-4.6.0/src/error/format.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/clap_builder-4.6.0/src/error/mod.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/clap_builder-4.6.0/src/mkeymap.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/clap_builder-4.6.0/src/output/help_template.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/clap_builder-4.6.0/src/output/usage.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/clap_builder-4.6.0/src/parser/arg_matcher.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/clap_builder-4.6.0/src/parser/error.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/clap_builder-4.6.0/src/parser/features/suggestions.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/clap_builder-4.6.0/src/parser/matches/arg_matches.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/clap_builder-4.6.0/src/parser/matches/matched_arg.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/clap_builder-4.6.0/src/parser/parser.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/clap_builder-4.6.0/src/parser/validator.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/clap_builder-4.6.0/src/util/flat_map.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/clap_builder-4.6.0/src/util/flat_set.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/clap_builder-4.6.0/src/util/graph.rs
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/clap_lex-1.1.0/src/ext.rs
```
