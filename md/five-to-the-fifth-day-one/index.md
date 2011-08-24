# Five to the Fifth: Day One Wrap Up

At the start of the day Monday, I had orginally stated that the first service that would be setup would be a remailer. I started working on setting up a [Mixmaster node][1] but it soon became clear that I had not set enough time aside to correctly configure the server *and* build a working automation script.  It was at that point I decided to switch to setting up a Tor relay and a [TorProject.org mirror][2]. 

The process of setting up Tor node was quite simple. So simple, that at a certain point it became clear that it would most likely take more time for a user who wanted to follow this setup to use the [automation scripts][3] than it would to simply set it up on their own.  If anything, the supplied code serves as a example for individuals to reference when setting up their own nodes.

I stuggled late into the night to keep my eyes open fully while attempting to configure a [TorProject.org mirror][2] with Nginx. Nginx is the server that I typically use for projects, so it seemed natural to use that over Apache. I hit some unsual issue (one that at least I had not seen before) where the server was returning unrendered html of the page requested with a 403 error header. I thought is was a permissions error or an issue with the rysynced files but I also could have just been hallucinating to whole error due to sleep deprivation.  At that point, I cut my losses and just used Apache and set it up nearly following the [Tor Projects Setup][4] exactly.  Our TorProject.org mirror can be found at:

[The Crypto Project TorProject.org Mirror][7]

The hosting provider the node was setup on (Rackspace Cloud) is most likely not the best host for running a high speed node because it can suck up bandwith *extremely* fast. So fast, that I had set a test 1GB daily limit on the node and it was up for less than an hour before it went into hibernation waiting for the next day.  Inbound traffic is free on the host but outbound is not cheap.  For 1TB a month on the base 256MB server size would cost you approximately $200 a month. The next step (most likely next week) is to move the Tor relay to [Hetzner.de][5] (or some other host, let us know of a recommendation) and open it up to be an exit node. Our Tor nodes current fingerprint is:

   cryptodotis 73F8D55A18657C4155E7440F67ACCA1F51A6FE74 

The great part about having the "Five to the Fifth Event" is all of the ideas, suggestions, attention, and help people have given to its effort.  I can see this becoming a regular event for The Crypto Project to run since there are so many great ideas and help needed for censorship circumvention, privacy, and security.  I can see The Crypto Project network expanding to DNS services, Tor Bridges, our own Tahoe-LAFS grid, and more as we move forward.  Of course running these nodes is not free and if we cannot cover the costs of the servers through donations I (Sir Valiance) pay for the remaining balance.  Please donate at [our Donations page][6] and we will continue to expand our network and services. Thank you for your time and attention as we work through this event!

Thank You Again,
Sir Valiance

   [1]: http://mixmaster.sourceforge.net/
   [2]: https://torproject.org
   [3]: https://github.com/cryptodotis/tor-server-setup
   [4]: https://www.torproject.org/docs/running-a-mirror.html.en 
   [5]: https://hetzner.de
   [6]: https://crypto.is/interact/money/
   [7]: https://torproject.crypto.is
