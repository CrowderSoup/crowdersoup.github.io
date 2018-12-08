+++
title = "Hosting Mastodon on DitialOcean"
description = "A how-to on hosting Mastodon on a DigitalOcean VPS and using Spaces"
date = "2018-11-27 17:14:00"
categories = ["SocialMast.xyz"]
tags = [
  "projects",
  "servers",
  "dev ops"
]
+++
I've been toying with the idea of setting up [Mastodon][1] on my own server for
a while now. Today I finally got around to actually doing it (after a failed
attempt a couple months ago). I found a [guide][2] that I loosely referred to
and was immensely helpful at a couple points.

At first I tried running on a super small $5 instance, which seemed fine during
setup, but died every few requests when I started using it. I ended up bumping
the server up to the $15 a month plan (3GB RAM, single CPU core) and things
seem to be working fine now. I'll re-evaluate my plan if things start slowing
down again.

I'm using docker to run Mastodon, so if you don't want to do that you'll have
better luck with a different guide. I like Docker because it makes it easy to
run the various things we need to run for Mastodon ([SideKiq][3], PostgreSQL,
etc.).

## TODO:
0. Set up mailgun
1. Create a VPS
2. Create your space
3. Generate keys to use with your space
4. Setup your VPS (install all the things)
5. Install / Configure Mastodon
6. Configure Nginx
7. Set up SSL/HTTPS with Certbot
8. Run Mastodon
9. Configure Cron Jobs for upkeep
10. Create your first user and make it an Admin


<!--Links-->
[1]: https://joinmastodon.org
[2]: https://github.com/ummjackson/mastodon-guide/blob/master/up-and-running.md
[3]: https://sidekiq.org/
