# proclaim-modules

Logos module catalog for [proclaim](https://github.com/goldennftplatform-svg/proclaim).

This catalog publishes the signed `registry` module built for LP-0023.
It follows the [`logos-repo.json` / `index.json` catalog format](https://github.com/logos-co/logos-modules-release-tool/blob/main/docs/catalog-format.md).

- Catalog identity: [`logos-repo.json`](logos-repo.json) — add its raw URL to a Logos client's repository list.
- Package listing: [`index.json`](index.json) — generated, binds the release asset by `rootHash` and signer DID.
- Artifact: [registry-0.1.0.lgx](https://github.com/goldennftplatform-svg/proclaim/releases/download/registry-v0.1.0/registry-0.1.0.lgx) (GitHub Release in the `proclaim` repository).

The signer is a self-generated **dev key**. It is listed in `trustedSigners` for
this catalog only; it is not in any Logos-wide trusted keyring. See
`docs/LGX-BUILD.md` in the proclaim repository for build/verification evidence
and honest caveats (lgx CLI rather than `logos-module-builder`, legacy
`type: "ui"`, linux-amd64 only, Basecamp install test pending).
