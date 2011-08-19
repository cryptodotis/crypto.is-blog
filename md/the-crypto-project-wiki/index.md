# The Crypto Project Wiki

The Crypto Project finally has a proper wiki for individuals to anonymously edit the [https://crypto.is][2] website properly. The wiki can be found at:

[https://wiki.crypto.is/][3]

## The Simple Explanation of the Editing Process

*This explanation is for those who are not developers.*

Editing the wiki will not automatically change the content on the live website. Once an edit is saved, a notification is made that lets the watchers of the repository know of the edits. Once the modifications are checked by reviewers (anyone) to make sure there is not malicious content, spam, or any other negative alteration the changes will be pushed live and generated into the new website.

## The More Complicated Explanation

*This explanation is for developers and can be skipped.*

The edits to the wiki are saved in a separate Git repository than that of the live site. Edits that are saved to the wiki trigger a post-commit hook that pushes the content to [This Github Repository][4]. Once the edits are approved, they are merged into the main [Crypto.is Repository][5]. From this point, once the new updates are made, approved, and merged, the build scripts take over and automatically generate the new website from the main repository.

## The Future of the Wiki

These protections are put in place as a precautionary measure so that readers of the website are not taken advantage of. At the current moment, this setup might seem like an over-engineered process. In the future we expect to have tutorials, guides, and all sorts of resources that, if modified to display incorrect information, could seriously endanger those who need anonymity, security, and privacy tools for survival.

This setup right now seems to be the best available that fits our needs: an easy to use and anonymous wiki interface, protections for the readers, and a website that still retains its design, readability, and visual integrity. The setup will evolve, simplify (hopefully), and become more automated as the problems with editing and creating content become evident.

It is the hope of The Crypto Project that these new additions will allow the project to be the canonical and authoritative resource for research, guides, tutorials, and more to individuals worldwide who hope to use anonymity, security, and privacy tools effectively.

Thank you for your time and support of The Crypto Project,

Sir Valiance

   [1]: http://blog.crypto.is/the-crypto-project-wiki
   [2]: https://crypto.is/
   [3]: https://wiki.crypto.is/
   [4]: https://github.com/cryptodotis-wiki/crypto.is-docs
   [5]: https://github.com/cryptodotis/crypto.is-docs
