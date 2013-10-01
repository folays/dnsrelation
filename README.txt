FORMAT v1

_OWNER._relation	IN	TXT	"v=RELATION1; name=RELATIVE; weight=PRIORITY; status=RELATIONSHIP; peerdomain=DOMAIN"

v=RELATION<n> : version of the DNS Relation Protocol
name=<RELATIVE> : name of the relative person
weight=<PRIORITY> : priority of the relative person, hightest priority win. zero is neutral, while the most negative means the most disliked.
status=<RELATIONSHIP> : relationship status. friend, girl/boy friend, parent, ...
peerdomain=<DOMAIN> : RELATIVE._relation.DOMAIN must point to a Relation DNS Entry pointing to you

FORMAT v1.1

Addition of the "delegate=DOMAIN" option.
Only usable with format v1.1+, and if delegate=DOMAIN is present, no others options are considered.

Example: _OWNER._relation      IN TXT "v=RELATION1.1; delegate=DOMAIN"
