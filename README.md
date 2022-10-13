# Protecting your email address via SVG instead of JS
Email addresses published on webpages usually need to be protected from email-harvesting spambots.

Conventionally, email protection techniques utilise a combination of **HTML**, **CSS** and **JS** - though each approach is subject to its own pros and cons.

In general, approaches involving **JS** tend to be more sophisticated than alternatives based on **HTML** and / or **CSS**.

But the downside is that **JS** then becomes an unavoidable dependency of that page.

We should consider the school of thought which advocates that while JS may enhance pages, ideally we should want those pages to work even when JavaScript is turned off.

_____

The technique detailed on this page comes from an entirely different place. It's different from all conventional email protection techniques.

Because it's based on **SVG**.

**N.B.** *This technique - and any other email-protection technique utilising front-end-technologies - **won't** protect your published email address from being harvested by the most determined and sophisticated spambots. But like many JS-based email-protection techniques, it will still protect you from a great many unsophisticated harvesters, keeping your email successfully hidden from any simple or amateurish scripts seeking to trawl the web, locating and copying any unprotected email addresses they find.*

_____

## Three advantages of an SVG-based approach to protecting email addresses

### 1. Works with JavaScript turned off
The main advantage of this **SVG-based approach** to protecting emails, is that it involves **no JavaScript**.

As such, even when a human visitor has their JavaScript turned off, the email address displayed on the page remains usable, accessible and protected, while remaining secure and hidden from spambots.

### 2. Permits a standard `mailto:` link
Unlike other no-JavaScript-required approaches (e.g. obfuscating email addresses by inserting non-visible HTML Comments or inserting visible elements and subsequently hiding them via CSS), this **SVG-based approach** allows for standard `mailto:` links. The twist is: the `mailto:` link exists inside the external SVG document, not inside the referring HTML document.

### 3. Conceals content like an image; Copyable like text

A third advantage is that embedded **SVGs** are *image-like* but *not* images.

As replaced elements embedded within a hypertext document, **SVGs** may conceal an email address from spambots nearly as effectively as an image might. 

But, strictly, **SVGs** are *graphics documents* rather than actual images.

Consequently, *unlike with an image*, a human visitor may still copy the email address by right-clicking on the embedded **SVG**.

This would not be possible with a conventional image.

