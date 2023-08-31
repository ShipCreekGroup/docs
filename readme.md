EDIT: This isn't gonna work, since the contents aren't __really__ encrypted, they are just placed under hashed file names.
So someone could just look through this source code (which has to be public for GH pages to work)
and they will be able to find the content (under weird directory names, but still...) :facepalm:

Hosts the password-protected docs.

In a different, private repo:
1. Generate site using mkdocs
2. Build encrypted version using https://github.com/matteobrusa/Password-protection-for-static-pages to statically.
  We can't host from here becaus egithub doesn't allow hosting GitHub Pages from a private repo.
3. Push the encrypted version to this repo using https://github.com/cpina/github-action-push-to-another-repository
4. The encypted version is hosted via github pages
