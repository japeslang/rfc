# Japes Request for Comments

This repository manages the Request for Comments (RFC) process in the Japes Programming Language. RFCs are the mechanism by which major language changes are made and are a way to solicit feedback and suggestions from the community.

## Licensing

To preserve both the authority and accessibility of the Japes Requests for Comments (RFC), a triple-licensing approach is used in this repository. When the assets involved are source code (including metacode such as BNF), you may either choose the [GNU General Public License version 3](GPLv3.txt) (GPLv3) with the [Classpath Exception](claspath.md) or the [MIT License](MIT.txt) except when that code may be found in the `/src` subdirectory. Code from the `/src` subdirectory is exclusively licensed under the GPLv3 with the Classpath Exception. All non-code works in this repository are licensed under the [Creative Commons 4.0 BY-ND](CC_BY_ND.txt) license.

## Applicability of RFC 1

Like in Marbury v. Madison, the first RFC must somehow gain its own legitimacy. RFC 1 shall become binding whenever it has been merged into [ratified/0001/](ratified/0001/README.md) from a pull request. RFC 1 shall specifically relate to the procedure by which RFCs are handled. RFC 1 is self-executing; after that, policy may only be modified through the RFC process.

## Directory Structure

The RFC repository has the following structure:

- `ratified/` - the index of ratified RFCs.
	- */^[0-9]{4}$/* - A directory containing the contents of the RFC of that accession. Unless amended, it is binding.
	- `history.rfc` - The RFC ledger used to track the publication history of ratified RFCs.
	- `history.rsd` - The initial seed, set to the contents of RFC 1.
- `draft` - the index of draft RFC proposals.
	- *github-user*/ - Draft RFC proposals belonging to the indicated user. Its subdirectories indicate names of working proposals.
- `src` - Utility source code. It is licensed under the GPLv3.