## Animated curtain menu

> Simple animated landing-page for signor vespa 🛵.

![alt text](./capture.png)

Featuring:

- A single vanilla page with curtain menu animation.
- Making use of HTML `data` attributes toggle activation.
- Images are all from [unsplash](https://unsplash.com/) directly.
- Applying a animation based on body `data` attribute:

```css
body:not([data-nav="true"]) > #nav-toggle:hover > .open {
  opacity: 1;
  transform: translate(-50%, -50%) scale(0.9);
}
body[data-nav="true"] > #nav-toggle {
  background: rgb(81, 164, 164);
}
body[data-nav="true"] > #nav-toggle > .close {
  opacity: 1;
  transform: translate(-50%, -50%) scale(1);
}
body[data-nav="true"] > main {
  transform: translateY(-50%);
}
body[data-nav="true"] > nav > #nav-links {
  transform: translateY(0%) scale(1);
}
```
