# jspiiv.github.io

Proof of control for [Split](https://github.com/JspIIV/split).

`.well-known/split-pledge.txt` holds one thing: the address this domain vouches
for. The Pledge contract fetches it in a consensus round, every validator reads
it independently, and only the address named here can pledge this domain.

The file is deliberately nothing but the address. A file that merely mentions an
address inside a sentence is not a domain vouching for it, and the contract
compares the whole trimmed body rather than looking for a substring.
