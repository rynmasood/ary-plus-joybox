# ARY Plus for the Nayatel JoyBox (Not Google Certified)

A small Android TV app that plays ARY Plus, built for one specific box: the **Nayatel JoyBox**.

Browse the catalogue, search it, and watch — with a remote control, on a television, the way it is
supposed to work. It is **4.3 MB** and starts in about a fifth of a second.

---

## Why this exists

ARY Plus already has a website, and the JoyBox can't open it. The problem is what happens next.

The box runs Android 6.0.1, and its built-in web browser is **Chromium 44 — an engine from 2015**.
That is old enough that it cannot run the ARY Plus website at all: the page loads technically in the background, but the video does
not. It is not a settings problem, and it is not something you can update, because the browser on
this box is part of the firmware. There is no app store entry for it and no way to replace it.

So on this box, the website route is closed. That is the entire reason this app exists — not to add
features, but to get the video playing at all.


---

## What it solves

**It plays video on a box that otherwise cannot.** That is the headline. Everything else follows.

| | |
|---|---|
| **Browse** | The home screen, with the same rows you see on the website — Latest, Dramas, Movies, genres and so on |
| **Search** | With a keyboard drawn inside the app, so you type with the remote instead of fighting an on-screen one |
| **Play** | Full playback controls: play/pause, skip back and forward 10 seconds, and a draggable progress bar |
| **Picture quality** | Defaults to 1080p, with a menu to drop to 720p or lower if your connection struggles |
| **Subtitles** | Off by default, with one button to turn them on — and only ever in English |
| **Skip intro** | Jumps past the opening titles, using the timing the service itself provides |
| **Next episode** | Finishes one episode and rolls straight into the next |
| **Films** | Films get a **Watch now** button, and their trailers play when a film cannot |

Remote control behaviour is the part that matters most on a television and is the part usually done
badly. Arrow keys move between things properly, everything you can select lights up, and the
controls get out of the way while you watch.

---

## What it can't do on the JoyBox

Worth being straight about, because these are limits of the box rather than of the app.

### Some films won't play

The service copy-protects part of its film catalogue. Playing those needs a feature that Android
only gained in **Android 7.0**, and the JoyBox runs **Android 6.0.1**. The app cannot work around
this, and neither can any other app on the same box — including the official one.

In practice: of every film on the service, **96 of 109 play normally**. The remaining **13** cannot,
and the app tells you so rather than showing you a button that fails. Where a trailer exists — and
for 7 of those 13 it does — you get a **Watch trailer** button instead.

You will see this most on the **MOVIES** row, which is almost entirely copy-protected. The
**Telefilms** and film-festival rows are unaffected and play fine.

### Live channels aren't built yet

The service carries live channels and live sports, and the app does not play them. This is a
deliberate omission rather than an oversight — live playback is a different problem from
on-demand playback, and it was left out so the on-demand side could be made solid first.

### It is limited by the box's age

The JoyBox is a 2016 device with about **1 GB of memory** and a 1080p output. The app is written
specifically for that — it deliberately avoids modern UI toolkits that would use more memory than
the app itself. It runs well there, and it will not look any better on newer hardware than the box
allows

If you have flaky internet, use the quality menu. 1080p is the default, but dropping to 720p or
480p will usually keep playback smooth where 1080p stutters.



### It depends on something that can change without warning

This app talks to the service's own servers rather than to the website. That is what makes it fast,
and it is also the risk: that interface is private and undocumented, so the service can change it
at any time and this app would stop working. A browser-based version would be slower and larger,
but it would survive such a change.

---

## Installing

The built app is in the Release Section.

1. Download that file and copy it to a **USB stick**.
2. Plug the stick into the JoyBox and open it with the box's file manager.
3. Select the file and install it.

The box will warn you about installing apps from outside the Play Store. That is expected — allow
it for this one file.

There is nothing to configure. The app needs no account, no login, and no key of your own.

---

## A note on what this is

This is an independent app. It is not made by, endorsed by, or connected to ARY or Nayatel. It uses
the same public service the website uses, and it is for personal use on your own box.

It was built to solve one problem on one device. If it works on yours, good — but that is what it
was made for.
