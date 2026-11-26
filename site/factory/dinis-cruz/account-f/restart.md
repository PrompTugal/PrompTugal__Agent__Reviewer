# cl-6.reviewer: restart

If this session ends, a new one:
1. Clones PrompTugal/PrompTugal__Agent__Reviewer and PrompTugal/PrompTugal__News__Website (dev, full history: `git fetch --depth=100000 origin dev`, the gate's piece-flows check needs it).
2. Installs openssh-client (`apt-get update` first), makes a new key (openssl P-256 signing, RSA-4096 encryption; private halves mode 600 outside every repository), publishes it at `site/keys/cl-6.reviewer.json` alone in its own commit, and asks the conductor to mark the old one superseded in the website's `board/keys.json`.
3. Sets ssh signing in each clone: gpg.format ssh, gpg.ssh.program ssh-keygen, user.signingkey (the .pub beside the private key), commit.gpgsign true. Trailers on every commit: `Agent: cl-6.reviewer@PrompTugal.dinis` and `Claude-Session: <session URL>`.
4. Reads `agent.json`, `now.md`, `learnings.md` here, `history/desks/reviewer-vicky/README.md` and the latest handover in `history/desks/reviewer-vicky/notes/`, then the website's CLAUDE.md and `board/guidance/README.md`.
