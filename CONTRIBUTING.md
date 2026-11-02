# Contributing

Thanks for helping. This is a Tiny Tapeout project built from a Wokwi design.

## Get it running

Clone the repository (the **Code** button on GitHub), then from its folder:

The design itself lives in Wokwi; `info.yaml` names the Wokwi project. Push a branch and the GitHub
Actions workflows fetch the netlist from Wokwi, then build and check the GDS, docs, FPGA bitstream and
the `wokwi_test` simulation. The workflows use Tiny Tapeout's
[tt-support-tools](https://github.com/TinyTapeout/tt-support-tools); see the
[local hardening guide](https://www.tinytapeout.com/guides/local-hardening/) to run them on your own
machine.

## Making a change

- Branch from `prototype` and open the pull request against `prototype`; `main` is what gets installed.
- Never commit real tokens, passwords, keys, IP addresses, Discord IDs, domains, or community, guild,
  channel, server or player names. Use placeholders such as `Example Community`,
  `community.example.org`, `203.0.113.10` and `000000000000000000`.
  CI runs `tools/check_generic.py`, which fails on addresses, IDs and private terms. The public Wokwi ID line in
  `info.yaml` ends with `check_generic: allow`.
- Lowercase filenames with underscores, no spaces.
- Add a line to `CHANGELOG.md` describing the change.

## Security problems

Please don't open a public issue; see [SECURITY.md](SECURITY.md).
