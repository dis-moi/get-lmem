# LMEM install dispatcher website

This website provides convenient URLs to redirect users to proper store.

- https://get.lmem.net/firefox redirects to the Firefox LMEM addon page on addons.mozilla.org.
- https://get.lmem.net/chrome redirects to the Chromium LMEM extesion page on the Chrome Web Store.
- So on so forth...

## How to edit the redirected URL for a given platform (from Github Web UI)

1. Open the corresponding file (i.e. `firefox.html` for Firefox).
2. Edit the 4th line: 
```html
<script>
  var redirectUrl = 'https://addons.mozilla.org/fr-FR/firefox/addon/lmem/';
</script>
```
3. Commit Changes creating a new branch.
4. Submit the pull request.
5. Request approval.
6. Merge the pull request.
7. Remove the stale branch.

Then, the new URL is automatically deployed.

**N.B.** You must [sign your commit](https://help.github.com/articles/associating-an-email-with-your-gpg-key/).
