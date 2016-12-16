# LXiMediaServer with Docker

Docker image for LXiMedia, a DLNA compatible, fully transcoding, media server designed for serving media (movies, TV shows, music, photos) to DLNA compliant televisions and media players (Streamium, PS3, XBox 360). Also subtitles and audio language selection are supported.

It use AUR [lximediaserver-svn](https://aur.archlinux.org/packages/lximediaserver-svn/) package based on [lximedia](https://sourceforge.net/projects/lximedia/) project.


License: **MIT**

## Local build
```sh
$ docker build -t mdouchement/lximediaserver .
```

## Running LXiMedia container

```sh
# Running and get a Bash interpreter
$ docker run -v /my_media:/data --net=host -it mdouchement/lximediaserver:latest

# Running as daemon
$ docker run -v /my_media:/data --net=host -d mdouchement/lximediaserver:latest
```

## License

MIT

## Contributing

All PRs are welcome.

1. Fork it ( https://github.com/[my-github-username]/gemsupport/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
