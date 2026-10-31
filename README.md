# check_mk

Portainer stack `check_mk` on ore-dock-103-1, git-backed with auto-update.

The compose uses `${VAR}` placeholders for stack environment values. The
real values live in the Portainer stack environment and in the host `.env`;
they are deliberately NOT committed. See `.env.example` for the keys.

## Update flow

Portainer polls this repo every 15 minutes and redeploys on a new commit.
