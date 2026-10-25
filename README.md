# simkit-website

Hosts SimKit's direct-download releases (GitHub Releases, `SimKit.dmg`) and the Sparkle
appcast that installed apps read at `https://ealtaca.github.io/simkit-website/appcast.xml`.
The App Store listing's privacy policy also links here.

The website itself is [ealtaca/simkit-site](https://github.com/ealtaca/simkit-site), served at
https://simkit.dev. This repo must not get a custom domain: GitHub would then redirect the
appcast to `http://`, and apps refuse that redirect.
