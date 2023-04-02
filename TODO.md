- Once git key is established:
    - git remote set-url origin...
        - git@github.com:unilock/dotfiles-<platform>.git
        - git@github.com:unilock/dotfiles-common.git
    - git checkout main (in each repo ^)

- Symlink dotfiles (gitconfig, gitignore, etc.) and other preferences into respective folders via independent scripts in each OS-specific repository

- "AutoScroll" Chrome extension
    - Move speed: 5

- Discord (per OS, but keep prefs here)
    - Themes:
    - ```
      @import url(https://discord-modifications.github.io/dark-discord/src/source.css);
      @import url(https://cdn.jsdelivr.net/gh/Overimagine1/old-discord-font/source.min.css);
      ```
    - Vencord: https://github.com/Vencord/Installer
        - AlwaysTrust
        - BetterGifAltText
        - BlurNSFW
            - BLUR: 10
        - ClearURLs
        - CrashHandler
            - PREVENT CRASHES: Enabled
            - NAVIGATE TO HOME: Disabled
        - EmoteCloner
        - Experiments
            - ISSTAFF: Disabled
            - STAGING BANNER: Disabled
        - ForceOwnerCrown
        - FxTwitter
        - iLoveSpam
        - MemberCount
        - MessageClickActions
            - DELETE: Disabled
            - EDIT: Enabled
        - MessageLinkEmbeds
            - BG COLOR: Disabled
            - AUTOMOD EMBEDS: Never
        - MessageLogger
            - STYLE: Red overlay
            - IGNORE BOTS: Enabled
            - IGNORE SELF: Enabled
        - MuteNewGuild
        - NoCanaryMessageLinks
            - SUBDOMAIN: (empty)
            - USE DISCORD.COM: Enabled
        - NoUnblockToJump
        - PlatformIndicators
            - MEMBER LIST: Enabled
            - USER PROFILES: Enabled
            - MESSAGES: Enabled
            - MOBILE MATCH STATUS: Enabled
        - PronounDB
            - FORMAT: Lowercase
            - CURRENT USER: Enabled
            - MESSAGES: Enabled
            - PROFILE: Enabled
        - QuickMention
        - ReverseImageSearch
        - ShikiCodeblocks
            - THEME: Monokai
            - DISCORD HIGHLIGHTER: Prefer Shiki
            - ICONS: Colorless
            - OPACITY: 100%
        - SortFriendRequests
            - SHOW DATES: Enabled
        - TypingTweaks
            - AVATARS: Enabled
            - ROLE COLORS: Enabled
            - SEVERAL USERS TYPING: Enabled
        - ViewIcons
        - ViewRaw
        - VoiceChatDoubleClick
        - VolumeBooster
            - MULTIPLIER: 2
        - WhoReacted

- IntelliJ prefs

- Vivaldi: Should be synced for the most part, but IIRC there are some platform-specific settings - document in respecitve OS dotfiles as they're found


- DuckDuckGo settings
    - Safe search: OFF
    - General
        - Advertisements: OFF
        - Install DuckDuckGo: OFF
        - Privacy Newsletters: OFF (both)
        - Homepage Privacy Tips: OFF
        - Help Improve DuckDuckGo: OFF
    - Privacy
        - Redirect (When Necessary): OFF
