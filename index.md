## About KevinBoucher.com

* [GitHub repository](https://github.com/kboucher/kevinboucher-dot-com)
* [JS Docs](https://kboucher.github.io/jsdoc/index.html)
* [Test coverage](https://kboucher.github.io/coverage/index.html)

### UI Development Principles

* Foster a culture of craftsmanship
* Less is more (let your tools do the work)
* Work harder to write less code

### JavaScript Authoring

It's very difficult to do this topic justice in sound-bytes and bullet points.

### Semantic HTML

Semantic HTML and modular CSS are at the heart of this website and all of the web user interfaces that I write. Practicing semantic HTML authoring is not only an exercise in intentionality, but an effective foundation for ensuring accessibility and usability. Important details often overlooked include:

* Ensuring that interactions are associated with interactive elements
* The value of semantic markup for sight-impaired users
* Using the appropriate interactive elements for the job (including understanding the purpose of links vs. buttons, using the correct form field types to enhance usability, and associating labels with form elements)
* Empowering developers who encounter your code in the future

### Modular CSS

Modular CSS is primarily about organizing both HTML class names and associated style declarations. Again, intentionality is key, and when combined with external front-end libraries like Bootstrap, authored CSS for modern web applications can become quite minimal and easy to update. KevinBoucher.com leverages Bootstrap 5 (via the `ember-bootstrap` addon), BEM (block-element-modifier) selectors, and a very specific file hierarchy that both limits the amount of custom code and eases extensibility in the future.

Key concepts here are:

* Leveraging variable overrides in CSS libraries to minimize the amount of custom CSS
* Organizing files around those library variable overrides, any additional library overrides, SASS placeholders and mixins, element styles, component styles, and custom layouts
* Thinking in terms of logical components/modules
* Mobile-first responsive development

[View the CSS structure for kevinboucher.com](https://github.com/kboucher/kevinboucher-dot-com/tree/main/app/styles)

### Source Control Hygiene

While I have used many source control systems throughout my career (like VSS, CVS, SVN, Mercurial, and TFS), I have primarily used Git over the past decade and will talk about source control in that context.

Some guiding principles related to source control are:

* Git history matters (commits should be logical chunks of work and should tell a coherent story)
* Git pre-commit and commit message hooks are essential tools for maintaining code quality
* Code reviews are also a essential tool for not only ensuring code quality, but edifying development teams
* While `git blame` can be unreliable `git bisect` is your friend in times of trouble
* `TODO:`s are an effective means of cutting corners when business demands it, but providing for future enhancements/improvements

[View the commit log for kevinboucher.com](https://github.com/kboucher/kevinboucher-dot-com/commits/main)
