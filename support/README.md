# Abhinav's Hardware Quest — GitHub Pages

A playful, original pixel-art landing page with interactive navigation, a cursor-following cat, selected verifiable Rust PRs, transparent equipment rationale, and configurable donation options. It uses no copyrighted Pokémon images, sprites, or branding.

## Deploy
1. Copy `index.html` and `qr-support.png` into a `support/` folder inside the GitHub Pages repository `paradoxicalguy.github.io`.
2. Commit and push to the publishing branch. Visit `https://paradoxicalguy.github.io/support/` to verify.
3. Test all PR links, mobile presentation, and QR code from a second device before sharing.

## Configure payment
At the very end of `index.html`, locate:
```js
const PAYMENT = { upiId: '', solanaPublicAddress: '64fRz7VPq9a1V7X8RjDhu9eL3Ju2c485X6Dr72GGDbcU', ethereumPublicAddress: '0xB5b40b183A20D7e2FA1600FD584A5617987e6851' };
```
The public Solana and Ethereum addresses supplied by the page owner are prefilled. **Verify both in Phantom before publishing.** Add your public UPI receiving ID when ready. Never publish a seed phrase, secret recovery phrase, private key, API secret, or wallet export. The page validates simple formats, enables copy controls for configured values, and leaves unconfigured controls disabled. Transfers are not verified or collected by this static website.

A UPI ID is not the same as a Google Pay QR image; if you later add a separate payment QR, label it clearly and keep the *page-sharing* QR distinct. Solana is a blockchain network: supporters need to send SOL or Solana-native USDC only using the stated network. Double-check addresses and test with a tiny amount. For UPI, consider a receiving ID that doesn't reveal a personal phone number.

## Customization
- The header/hero uses original SVG pixel artwork and a small original SVG cat.
- Update `supportUrl` in `index.html` and regenerate `qr-support.png` if your actual hosting path changes.
- Replace text for final model, pricing quote, support contact, and funding status when verified.
- The page intentionally contains no laptop photos.
- You can remove the Google Fonts import for zero remote assets; fallback fonts will be used.

## Accuracy & trust
- PRs are linked as selected examples, not total contributions.
- This is not an official Rust Project appeal.
- Do not publish guessed donation totals or use any payment credentials in the HTML.
- This is a static page: there is no payment processing or automatic fundraising progress tracking.

Ethereum card accepts ETH on Ethereum mainnet only; do not imply transfers on other EVM chains are supported.
