# grew-cards

Hosting for **encrypted cards**.

Every `.html` file here is a card that has been encrypted (AES-256-GCM) before it was
ever uploaded. The key isn't in this repo, isn't in the page, and never reaches GitHub —
it travels in the fragment of the link the card was shared with (the part after `#`),
which browsers don't send to servers.

So there is nothing to read here. Without the link, a card is a few hundred kilobytes of
base64 noise. That's the point: the cards are hosted publicly, but they aren't public.

Cards are built by a private tool that lives elsewhere. This repo is just where the
ciphertext sits so a phone can fetch it over HTTPS.
