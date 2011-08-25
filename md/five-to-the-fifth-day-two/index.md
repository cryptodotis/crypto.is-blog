# Five to the Fifth: Day Two Wrap Up

So after the headaches of Day One, Day Two went much smoother mostly due to the simple service that was chosen for Day Two, [Convergence][1].  Convergence is, as stated on the website, "An agile, distributed, and secure strategy for replacing Certificate Authorities".  What this means, simply put, is that Convergence is a Firefox plugin that verifies the SSL certificate for the site you are currently viewing by checking it against the SSL certificate retrieved by a server or servers for that website.  A convergence server is called a "notary".  In our case, we will be setting up a a notary for others to use. 

The only roadblock that I ran into when setting up the notary was attempting to run it behind Nginx.  Oddly, the notary was failing when simply placing it behind Nginx (for The Crypto Project, Nginx is run as an SSL reverse proxy to other servers, so Convergence was run on a separate machine). 

The Crypto Project Convergence Notary will be put up for public use today, but please be aware that its status could change very soon. Ideally, it would run behind Nginx and accept connections on the standard 80/443 ports.  Currently, our Convergence notary runs a self-signed cert generated by Convergence.  This might changes as well.  After this week, most of the services setup for "Five to the Fifth" will be shuffled around a bit to make sure they are configured in the best setup possible.  To download our notary file, go to: 

[The Crypto Project .notary File][2]

Once again, running the all of these servers/services is not free. Please donate at [our Donations page][3] and we will continue to expand our network and services. Thank you again for your time and attention as we work in this event and setup more services to help with security, privacy, and censorship circumvention!

   [1]: http://convergence.io
   [2]: http://crypto.is/static/files/cryptodotis.notary 
   [3]: https://crypto.is/interact/money/


