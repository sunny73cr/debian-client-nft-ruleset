# debian-client-nft-ruleset
A small (strict) ruleset useful for a debian network client / server. The machine consumes an NTP service, an APT service (HTTP/S), and a DNS service. This ruleset could be augmented by a cron job to (periodically) query addresses of names such as 'deb.debian.org' and 'pool.ntp.org'.

You should note that raw payload expressions not aligned to an 8-bit boundary are modified by NetFilter to do exactly that when the rule is applied.
This makes it especially difficult to confirm validity of the rules that you had written.
Though, please rest assured, the rules generated by this configuration file have been validated, and are correct after application.
