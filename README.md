# chess.js fork for CWDA

Original library: https://github.com/jhlywa/chess.js

> chess.js is a Javascript chess library that is used for chess move generation/validation, piece placement/movement, and check/checkmate/stalemate detection - basically everything but the AI.
>
> chess.js has been extensively tested in node.js and most modern browsers.

This fork aims to support Chess With Different Armies.

TODO

- look for hard-coded piece.type -- i think the only other relevant place is attacked() (i.e. places where pieces' logic is not just in PIECE\_OFFSETS and ATTACKED)
- understand ATTACKED and RAYS -- looks like PIECE\_OFFSETS is used for movement, but ATTACKS is used (at least) to check if king can go to a square. perhaps ATTACKED is merely a performance optimization. can i just use PIECE\_OFFSETS for this?
- figure out how to implement short rook, if possible
- figure out how to implement colorbound castling, if possible
- create my own proper fork of this library maybe?
