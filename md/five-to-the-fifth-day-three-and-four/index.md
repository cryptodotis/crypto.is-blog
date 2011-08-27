# Five to the Fifth: Day Three and Four Wrap Up

It should probably be clear to everyone at this point that I am running a little "behind" on the schedule of the "Five to the Fifth" event.  Wrap up posts are a day or so late and it is Friday night and only 4 of the 5 services are up.  Hopefully I will have the fifth service up tonight. To recap, the server setup on Monday was a Tor relay, but I also setup a mirror of the TorProject.org website.  On Tuesday, I setup a Convergence.io notary server.  Since then, I have setup an anonymous remailer and the start of our Tahoe-LAFS grid.

## Anonymous remailer

At the start of the "Five to the Fifth" event, it looked like the I was going to setup a Mixmaster server.  It became very clear, very quickly that this was going to be a configuration nightmare, especially to automate the building and setup of it. The remailer was put off until later in the week.  I finally decided that a [Mixminion][1] node was the way to go.

I had previously made some slight updates to the Mixminion source to allow it to run with newer Pythons (2.6, 2.7+) so I was able to get it running quite easily on our Ubuntu 10.10 servers. The setup and configuration is a breeze compared to Mixmaster.  The nickname for our remailer is "cryptodotis" and it is currently running as a relay (should be in the Directory shortly). You can find the source for the mixminion setup at [our github repository][2], but I would not recomend running the script just yet.

## Tahoe-LAFS Grid

The next service that was setup was a [Tahoe-LAFS][3] introducer node and storage grid.  The process of setting this up was quite easy as well.  I will not publicize the FURL for our introducer just yet because I want to get the kinks ironed out first.  Ideally, I would like to have our Tahoe grid run over Tor, preferably with the storage nodes behind hidden services.  Initially, our grid will remain private to The Crypto Project developers (you could be one, just hang out in IRC!) to prevent abuse.  Once we have the grid setup, access permisions properly handled, and assurance that it is safe for both clients and server admins, The Crypto Project Grid will be slowly opened up.

## Whats next?

For the last service, I am thinking I will create a web-frontend to Mixminion.  The idea would be to place this behind a Tor hidden service. There are plenty of flaws in the idea of a web frontend to such tools, especially when you add in Javascript based encryption of messages.  This will simply be an experiment.  The guides and setup source code repositories for each service setup from the week should be published to the website by the end of the weekend.  I will also have an event wrap up blog post.

Thank You Again, 
Sir Valiance


   [1]: http://mixminion.net
   [2]: https://github.com/cryptodotis/mixminion-setup
   [3]: http://tahoe-lafs.org
