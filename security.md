# Security and Privacy

Here are some tips for security and for keeping your data and personal information private.

## Authentication

### Passwords

- Use unique passwords and forget about remembering them: use a password manager!
  - [Bitwarden](https://bitwarden.com/) is open source; multi-platform; multi-browser. This means your passwords are not stuck
    to a particular browser, account, or operating system (Apple Keychain).
    
### Two-factor authentication (2fa)

- Enable two-factor authentication where possible.
- Use an _OTP app_ such as [OTP Auth](https://cooperrs.de/otpauth.html) (iOS/macOS), FreeOTP etc. Prefer open-source as they can be externally scrutinized.
- When activating 2fa you often get a set of _recovery codes_. Keep them in a safe place, preferably offline or printed.
- _Avoid giving your phone number_ for OTPs via SMS. This connects your online identity with real identity.


### Security Key

Security keys such as [YubiKey](www.yubico.com) or the open source [Solokey](https://solokeys.com/) is a convenient and safe way to avoid typing in OTPs as mentioned above.
Far from all sites support this, but they seem to be increasing due to the [WebAuthn](https://en.wikipedia.org/wiki/WebAuthn)
standard. Security keys can also store other information for strong encryption. See [video](https://www.youtube.com/watch?v=aAr41uSC4vs) for some inspiration.

## Privacy

- Your online movements are stored and used to profile you to determine your behavior and views. A VPN may reduce tracking and
  for work, you can use LU's VPN which further gives access to the Library.
  [ProtonVPN](https://protonvpn.com) is a Swiss based alternative.
- Avoid companies that live from your data: Facebook, Google, are prime examples. If you don't, **always log out** of your account.
- Do not use your Google or Facebook login to access other sites.
- Do not let websites store personal information (address, age, phone number etc.). There are countless examples of databreaches where user information
  has been exposed and sold on auctions.
- Never give your personal id number!
- Do not give applications or websites access to your contact list.
- If you believe your privacy is safe just because you use end-to-end encryption in e.g. WhatsApp, [think again!](https://www.globalviews360.com/articles/whatsapps-new-privacy-policy-collecting-metadata-and-its-implications)
- Possible replacements:
  - Google search → [DuckDuckGo](https://duckduckgo.com) or [Startpage](https://www.startpage.com/) (no tracking)
  - Google mail → [ProtonMail](https://protonmail.com) or [Tutanota](https://tutanota.com/)
  - WhatsApp → [Signal.app](https://signal.org) (non-profit, open source, used by Edward Snowden!).
  - Apple Keychain → [Bitwarden](https://bitwarden.com/) (open source, premium service available, ["zero-trust"](https://en.wikipedia.org/wiki/Zero_trust_security_model))
  - Facebook/twitter → [Mastodon](https://joinmastodon.org/) (de-centralized)
  - Browser → [Brave Browser](https://brave.com/) (fights digital fingerprinting)
  - (Large) file sharing → [Syncthing](https://syncthing.net/) (open-source, encrypted, de-centralized)
  - Box/Dropbox → [Mega.io](https://mega.io/) (20 GB free, open-source, end-to-end encrypted, ["zero-trust"](https://en.wikipedia.org/wiki/Zero_trust_security_model))

## More information

This document is only a very brief set of recommendations. For much more information, see _e.g._ EFF's [Surveillance Self Defence Guide](https://ssd.eff.org)
