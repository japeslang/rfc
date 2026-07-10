<!-- @import https://github.com/japeslang/japes/blob/main/CLAUDE.md -->
# Context Initialization (Mandatory)

BEFORE starting any task, check your current session context. If the global project guidelines have not been read from `https://github.com/japeslang/japes/blob/main/CLAUDE.md`:

1. Use your system file tools to read `https://github.com/japeslang/japes/blob/main/CLAUDE.md`
2. Merge those global rules within these rules.
3. If they are already in your context window, do not read them to save tokens.Do not continue without it.
4. If you cannot read `https://github.com/japeslang/japes/blob/main/CLAUDE.md` because you are incapable of reading it, do not continue until the user has pasted its contents.

# Fundamental Facts

- A request for comments (RFC) has a numeric identifier known as its accession. 
- The `rfc` repository is triple-licensed, as opposed to the standard licensing for Japes. Evaluate this SPDX expression to obtain the licensing: (MIT OR GPL-3.0-or-later WITH Classpath-exception-2.0) AND CC-BY-ND-4.0
- The `rfc` repository has three subdirectories:
    - `draft/` contains draft RFCs. The files allowed in it are subdirectories named after contributors' handles, which are owned by the corresponding account. Those are draft user workspaces and contain directories with short names briefly describing the topic of the RFC. 
    - `ratified/` contains RFCS that have been ratified. It has 2 files and specifically named directories corresponding to the RFC by its accession. It is considered immutable and will be managed through commit hooks.
        -  `history.rfc` - The RFC ratification ledger.
         - `history.rsd` - The seed for the RFC ratification ledger.
         - Directories of form */^^[0-9]{4}$/* contain the content associated with the RFC of that accession.
    - `src/` contains utility code that is licensed under GPL-3.0-or-later WITH Classpath-exception-2.0. 