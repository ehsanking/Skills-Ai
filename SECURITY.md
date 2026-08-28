# Security Policy

The short version. The app needs no account. It asks Android for internet, and — only if you sign in and choose to — for permission to show notifications. There is no advertising identifier, no device identifier, no analytics SDK and no third-party tracker in it. Usage statistics are off unless you turn them on.

Browsing and searching do reach our server, so that a skill added today can be found today; the table below says exactly what those requests carry. With no connection the app falls back to the copy it ships with and keeps working. If you never sign in, we hold no account that identifies you.

Who is responsible
Skills AI is run by an individual developer, not a company. The servers are operated by Hetzner in Germany. Wherever you are reading this, your requests reach a machine in the European Union, and this service is run under European data-protection rules.

What the app sends without asking
Only what is needed to draw a screen you opened:

When	What is sent	Why
The home screen loads	A request for the sponsored slots and the tool list. No identifier of any kind is attached.	To show current ads and a current catalogue
You open a tool or a skill	Which tool or skill you asked for, and your interface language for the description	To fetch the newest version of that text
You search	The words you typed	Search runs on the server so that skills added today can be found today. The app also has an offline index and falls back to it when there is no network.
None of these requests carries a name, an account, a device identifier or a cookie. What our web server records for them is described under Server logs below.

Usage statistics — off by default
In Settings there is a switch called Share usage statistics. It is off when you install the app. If you turn it on, then once a day the app sends:

a random identifier that the app generated on your device — not your device ID, not your advertising ID, and not derived from anything about your phone;
your interface language, your app build and your Android version;
which content version you have, and a count of how many times each skill was opened.
That is the whole payload. There is a button beside the switch — Forget this installation — that throws the random identifier away and makes a new one, which severs the link to everything sent before it.

On our side that identifier is stored only as a salted hash, no IP address is written to the database, and the per-skill counts are not linked to any installation.

If you sign in
Signing in is only needed for the community and for publishing. Everything else works without it.

You sign in through Google or GitHub. We never see your password. The provider tells us three things and we store them: your name, your email address, and the URL of your profile picture. We also store which provider you used and that provider's ID for you. We do not keep the provider's access token — it is used once, to ask who you are, and then discarded.

We issue our own sign-in token for the app. Only a SHA-256 hash of it is stored, so a copy of our database does not contain a working credential.

Notifications
The app can tell you when somebody replies to you, likes what you wrote, reports that one of your published skills worked, or when a moderator takes something of yours down. All of that happens inside the app whether or not you allow anything: the list is on the notifications screen and the count is on the bell.

If you are signed in and you allow it, the same notifications also reach your phone while the app is closed. Android asks you first, and refusing changes nothing else — every other part of the app behaves exactly as before.

Delivering them uses Google's Firebase Cloud Messaging, because on Android that is how a push is delivered. Google therefore handles the moment of delivery and sees the short line that appears on your screen. To address it we store one thing: the registration token Google issues to your installation, together with your phone's language and the build of the app — the language so the notification arrives in it, the build so a fault can be tied to a version.

That token identifies an installation, not a person. It is not your device identifier and not an advertising identifier; the app carries neither. Google rotates it on its own schedule, reinstalling the app replaces it, and signing out deletes it here at once.

A phone without Google Play Services receives no push at all, and nothing else about the app changes. That is why notifications were built as a screen first and a push second.

What you publish
Posts, replies, likes, published skills and your profile are public. They are shown to anyone using the app, signed in or not, next to your name and picture. Treat anything you write there as published.

When you answer "did it work?" on a skill, your answer is counted into a public total. The total is public; which way you personally answered is shown only to you.

If you report something, we record that you reported it, so that ten reports from one account cannot look like ten people objecting.

What never leaves your device
Your favourites
Which tools you have pinned
Your language and theme choices
The count of skills you have opened, while statistics are off
Server logs
Like every web server, ours records each request: the IP address, the time, the path, the response code and the user-agent string. These logs are kept for 14 days and then deleted automatically. They are used to find faults and abuse, and for nothing else.

Counting visitors to this website
This website — not the app — keeps a daily count of how many people reached it, so that the person running it can tell whether anybody is there. No cookie is added for counting, and nothing about you is stored: not your address, not your browser string.

Each day the server makes a random secret, combines it with your address, your browser string and the id of the session cookie this site already sets for signing in and for form security, and keeps only the one-way result. That is what makes it a count of people rather than of page loads. The secret is different every day and destroyed after two days, so the same visitor cannot be recognised from one day to the next, and once it is gone no address in the world can be matched against what was kept. What remains is a number per day.

Beside it, for a few minutes at a time, we keep the fact that somebody is here — that is the “online now” figure and nothing more. If your browser sends DNT: 1 or Sec-GPC: 1, you are not counted at all. None of this is shared with anyone, and no third-party analytics service is used.

Who else gets your data
Nobody, in the sense people usually mean: we sell nothing, share nothing with advertisers, and run no analytics service. Three parties are unavoidably involved:

Hetzner, who run the server the data sits on.
Google or GitHub, but only if you choose to sign in with them — and they learn only that you signed in to this app.
Your profile picture is loaded from the provider's own servers when it is shown, so they can see that it was displayed.
Google again, separately, if you turn notifications on: every push is delivered by them, so they see the registration token and the one line it carries.
Your rights, and how to use them
You can ask for a copy of what we hold about you, ask for it to be corrected, or ask for it to be deleted. Email us from the address on your account and you will get an answer within 30 days.

Deleting your account removes your profile, your email address, your picture URL and your sign-in tokens. Tell us in the same message whether you want what you published removed as well or left in place without your name attached — replies written by other people around it stay either way.

You can stop almost everything without asking us: turn statistics off, do not sign in, or use the app in aeroplane mode, where it still works.

Children
This app is not intended for children. You must be at least 16 to create an account, or the minimum age set by your own country if it is lower. If we learn an account belongs to someone younger, we delete it.

Changes
If this policy changes in a way that matters, the date at the top changes and the app will say so before you next post. Small corrections are made quietly and the date still moves.
