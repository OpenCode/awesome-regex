# Awesome Regex (Regular Expressions) [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated list of awesome Regex (Regular Expressions) ready to use

## Table of Content

- [Awesome Regex](#awesome-regex)
    - [Information technology](#information-technology)
      - [Hex color](#hex-color)
      - [IP Address](#ip-address)
      - [MAC Address](#mac-address)
      - [Mail](#mail)
      - [URL](#url)
        - [Spotify track](#spotify-track)
        - [Spotify playlist](#spotify-playlist)
        - [Soundcloud](#soundcloud)
        - [Deezer track/album/playlist](#deezer-trackalbumplaylist)
        - [Youtube](#youtube)
        - [Vimeo](#vimeo)
        - [Dailymotion](#dailymotion)
        - [Facebook](#facebook-photo--video)
        - [NERDZCrush](#nerdzcrush)
        - [Imgur](#imgur)
        - [GitHub](#github-profile--organization)
        - [Twitter status](#twitter-status)
      - [Text manipulation](#text-manipulation)
        - [Remove CDATA tags](#remove-cdata-tags)

## Information technology

### Hex color
    /^#([A-Fa-f0-9]{6}|[A-Fa-f0-9]{3})$/

### IP Address
    /^((?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?))*$/
    
### MAC Address
    /^(?:[0-9a-f]{2}[\-:]?){6}(?<![\-:])$/i

### Mail
    /^([a-zA-Z0-9_\-\.]+)@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.)|(([a-zA-Z0-9\-]+\.)+))([a-zA-Z]{2,4}|[0-9]{1,3})(\]?)$/

### URL
    /^(((http|https|ftp):\/\/)?([[a-zA-Z0-9]\-\.])+(\.)([[a-zA-Z0-9]]){2,4}([[a-zA-Z0-9]\/+=%&_\.~?\-]*))*$/

#### Spotify track
    /^https?:\/\/(?:open|play)\.spotify\.com\/track\/[\w\d]+$/i

#### Spotify playlist
    /^https?:\/\/(?:open|play)\.spotify\.com\/user\/([\w\d]+)\/playlist\/[\w\d]+$/i

#### Soundcloud
    /^https?:\/\/soundcloud\.com\/\S+\/\S+$/i

#### Deezer track/album/playlist
    /^https?:\/\/(?:www\.)?deezer\.com\/(track|album|playlist)\/(\d+)$/

#### Youtube
    /^https?:\/\/(?:(?:www|m)\.)?(?:youtube\.com\/watch(?:\?v=|\?.+?&v=)|youtu\.be\/)([a-z0-9_-]+)$/i

#### Vimeo
    /^https?:\/\/(?:www\.)?vimeo\.com.+?(\d+).*$/i

#### Dailymotion
    /^https?:\/\/(?:www\.)?(?:dai\.ly\/|dailymotion\.com\/(?:.+?video=|(?:video|hub)\/))([a-z0-9]+)$/i

#### Facebook photo / video
    /^https?:\/\/(?:www\.)?facebook\.com\/(?:(?:photo|video)\.php(?:\?v=|\?.+?&v=)|[a-z0-9._-]+\/videos\/)(\d+)\/?$/i

#### NERDZCrush
    /^https?:\/\/(?:cdn\.)?media\.nerdz\.eu\/([a-z0-9_-]{12})(?:|\.[a-z0-9]{2,4})$/i

#### Imgur
    /^https?:\/\/(?:www\.)?(?:i\.)?imgur\.com\/([a-z0-9_-]+)\.(?:gifv|webm)$/i

#### GitHub profile / organization
    /^https?:\/\/(www\.)?github\.com\/[a-z0-9]+$/i

#### Twitter status
    /^https?:\/\/twitter.com\/[a-z0-9_]+\/status\/[0-9]+$/i

## Text manipulation

### Remove CDATA tags
    /<!\[CDATA\[(.*)\]\]>/
