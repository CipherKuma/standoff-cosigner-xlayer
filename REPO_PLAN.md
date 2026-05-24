# REPO PLAN

Updated 2026-05-22 — repo migrated from `gabrielantonyxaviour` to `CipherKuma` per `/Users/gabrielantonyxaviour/Documents/hackathons/PERSONA_ALLOCATION.md`.

## Repository (current)

- Owner: `CipherKuma`
- Repo name: `standoff-cosigner-xlayer`
- URL: `https://github.com/CipherKuma/standoff-cosigner-xlayer`
- Visibility: public

## Owner Verification

- `gh auth status` shows `CipherKuma` token in keyring with scopes `gist, read:org, repo`.
- Switch active account via `gh auth switch --user CipherKuma`.
- Cipher Kuma is the assigned persona per `submission-profile-registry.json` (Chrome `Profile 9`, `jedionchain@gmail.com`).

## Creation Method

GitHub CLI: switch active account to `CipherKuma`, then `gh repo create CipherKuma/standoff-cosigner-xlayer --public --source=. --remote=origin --push`. No PAT fetch required.

## Migration Path

1. Update `TEAM.md` + `REPO_PLAN.md` to Cipher Kuma persona. Done.
2. `gh auth switch --user CipherKuma`.
3. `gh repo create CipherKuma/standoff-cosigner-xlayer --public`.
4. `git remote set-url origin https://github.com/CipherKuma/standoff-cosigner-xlayer.git`.
5. `git push -u origin main`.
6. `gh auth switch --user gabrielantonyxaviour` and archive (or rename) the old `gabrielantonyxaviour/standoff-cosigner-xlayer` repo. Cipher Kuma token does not carry `delete_repo`; archiving is the chosen disposition.

## Status

- URL: `https://github.com/CipherKuma/standoff-cosigner-xlayer` (after migration)
- Visibility: public
- Final documentation/report commits are pushed on `main`.
