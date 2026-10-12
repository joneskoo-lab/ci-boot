# ci-boot

Public autoinstall seed for the home Firecracker CI host (Ubuntu Server 26.04 LTS). Public on purpose: no secrets,
keys, tokens, password hashes or internal addresses. The host joins Tailscale interactively (QR code on the console).

Boot the stock Ubuntu Server ISO in UEFI mode, press `e` on "Try or Install Ubuntu Server", add before `---`, press F10:

    autoinstall ds=nocloud\;s=https://raw.githubusercontent.com/joneskoo-lab/ci-boot/main/

It wipes the largest disk without asking. Source of truth: `boot/` in the private `gh-actions` repo.
