---
layout: page
title: Privacy Policy
description: How Plenty handles personal data on plenty.is and in its apps.
permalink: /privacy/
---

# Privacy policy

{: .lede}
Plenty collects as little as it can. This site sets no cookies, and Plenty's desktop apps and Omarchy plugins send nothing to Plenty unless this page says so.

Last updated: 20 October 2026

## Who is responsible

PlentyLabs UG (haftungsbeschränkt) & Co. KG<br>
Brunnenstraße 169<br>
10119 Berlin, Germany<br>
E-Mail: [hello@plenty.is](mailto:hello@plenty.is)

More details are in the [imprint](/imprint/). Write to the address above about anything on this page.

## This website

**Hosting.** plenty.is is hosted on GitHub Pages by GitHub, Inc., 88 Colin P. Kelly Jr. Street, San Francisco, CA 94107, USA. To deliver a page, GitHub's servers receive your IP address, the page you ask for, your browser's user agent, and the referring page, and GitHub may keep them in its server logs for security. See [GitHub's privacy statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement). GitHub is certified under the EU-U.S. Data Privacy Framework. The legal basis is our legitimate interest in running the site (Art. 6(1)(f) GDPR).

**Statistics.** The site counts visits with [Plausible](https://plausible.io) Community Edition, which Plenty runs itself at stats.paolino.me on a server rented from Hetzner in Helsinki, Finland. No data goes to Plausible the company or anyone else. Plausible sets no cookies and does not follow you across sites. It records the page, the referring site, your browser, operating system, device type, and country. Your IP address is not stored: Plausible uses it, with your user agent and a salt that changes every day, to count unique visitors for that day, and the country is looked up on the same server. The legal basis is our legitimate interest in knowing which pages people read (Art. 6(1)(f) GDPR). The project sites for Spotifast, ZapFast, TonePush, hyprmoncfg, and Cluster Headache Tracker use the same server.

**Fonts.** The fonts are served from plenty.is itself. Your browser does not contact Google Fonts or any other font service.

**Email.** If you write to hello@plenty.is, Plenty keeps your message and address to answer you, and for as long as the conversation needs (Art. 6(1)(b) or (f) GDPR). Plenty's email is hosted by HEY (37signals, LLC, USA).

**Links.** Links to GitHub, the apps' own sites, and other sites take you to services with their own privacy policies.

## Apps with their own privacy policy

- Chat with Work: [chatwithwork.com/privacy-policy](https://chatwithwork.com/privacy-policy)
- Solco: [getsolco.com/privacy](https://getsolco.com/privacy)
- Spotifast: [spotifast.rocks/privacy](https://spotifast.rocks/privacy/)
- Cluster Headache Tracker: [clusterheadachetracker.com/privacy-policy](https://clusterheadachetracker.com/privacy-policy)

## Calendar for Omarchy and Google sign-in

[Calendar for Omarchy](https://github.com/crmne/omarchy-calendar) runs on your computer. It has no server, and it sends nothing to Plenty.

**Google Calendar.** The plugin signs in to Google through the [Google Workspace CLI](https://github.com/googleworkspace/cli) (`gws`) and an OAuth client in a Google Cloud project, either your own or Plenty's, which appears on Google's consent screen as "gws". It uses the Google Calendar scope (`https://www.googleapis.com/auth/calendar`) to read your calendar list and events, and, only when you create, edit, move, or delete an event, to write that change. Requests go straight from your computer to Google. The tokens stay in gws's own encrypted store on your computer, and the plugin holds them in memory only while it talks to Google. It saves no Google events on disk. Events go to Google with invitation emails turned off. Plenty never receives your Google data or your tokens, even when you sign in through Plenty's OAuth client. You can revoke access at any time in your [Google Account](https://myaccount.google.com/permissions).

Calendar for Omarchy's use of information received from Google APIs adheres to the [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy), including the Limited Use requirements.

**Other calendars.** HEY calendars go through HEY's own command-line tool and API. Calendar feeds you add are fetched from their addresses over HTTPS, and the addresses are saved in `~/.config/omacal/feeds.json` on your computer.

**Place suggestions.** While you type a place for an event, the plugin sends what you typed, your language, and the location of your time zone's city to [Photon](https://photon.komoot.io) by komoot, or to Google Places if you add your own Maps key. You can turn place suggestions off in its settings.

## Other apps and Omarchy plugins

None of these send anything to Plenty unless noted. Where they reach other services, those services see your IP address and what is listed.

- **ZapFast** talks to WhatsApp to send and receive your messages. GIF search sends your search text to GIPHY. Importing a Signal sticker pack fetches it from Signal. It checks GitHub for new releases, which you can turn off.
- **TonePush** (the desktop editor) loads and publishes tones through tonepush.rocks and checks GitHub for new releases. It sends crash reports only if you agree, when it asks or in its settings. A report holds where in the code it failed, the app's version, your operating system, and file paths with your home folder hidden. They go to Plenty's own error tracker on its server at Hetzner in Germany, which opens an issue in TonePush's public GitHub repository naming only where in the code it failed and how often.
- **The TonePush website** (tonepush.rocks) runs on Plenty's server at Hetzner in Germany. If you sign up, it keeps your email address, name, the tones and setlists you publish, and, for each sign-in, your IP address and browser. Sign-in links are sent by email. Error reports go to Plenty's own error tracker on the same server, where a report can include your account's id, email address, and name. The tracker files a summary of each error as an issue in Plenty's private GitHub repository, without your account details. Plenty keeps your account until you ask for it to be deleted.
- **OmaTasks for Todoist** talks to Todoist's API with your Todoist token, which it keeps in `~/.config/omarchy-todoist/token`.
- **Ultimate Guitar Tabs** searches Ultimate Guitar for the artist and title of the song that's playing.
- **Lyrics Synced with Music** looks up the playing song's artist, title, album, and length on [LRCLIB](https://lrclib.net).
- **OmaStats** shows your public IP address by asking api.ipify.org, then icanhazip.com or ifconfig.me if that fails. It does this while its Network page is open, at most every ten minutes. You can turn it off in its settings.
- **Media Controls + Album Art**, like the plugins above, shows the cover art your music player names, which can mean loading it from the player's service.
- **Omarchy Rescue** checks that it's online by contacting pkgs.omarchy.org. The coding agents it includes talk to their own providers once you sign in to them.
- **Files for Omarchy, MOZA for Omarchy, hyprmoncfg, hyprmoncfg for Omarchy, and Active Window + Icon** make no network requests.

## How long data is kept

Plausible's visit records hold no IP address and are kept to compare traffic over time. Emails are kept as long as the conversation needs. GitHub's and Hetzner's own logs follow their policies.

## Your rights

Under the GDPR you can ask what personal data Plenty has about you (Art. 15), and have it corrected (Art. 16), deleted (Art. 17), or restricted (Art. 18). You can ask for it in a portable format (Art. 20), and object to processing based on legitimate interest (Art. 21). Write to [hello@plenty.is](mailto:hello@plenty.is).

You can also complain to a data protection authority. Plenty's is the Berliner Beauftragte für Datenschutz und Informationsfreiheit, Alt-Moabit 59–61, 10555 Berlin, [datenschutz-berlin.de](https://www.datenschutz-berlin.de).

## Changes

When Plenty changes what it collects, this page changes with it, and the date above.
