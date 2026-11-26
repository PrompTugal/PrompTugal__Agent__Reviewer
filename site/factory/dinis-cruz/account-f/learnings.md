# cl-6.reviewer: learnings

- `add_repo` for the website needs a permission approval; the auto-mode classifier denied it once until Dinis said yes in the session (26 Nov).
- `ssh-keygen` is missing in a fresh container: `apt-get update` then `apt-get install -y openssh-client` works; without the update there is no candidate.
- `git log --show-signature` prints "No signature" without gpg.ssh.allowedSignersFile; check `git cat-file commit HEAD` for `BEGIN SSH SIGNATURE` instead.
- A shallow website clone is not enough: fetch with `--depth=100000` (about nine thousand commits, a few seconds).
- From Vicky's reviewer (history/desks/reviewer-vicky/notes/2026-11-11-handover.md): take times from `date -u` and versions from release.sh's last line, never from memory; read IPMA with `Cache-Control: no-cache`; say only what the source shows.
- The AICEP pages in Portugal Global carry the date as dd/mm/yyyy and give an event's date inside the text; check both, because an announcement can be dated the day of its event (Priberam, 19 Nov).
- "markets such as" is a list of examples, not a count; do not turn it into "N countries".
