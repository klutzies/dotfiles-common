- Once git key is established:
    - git remote set-url origin...
        - git@github.com:unilock/dotfiles-linux.git
        - git@github.com:unilock/dotfiles-common.git
    - git checkout main (in each repo ^)

- Symlink dotfiles (gitconfig, gitignore, etc.) and other preferences into respective folders via independent scripts in each OS-specific repository

- "AutoScroll" Chrome extension
    - Move speed: 5

- Discord (per OS, but keep prefs here)
    - OpenAsar: https://openasar.dev
        - Themes:
        - ```
          @import url(https://discord-modifications.github.io/dark-discord/src/source.css);
          @import url(https://cdn.jsdelivr.net/gh/Overimagine1/old-discord-font/source.min.css);
          ```
    - Vencord: https://github.com/Vencord/Installer
        - AnonymiseFileNames
            - Anonymising method: RANDOM
            - Random characters length: 7
            - Consistent filename: N/A
        - BetterGifAltText
        - BetterNotesBox
            - Hide notes: ENABLED
            - Disable spellcheck in notes: N/A
        - BlurNSFW
            - Blur amount: 10
        - ClearURLs
        - EmoteCloner
        - ForceOwnerCrown
        - FxTwitter
        - iLoveSpam
        - MemberCount
        - MessageLinkEmbeds
            - Background color for messages in rich embeds: DISABLED
            - Use automod embeds instead of rich embeds: NEVER
        - MessageLogger
            - The style of deleted messages: RED OVERLAY
            - Whether to ignore messages by bots: ENABLED
            - Whether to ignore messages by yourself: ENABLED
        - NoCanaryMessageLinks
            - The subdomain for your Discord message links: N/A
            - Always use discord.com host (replace discordapp.com): ENABLED
        - NoReplyMention
            - List of users to exempt from this plugin (separated by commas): N/A
        - NoUnblockToJump
        - PlatformIndicators
            - Show indicators in the member list: ENABLED
            - Show indicators in user profiles, as badges: ENABLED
            - Show indicators inside messages: ENABLED
        - PronounDB
            - The format for pronouns to appear in chat: LOWERCASE
            - Enable or disable showing pronouns for the current user: ENABLED
        - QuickMention
        - ReverseImageSearch
        - ShikiCodeblocks
            - Default themes: MONOKAI
            - A link to a custom VSCode theme: N/A
            - Use the more lightweight default Discord highlighter and theme: PREFER SHIKI
            - How to show language icons on codeblocks: COLORLESS
            - Background opacity: 100
        - SortFriendRequests
            - Show dates on friend requests: DISABLED
        - ViewIcons
        - ViewRaw
        - VoiceChatDoubleClick
        - VolumeBooster
        - WebContextMenus
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
