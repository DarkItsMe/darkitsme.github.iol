
/*
 $$$$$$\  $$\           $$\                 $$\           
$$  __$$\ $$ |          $$ |                $$ |          
$$ /  \__|$$ | $$$$$$\  $$$$$$$\   $$$$$$\  $$ | $$$$$$$\ 
$$ |$$$$\ $$ |$$  __$$\ $$  __$$\  \____$$\ $$ |$$  _____|
$$ |\_$$ |$$ |$$ /  $$ |$$ |  $$ | $$$$$$$ |$$ |\$$$$$$\  
$$ |  $$ |$$ |$$ |  $$ |$$ |  $$ |$$  __$$ |$$ | \____$$\ 
\$$$$$$  |$$ |\$$$$$$  |$$$$$$$  |\$$$$$$$ |$$ |$$$$$$$  |
 \______/ \__| \______/ \_______/  \_______|\__|\_______/ 
*/
/*BD Addon Mini List by Disease#3749*/
@import url(https://maendisease.github.io/BetterDiscordStuff/css/bdAddonMini.css);
:root {
  /*Global variables that were made/edited by me*/
  --Main-Color: rgb(250,0,0); /*main master color*/
  --Secondary-Color: rgb(150,0,0); /*secondary color*/
  --Third-Color: rgb(120,0,0); /*third color*/
  --Color-4: rgb(90,0,0); /*color number 4*/
  --Grey-Color: rgb(31, 31, 31); /*grey color*/
  --Black: rgb(0,0,0); /*black color*/
  --White: rgb(255,255,255); /*white color*/
  --White-Second: rgb(175, 175, 175); /*white but gray color*/
  --Neon-Line: 150,0,0; /*master neon color*/
  --Neon-Rgb: var(--Neon-Line); /*neon node*/
  /*Backgrounds*/
  --master-background: url('https://faunistics.com/wp-content/uploads/2020/01/1-5.jpg'); /*master background*/
  --background-floating: linear-gradient(rgba(0, 0, 0, 0.5),rgba(0, 0, 0, 0.2)) , var(--master-background)50% 50%/cover !important; /*background used in normal discord's code*/
  --background-black-and-white1: url('https://inspirationfeed.com/wp-content/uploads/2018/12/lou-batier-365323-unsplash-768x512.jpg'); /*background 3*/
  --background-black-and-white2: url('https://inspirationfeed.com/wp-content/uploads/2018/12/martin-sattler-160751-unsplash-768x575.jpg'); /*background 4*/
  /*Gifs for popouts and stuff*/
  --loop-gif: url('https://c.tenor.com/2oQwi7vJz9wAAAAC/loop-space.gif'); /*Used in files background*/
  --loop-gif2: url('https://64.media.tumblr.com/16314eedf67c43cc5cb711ffe8c0b08e/22caaa59656e483e-b3/s640x960/7f706f80fb11b3390532fea23ffca444a6f3ea32.gifv'); /*Used in guild popouts > User popout*/
  --loop-gif3: url('https://i.pinimg.com/originals/d5/a7/cb/d5a7cb46e2f15a8fed10aaf1dd00965c.gif'); /*Used in message area input*/
  --loop-gif4: url('https://64.media.tumblr.com/8da032603a2ff3343c32833d7959e7bc/tumblr_p61tzgchCN1qeyvpto1_500.gifv'); /*Used in guild popouts > Mentioned card*/
  --loop-gif5: url('https://64.media.tumblr.com/998b664cb9fd89a155b3b105dbdc9a09/808262fefad64e38-9c/s500x750/5f09d008c448b11092d119bf69d0751e08d79631.gifv'); /*Used in emoji, sticker, gif, nitro, pinned messages and left click on dm in friends tab*/
  --loop-gif-diamond: url('https://giffiles.alphacoders.com/143/14390.gif'); /*Used on home icon*/
  /*Borders*/
  --border1: 2px solid var(--Secondary-Color); /*master border*/
  --border2: 2px solid var(--Third-Color); /*border 2*/
  --border3: 2px solid rgb(90,0,0); /*border 3*/
  
  /*Others variables*/
  /*Radial status*/
  --rs-small-spacing: 0px; /* Gap between avatar and status for members list/dms | MUST end in px */
  --rs-medium-spacing: 0.1px; /* Gap between avatar and status for User popout | MUST end in px */
  --rs-large-spacing: 0px; /* Gap between avatar and status for User profiles | MUST end in px */
  --rs-small-width: 2px; /* Thickness of status border for members list/dms | MUST end in px */
  --rs-medium-width: 3px; /* Thickness of status border for User popout | MUST end in px */
  --rs-large-width: 4px; /* Thickness of status border for User profile | MUST end in px */
  --rs-avatar-shape: 50%; /* 50% for round - 0% for square */
  --rs-online-color: #21df00; /* Colour for online status */
  --rs-idle-color: #ffffff; /* Colour for idle status */
  --rs-dnd-color: #ee0000; /* Colour for dnd status */
  --rs-offline-color: #636b75; /* Colour for offline status */
  --rs-streaming-color: #b300fa; /* Colour for streaming status */
  --rs-invisible-color: #747f8d; /* Colour for invisible status - Note: this will only show for your own invisibility */
  --rs-phone-color: var(--rs-online-color); /* Colour of the ring and phone icon when a user is on their phone |  */
  /*edited only this one below*/
  --rs-phone-visible: none; /* Visibility of the phone icon next to a users avatar. | block = visible | none = hidden */
}
/*
$$\      $$\             $$\                                                           $$\       
$$ | $\  $$ |            $$ |                                                          $$ |      
$$ |$$$\ $$ | $$$$$$\  $$$$$$\    $$$$$$\   $$$$$$\  $$$$$$\$$$$\   $$$$$$\   $$$$$$\  $$ |  $$\ 
$$ $$ $$\$$ | \____$$\ \_$$  _|  $$  __$$\ $$  __$$\ $$  _$$  _$$\  \____$$\ $$  __$$\ $$ | $$  |
$$$$  _$$$$ | $$$$$$$ |  $$ |    $$$$$$$$ |$$ |  \__|$$ / $$ / $$ | $$$$$$$ |$$ |  \__|$$$$$$  / 
$$$  / \$$$ |$$  __$$ |  $$ |$$\ $$   ____|$$ |      $$ | $$ | $$ |$$  __$$ |$$ |      $$  _$$<  
$$  /   \$$ |\$$$$$$$ |  \$$$$  |\$$$$$$$\ $$ |      $$ | $$ | $$ |\$$$$$$$ |$$ |      $$ | \$$\ 
\__/     \__| \_______|   \____/  \_______|\__|      \__| \__| \__| \_______|\__|      \__|  \__|
*/
div[class*="typeWindows-"]::after {
  content: 'DRACONICXYROLES version 40';
  font-weight: bold;
  line-height: 30px;
  color: var(--Main-Color);
  font-size: 13.5px;
  position: absolute;
  padding: 0 15px;
  top: 0;
  left: 0;
  width: 100%;
  height: 20px;
  background: transparent;
  z-index: -1;
}

/*Discord's global variables copy-paste and edited*/
.theme-dark, .theme-light {
  --info-positive-background: transparent!important;
  --info-positive-foreground: transparent!important;
  --info-warning-background: transparent!important;
  --info-warning-foreground: transparent!important;
  --info-danger-background: transparent!important;
  --info-danger-foreground: transparent!important;
  --status-positive-background: transparent!important;
  --status-positive-text: #fff;
  --status-warning-background: hsl(38,calc(var(--saturation-factor, 1)*95.7%),54.1%);
  --status-danger-background: hsl(359,calc(var(--saturation-factor, 1)*82.6%),59.4%);
  --status-danger-text: #fff;
  --focus-primary: hsl(197,calc(var(--saturation-factor, 1)*100%),47.8%);
}
.theme-dark {
  --header-primary: #8f949c;
  --header-secondary: #7a7f86;
  --text-normal: #fff;
  --text-muted: #55585d;
  --text-link: hsl(197,calc(var(--saturation-factor, 1)*100%),47.8%);
  --text-link-low-saturation: hsl(197,calc(var(--saturation-factor, 1)*100%),52.9%);
  --text-positive: hsl(139,calc(var(--saturation-factor, 1)*66.8%),58.6%);
  --text-warning: hsl(38,calc(var(--saturation-factor, 1)*95.7%),54.1%);
  --text-danger: hsl(359,calc(var(--saturation-factor, 1)*82.6%),59.4%);
  --text-brand: hsl(235,calc(var(--saturation-factor, 1)*86.1%),77.5%);
  --interactive-normal: #72767d;
  --interactive-hover: #fff;
  --interactive-active: #fff;
  --interactive-muted: #55585d;
  --background-primary: transparent;
  --background-secondary: transparent;
  --background-secondary-alt: transparent;
  --background-tertiary: transparent;
  --background-accent: transparent;
  --background-floating: transparent;
  --background-nested-floating: transparent;
  --background-mobile-primary: transparent;
  --background-mobile-secondary: transparent;
  --background-modifier-hover: transparent;
  --background-modifier-active: transparent;
  --background-modifier-selected: transparent;
  --background-modifier-accent: transparent;
  --info-positive-text: #fff;
  --info-warning-text: #fff;
  --info-danger-text: #fff;
  --info-help-background: transparent;
  --info-help-foreground: transparent;
  --info-help-text: #fff;
  --status-warning-text: #000;
  --scrollbar-thin-thumb: var(--Main-Color);
  --scrollbar-thin-track: transparent;
  --scrollbar-auto-thumb: transparent;
  --scrollbar-auto-track:  transparent;
  --scrollbar-auto-scrollbar-color-thumb: transparent;
  --scrollbar-auto-scrollbar-color-track: transparent;
  --elevation-stroke: 0 0 0 1px rgba(4,4,5,0.15);
  --elevation-low: 0 1px 0 rgba(4,4,5,0.2),0 1.5px 0 rgba(6,6,7,0.05),0 2px 0 rgba(4,4,5,0.05);
  --elevation-medium: 0 4px 4px rgba(0,0,0,0.16);
  --elevation-high: 0 8px 16px rgba(0,0,0,0.24);
  --logo-primary: #fff;
  --control-brand-foreground: hsl(235,calc(var(--saturation-factor, 1)*86.1%),77.5%);
  --control-brand-foreground-new: hsl(235,calc(var(--saturation-factor, 1)*86.1%),77.5%);
  --background-mentioned: transparent;
  --background-mentioned-hover: transparent;
  --background-message-hover: transparent;
  --background-message-automod: transparent;
  --background-message-automod-hover: transparent;
  --channels-default: #8e9297;
  --guild-header-text-shadow: 0 1px 1px rgba(0,0,0,0.4);
  --channeltextarea-background: transparent;
  --activity-card-background: #202225;
  --textbox-markdown-syntax: #8e9297;
  --spoiler-revealed-background: #292b2f;
  --spoiler-hidden-background: #202225;
  --deprecated-card-bg: transparent;
  --deprecated-card-editable-bg: transparent;
  --deprecated-store-bg: transparent;
  --deprecated-quickswitcher-input-background: transparent;
  --deprecated-quickswitcher-input-placeholder: hsla(0,0%,100%,0.3);
  --deprecated-text-input-bg: transparent;
  --deprecated-text-input-border: rgba(0,0,0,0.3);
  --deprecated-text-input-border-hover: #040405;
  --deprecated-text-input-border-disabled: #202225;
  --deprecated-text-input-prefix: #dcddde;
}
/*
$$$$$$$\                      $$\                                                               $$\ 
$$  __$$\                     $$ |                                                              $$ |
$$ |  $$ | $$$$$$\   $$$$$$$\ $$ |  $$\  $$$$$$\   $$$$$$\   $$$$$$\  $$\   $$\ $$$$$$$\   $$$$$$$ |
$$$$$$$\ | \____$$\ $$  _____|$$ | $$  |$$  __$$\ $$  __$$\ $$  __$$\ $$ |  $$ |$$  __$$\ $$  __$$ |
$$  __$$\  $$$$$$$ |$$ /      $$$$$$  / $$ /  $$ |$$ |  \__|$$ /  $$ |$$ |  $$ |$$ |  $$ |$$ /  $$ |
$$ |  $$ |$$  __$$ |$$ |      $$  _$$<  $$ |  $$ |$$ |      $$ |  $$ |$$ |  $$ |$$ |  $$ |$$ |  $$ |
$$$$$$$  |\$$$$$$$ |\$$$$$$$\ $$ | \$$\ \$$$$$$$ |$$ |      \$$$$$$  |\$$$$$$  |$$ |  $$ |\$$$$$$$ |
\_______/  \_______| \_______|\__|  \__| \____$$ |\__|       \______/  \______/ \__|  \__| \_______|
                                        $$\   $$ |
                                        \$$$$$$  |
                                         \______/
*/
.appMount-3lHmkl, body {
  background: linear-gradient(rgba(0, 0, 0, 0.5),rgba(0, 0, 0, 0.2)) , var(--master-background) 50% 50%/cover !important;
  background-color: transparent!important;
  text-rendering: optimizeLegibility;
}
.appMount-2yBXZl, body {
  background: linear-gradient(rgba(0, 0, 0, 0.6),rgba(0, 0, 0, 0.8)) , var(--master-background) 50% 50%/cover !important;
  background-color: transparent!important;
  text-rendering: optimizeLegibility;
}
  
/*
 $$$$$$\            $$\ $$\       $$\           
$$  __$$\           \__|$$ |      $$ |          
$$ /  \__|$$\   $$\ $$\ $$ | $$$$$$$ | $$$$$$$\ 
$$ |$$$$\ $$ |  $$ |$$ |$$ |$$  __$$ |$$  _____|
$$ |\_$$ |$$ |  $$ |$$ |$$ |$$ /  $$ |\$$$$$$\  
$$ |  $$ |$$ |  $$ |$$ |$$ |$$ |  $$ | \____$$\ 
\$$$$$$  |\$$$$$$  |$$ |$$ |\$$$$$$$ |$$$$$$$  |
 \______/  \______/ \__|\__| \_______|\_______/
*/

/* #################### User popout in guilds #################### */
/*User popout*/
.userPopout-2j1gM4 {
  background: linear-gradient(rgba(0, 0, 0, 0.5),rgba(0, 0, 0, 0.6)) , var(--loop-gif2) 50% 50%/cover !important;
  border-color: rgb(var(--Neon-Rgb))!important;
  box-shadow: inset 0px 0px 5px 1px rgb(var(--Neon-Rgb)), 0px 0px 15px 4px rgb(var(--Neon-Rgb))!important;
}
/*The "+" popout, add roles*/
.container-2O1UgZ {
  background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.9)) , var(--background-black-and-white1) 50% 50%/cover no-repeat!important;
  border-color: rgb(var(--Neon-Rgb));
  box-shadow: inset 0px 0px 5px 1px rgb(var(--Neon-Rgb)), 0px 0px 15px 4px rgb(var(--Neon-Rgb));
}

/*All in channel icons, Threads, Notifications, Pinned messages, Hide member List, Notes*/
.clickable-ZD7xvu .icon-2xnN2Y {
  color: var(--Main-Color);
}
.icon-2xnN2Y {
  color: var(--Main-Color);
}

/*Server name color*/
.name-3Uvkvr {
  color: var(--Main-Color);
}

/*Selected channels in guild*/
/*channel text color*/
.modeConnected-NrO4cP .name-28HaxV, .modeConnected-NrO4cP:hover .name-28HaxV, .modeSelected-3DmyhH .name-28HaxV, .modeSelected-3DmyhH:hover .name-28HaxV, .modeUnread-3Cxepe .name-28HaxV, .modeUnread-3Cxepe:hover .name-28HaxV, .notInteractive-2tFrlE.modeConnected-NrO4cP .name-28HaxV, .notInteractive-2tFrlE.modeSelected-3DmyhH .name-28HaxV {
  color: var(--Main-Color);
}
/*icon color*/
.modeSelected-3DmyhH .icon-2W8DHg, .modeSelected-3DmyhH:hover .icon-2W8DHg, .modeUnread-3Cxepe .icon-2W8DHg, .modeUnread-3Cxepe:hover .icon-2W8DHg {
  color: var(--Main-Color);
}

/* #################### Guilds unread & mentioned popouts #################### */
/*Unread*/
.unread-2wipsx {
  background: linear-gradient(rgba(0, 0, 0, 0.5),rgba(0, 0, 0, 0.2)) , var(--loop-gif) 50% 50%/cover !important;
  opacity: .9;
  border: solid 2px var(--Secondary-Color);
}
/*Metioned*/
.mention-3XBnnZ {
  background: linear-gradient(rgba(0, 0, 0, 0.5),rgba(0, 0, 0, 0.2)) , var(--loop-gif4) 50% 50%/cover !important;
  opacity: .9;
  border-radius: 5px;
  border-color:var(--Black);
}

/* #################### Guild Channel Slow Mode warning ####################*/
.base-3bcbY3 .cooldownWrapper-2k1jHK {
  color: var(--Main-Color)!important;
}

/*Guild folders*/
.expandedFolderBackground-1kSAf6 {
  position: absolute;
  top: 0px;
  left: 9.5px;
  bottom: 0px;
  width: 50px;
  border-radius: 20px;
  background: var(--Black);
  border: solid 2px var(--Secondary-Color);
}
/*Closed guilds folder blur effect*/
.closedFolderIconWrapper-3tRb2d {
  filter: blur(3px);
}
/*Guild info popout when hover (Thanks Disease)*/
.tooltip-14MtrL {
  background: var(--Black)!important;
  border: var(--border2)!important;
  border-radius: 15px;
}

/*In guild hover on voice channel popout (playing, listening to spotify)*/
.container-8Futzw {
  background: linear-gradient(rgba(0, 0, 0, 0.6),rgba(0, 0, 0, 0.4)) , var(--background-black-and-white1) 50% 50%/cover !important;
  border-color: rgb(var(--Neon-Rgb));
  box-shadow: inset 0px 0px 5px 1px rgb(var(--Neon-Rgb)), 0px 0px 15px 4px rgb(var(--Neon-Rgb));
}

/*In guild channel, roles acces*/
.role-23oyrw {
  color: var(--text-normal);
  background-color: transparent;
  border: var(--border2);
  border-radius: 15px;
}

/*Guild Roles*/
/* Default permissions */
.container-_phMUq {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  background-color: transparent;
  color: var(--Main-Color);
  border-radius: 0px;
  padding: 16px 24px 16px 16px;
  cursor: pointer;
}
.container-_phMUq:hover {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  background-color: var(--Black-Color);
  color: var(--Main-Color);
  border-radius: 0px;
  padding: 16px 24px 16px 16px;
  cursor: pointer;
}
/* Search Roles */
.container-cMG81i {
  border-radius: 4px;
  overflow: hidden;
  background-color: transparent;
}
/*Roles Column Margins*/
.rolesList-3uZoaa {
  margin-bottom: 20px;
}
/*Roles margin left-right*/
.role-2TIOKu {
  font-size: 12px;
  font-weight: 500;
  background: var(--background-secondary-alt);
  border-radius: 4px;
  -webkit-box-sizing: border-box;
  box-sizing: border-box;
  height: 22px;
  margin: 0 4px 4px 0;
  padding: 4px;
  margin-right: 200px;
}
/*Roles card in guilds*/
.userPopout-2j1gM4 {
  -webkit-box-shadow: var(--elevation-high);
  box-shadow: var(--elevation-high);
  background-color: var(--background-floating);
  border-radius: 8px;
  border-color: var(--Main-Color);
  overflow: hidden;
  max-height: calc(100vh - 20px);
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
}
/*+ add roles popout*/
.container-2O1UgZ {
  width: 250px;
  overflow: hidden;
  border-radius: 4px;
  -webkit-box-sizing: border-box;
  box-sizing: border-box;
  padding: 8px;
  background-color: var(--Black);
  border: var(--border2);
}

/*Unread message bar "X+ new messages since XX:XXPM/AM" color and background*/
.newMessagesBar-1hF-9G {
  border: none;
  background: linear-gradient(rgba(0, 0, 0, 0.6),rgba(0, 0, 0, 0.4)) , var(--background-black-and-white1) 50% 50%/cover !important;
}

/* #################### Server boost tab #################### */
/*background*/
.theme-dark .perksModal-CLcR1c {
  background-image: linear-gradient(rgba(0, 0, 0, 0.5),rgba(0, 0, 0, 0.2)) , var(--master-background) 50% 50%/cover !important;
  background-color: transparent;
}

/*Everything below "server boost" text*/
/*gift icon from "gift nitro"*/
.theme-dark .giftIcon-2kmx1K {
  color: var(--Main-Color);
}

/*Server boost icon "no boosts"*/
.theme-dark .badgeIconWithoutSubscribers-1hjTfX {
  color: var(--Main-Color);
}
/*Server boost icon "X boosts"*/
.badgeIconWithSubscribers-2WYJsQ {
  color: var(--Main-Color);
}

/*Progress bar stable*/
.barForeground-2kwBa_ {
  background-color: var(--Main-Color);
}
/*Progress bar when hover on a tier level*/
.barSecondary-VouwoY {
  background-color: var(--Third-Color);
}

/*Tiers*/
.theme-dark .tierMarkerBackground-G8FoN4 {
  background-color: var(--Third-Color);
}

/*"Get cool rewards for becoming a Booster!" the 3 cards below*/
.perks-BtAudq {
  background: transparent;
}
.theme-dark .perk-19D_HN {
  background-color: transparent;
}

/*"Read to boost?" card from below*/
.wrapper-3Zq_cJ {
  background: transparent;
  color: var(--Main-Color);
  border-color: rgb(var(--Neon-Rgb));
  box-shadow: inset 0px 0px 5px 1px rgb(var(--Neon-Rgb)), 0px 0px 15px 4px rgb(var(--Neon-Rgb));
}
/*"Learn more about discord nitro button" color and background*/
/*normal*/
.lookInverted-2mDUMi.colorBrand-I6CyqQ {
  color: var(--Main-Color);
  background-color: transparent;
}
/*hover*/
.lookInverted-2mDUMi.colorBrand-I6CyqQ:hover {
  color: var(--Black);
  background-color: var(--Secondary-Color);
}


/*
 $$$$$$\                                                            $$$$$$\              $$\       $$\     $$\                               
$$  __$$\                                                          $$  __$$\             $$ |      $$ |    \__|                              
$$ /  \__| $$$$$$\   $$$$$$\  $$\    $$\  $$$$$$\   $$$$$$\        $$ /  \__| $$$$$$\  $$$$$$\   $$$$$$\   $$\ $$$$$$$\   $$$$$$\   $$$$$$$\ 
\$$$$$$\  $$  __$$\ $$  __$$\ \$$\  $$  |$$  __$$\ $$  __$$\       \$$$$$$\  $$  __$$\ \_$$  _|  \_$$  _|  $$ |$$  __$$\ $$  __$$\ $$  _____|
 \____$$\ $$$$$$$$ |$$ |  \__| \$$\$$  / $$$$$$$$ |$$ |  \__|       \____$$\ $$$$$$$$ |  $$ |      $$ |    $$ |$$ |  $$ |$$ /  $$ |\$$$$$$\  
$$\   $$ |$$   ____|$$ |        \$$$  /  $$   ____|$$ |            $$\   $$ |$$   ____|  $$ |$$\   $$ |$$\ $$ |$$ |  $$ |$$ |  $$ | \____$$\ 
\$$$$$$  |\$$$$$$$\ $$ |         \$  /   \$$$$$$$\ $$ |            \$$$$$$  |\$$$$$$$\   \$$$$  |  \$$$$  |$$ |$$ |  $$ |\$$$$$$$ |$$$$$$$  |
 \______/  \_______|\__|          \_/     \_______|\__|             \______/  \_______|   \____/    \____/ \__|\__|  \__| \____$$ |\_______/ 
                                                                                                                         $$\   $$ |
                                                                                                                         \$$$$$$  |
                                                                                                                          \______/
Sidebar > Category headers ("Guild name", "Community", "User Management") colors*/
.header-2Kx1US {
  color: var(--Main-Color);
}
/*Sidebar > Sub-category colors*/
/*Default*/
.brand-3g5E0C.item-3XjbnG, .themed-2-lozF.item-3XjbnG {
  color: var(--White-Second);
}
/*Hover*/
.side-2ur1Qk .themed-2-lozF.item-3XjbnG:hover:not(.disabled-1nofHP), .topPill-3DJJNV .themed-2-lozF.item-3XjbnG:hover:not(.disabled-1nofHP) {
  background-color: transparent;
  color: var(--Main-Color);
}
/*When sub-category selected > border and color*/
.brand-3g5E0C.item-3XjbnG, .themed-2-lozF.item-3XjbnG[aria-selected=true] {
  color: var(--Main-Color);
  border-left: 2px solid var(--Main-Color);
}

/*Server boost status color text and background*/
.serverBoostTabItem-3QwA3W[aria-selected=true] {
  background-color: transparent!important;
  color: var(--Main-Color)!important;
  border-left: 2px solid var(--Main-Color)!important;
}

/*All buttons*/
.container-2nx-BQ {
  opacity: 0.3;
  background-color: var(--Secondary-Color)!important;
}

/* #################### Overview #################### */
/*All spacers*/
.theme-dark .divider--oiTeJ {
  border-color: var(--Third-Color);
}

/*Server overview*/
.defaultColor-2cKwKo {
  color: var(--Main-Color);
}

/*All titles ("Server name", "Inactive channel", "Inactive timeout", "System message channel", "Default notification settings", "Server banned background lvl2", "Server invite background lvl1")*/
.h5-2RwDNl {
  color: var(--Main-Color);
}

/*All disabled dropdowns*/
.select-1Ia3hD, .wrapper-1b33hy {
  color: var(--Secondary-Color);
}

/*All sub dropdowns*/
.colorStandard-21JIj7 {
  color: var(--Secondary-Color);
}

/*Remove button under the photo*/
.removeButton-2apMfV {
  color: var(--Main-Color);
}
.removeButton-2apMfV:hover {
  color: var(--Secondary-Color);
}

/*Photo description*/
.description-30xx7u, .labelDescriptor-34wZ-z {
  color: var(--White-Second);
}

/*Upload Image button*/
.theme-dark .lookOutlined-3yKVGo.colorPrimary-2AuQVo {
  color: var(--Main-Color);
  border-color: var(--border2);
  background-color: transparent;
}
.theme-dark .lookOutlined-3yKVGo.colorPrimary-2AuQVo:hover {
  color: var(--Secondary-Color);
  border-color: var(--border3);
  background-color: transparent;
}

/*System messages channel disabled messages*/
.title-2dsDLn {
  color: var(--Secondary-Color);
}

/*Default notification settings, circle buttons*/
.radioIconForeground-2BMavi {
  color: var(--Secondary-Color);
}
/*"All messages", "Only @mentions" text color*/
.title-1yyp9V {
  color: var(--Secondary-Color);
}

/*Display > Show boost progress bar*/
.colorInteractiveActive-30E9n8 {
  color: var(--Secondary-Color);
}

/*"Server banner background", "Server invite background", "Unlock with boosting" buttons color*/
/*Normal*/
.lookFilled-yCfaCM.colorGreen-3y-Z79 {
  color: var(--Main-Color);
  background-color: var(--Third-Color);
}
/*Hover*/
.lookFilled-yCfaCM.colorGreen-3y-Z79:hover {
  color: var(--Secondary-Color);
  background-color: var(--Color-4);
}

/* #################### Roles #################### */
/*The descriptions under "Roles", "Search Roles"*/
.colorHeaderSecondary-g5teka {
  color: var(--Secondary-Color);
}
/*Default Permissions, icon and description*/
.icon-2DGsye {
  color: var(--Secondary-Color);
}
/*"Default permissions" text*/
.label-2Pe5f1 {
  color: var(--Secondary-Color);
}
/*"@everyone * applies to all server members" text*/
.size12-oc4dx4 {
  color: var(--Secondary-Color);
}

/*The arrow icon*/
.arrow-2v2Yl2 {
  color: var(--Secondary-Color);
}

/*Search roles input*/
.input-2m5SfJ {
  color: var(--Secondary-Color);
}

/*Create role button*/
/*Normal*/
.lookFilled-yCfaCM.colorBrand-I6CyqQ {
  color: var(--Main-Color);
  background-color: transparent;
  border-color: rgb(var(--Neon-Rgb));
  box-shadow: inset 0px 0px 5px 1px rgb(var(--Neon-Rgb)), 0px 0px 15px 4px rgb(var(--Neon-Rgb));
}
/*Hover*/
.lookFilled-yCfaCM.colorBrand-I6CyqQ:hover {
  color: var(--Secondary-Color);
  background-color: transparent;
  border-color: rgb(var(--Neon-Rgb));
  box-shadow: inset 0px 0px 5px 1px rgb(var(--Neon-Rgb)), 0px 0px 15px 4px rgb(var(--Neon-Rgb));
}

/* ########## Roles > Default permissions tab ########## */
/*Back button*/
/*Normal*/
.title-JU0E7C {
  color: var(--Main-Color);
}
/*Hover*/
.title-JU0E7C:hover {
  color: var(--Secondary-Color);
}

/*Create new role "+" icon*/
.addRole-viKZpC {
  color: var(--Main-Color);
}

/*The container for edit role, display, permissions, manager members, edit role and the 3 dots*/
.header-JUTO-g {
  background-color: var(--Black);
}

/*Edit role <role-name>*/
.titleText-35PD5k {
  color: var(--Main-Color);
}

/*The 3 dots, the menu*/
.menu-2p630X {
  color: var(--Main-Color);
}

/*Role icon > Choose image button*/
/*Normal*/
.lookOutlined-3yKVGo.colorWhite-1H92hK {
  color: var(--Main-Color);
  border: var(--border2);
}
.lookOutlined-3yKVGo.colorWhite-1H92hK:hover {
  color: var(--Secondary-Color);
  border: var(--border3);
}

/*View server as role button*/
/*Normal*/
.theme-dark .lookFilled-yCfaCM.colorGrey-2iAG-B {
  color: var(--Main-Color);
  background-color: transparent;
  border: var(--border2);
}
/*Hover*/
.theme-dark .lookFilled-yCfaCM.colorGrey-2iAG-B:hover {
  color: var(--Secondary-Color);
  background-color: transparent;
  border: var(--border3);
}

/* #################### Stickers tab #################### */
/*Get boosted card background*/
.upsellContainer-22N_CL {
  background-color: transparent!important;
  background: transparent!important;
  border-color: rgb(var(--Neon-Rgb));
  box-shadow: inset 0px 0px 5px 1px rgb(var(--Neon-Rgb)), 0px 0px 15px 4px rgb(var(--Neon-Rgb));
}
/*Get boosted card description under "Get boosted"*/
.upsellDescription-2O_p3B {
 color: var(--White-Second);
}
/*Both buttons backgrounds*/
/*normal*/
.lookFilled-yCfaCM.colorWhite-1H92hK {
  background-color: transparent;
  border-color: rgb(var(--Neon-Rgb));
  box-shadow: inset 0px 0px 5px 1px rgb(var(--Neon-Rgb)), 0px 0px 15px 4px rgb(var(--Neon-Rgb));
}
/*hover*/
.lookFilled-yCfaCM.colorWhite-1H92hK:hover {
  background-color: var(--Third-Color);
  border-color: rgb(var(--Neon-Rgb));
  box-shadow: inset 0px 0px 5px 1px rgb(var(--Neon-Rgb)), 0px 0px 15px 4px rgb(var(--Neon-Rgb));
}

/*Level cards (1,2,3)*/
/*border*/
.tier-3CS7-p {
  border-color: rgb(var(--Neon-Rgb));
  box-shadow: inset 0px 0px 5px 1px rgb(var(--Neon-Rgb)), 0px 0px 15px 4px rgb(var(--Neon-Rgb));
}
/*top tier header*/
.theme-dark .tierHeaderLocked-30MLlO {
  background-color: transparent;
}
/*second tier body (middle)*/
.theme-dark .tierBody-1d3UiS {
  background-color: transparent;
}

/* #################### Widgets tab #################### */
.theme-dark .copyInputDefault-3jiMHw {
  background-color: transparent;
  border-color: rgb(var(--Neon-Rgb));
  box-shadow: inset 0px 0px 5px 1px rgb(var(--Neon-Rgb)), 0px 0px 15px 4px rgb(var(--Neon-Rgb));
}

/* #################### Community tab #################### */
/*"Are you building a community?" text colors*/
.wrapper-1HSdhi {
  margin: 0;
  color: var(--Main-Color);
}
/*"Grow your community", "Keep members engaged", "Stay informed" text colors*/
.base-21yXnu {
  font-weight: 600;
  font-family: var(--font-display);
  color: var(--Main-Color);
}
/*"Disable community" button*/
/*background*/
/*normal*/
.lookFilled-yCfaCM.colorRed-rQXKgM {
  background-color: transparent;
  border-color: rgb(var(--Neon-Rgb));
  box-shadow: inset 0px 0px 5px 1px rgb(var(--Neon-Rgb)), 0px 0px 15px 4px rgb(var(--Neon-Rgb));
}
/*text normal*/
.contents-3ca1mk {
  color: var(--Main-Color)!important;
}
/*background hover*/
.lookFilled-yCfaCM.colorRed-rQXKgM:hover {
  background-color: var(--Main-Color);
}
/*text hover*/
.contents-3ca1mk:hover {
  color: var(--White)!important;
}

/* #################### Members tab #################### */
/*"Display role" text color*/
.quickSelectLabel-ArUyd9 {
  color: var(--Main-Color);
}
/*"@everyone" text color*/
.quickSelectValue-rmtkbe {
  margin-left: 4px;
  color: var(--Main-Color);
}

/*
$$\   $$\                                      $$$$$$\              $$\       $$\     $$\                               
$$ |  $$ |                                    $$  __$$\             $$ |      $$ |    \__|                              
$$ |  $$ | $$$$$$$\  $$$$$$\   $$$$$$\        $$ /  \__| $$$$$$\  $$$$$$\   $$$$$$\   $$\ $$$$$$$\   $$$$$$\   $$$$$$$\ 
$$ |  $$ |$$  _____|$$  __$$\ $$  __$$\       \$$$$$$\  $$  __$$\ \_$$  _|  \_$$  _|  $$ |$$  __$$\ $$  __$$\ $$  _____|
$$ |  $$ |\$$$$$$\  $$$$$$$$ |$$ |  \__|       \____$$\ $$$$$$$$ |  $$ |      $$ |    $$ |$$ |  $$ |$$ /  $$ |\$$$$$$\  
$$ |  $$ | \____$$\ $$   ____|$$ |            $$\   $$ |$$   ____|  $$ |$$\   $$ |$$\ $$ |$$ |  $$ |$$ |  $$ | \____$$\ 
\$$$$$$  |$$$$$$$  |\$$$$$$$\ $$ |            \$$$$$$  |\$$$$$$$\   \$$$$  |  \$$$$  |$$ |$$ |  $$ |\$$$$$$$ |$$$$$$$  |
 \______/ \_______/  \_______|\__|             \______/  \_______|   \____/    \____/ \__|\__|  \__| \____$$ |\_______/ 
                                                                                                    $$\   $$ |
                                                                                                    \$$$$$$  |
                                                                                                     \______/
#################### My account tab ####################*/
/*Name, email, phone number colors*/
.colorHeaderPrimary-jN_yGr {
  color: var(--Main-Color);
}

/*Name, email, phone number buttons colors*/
/*Normal*/
.lookFilled-yCfaCM.colorPrimary-2AuQVo {
  color: var(--Main-Color);
  background-color: transparent;
  border-color: rgb(var(--Neon-Rgb));
  box-shadow: inset 0px 0px 5px 1px rgb(var(--Neon-Rgb)), 0px 0px 15px 4px rgb(var(--Neon-Rgb));
}
/*Hover*/
.lookFilled-yCfaCM.colorPrimary-2AuQVo:hover {
  background-color: var(--Secondary-Color);
}

/*Phone number "remove" & "Change Phone Number?" messages colors*/
/*Normal*/
.theme-dark .lookLink-15mFoz.colorPrimary-2AuQVo {
  color: var(--Main-Color);
}
/*Hover*/
.theme-dark .lookLink-15mFoz.colorPrimary-2AuQVo:hover .contents-3ca1mk {
  background-image: linear-gradient(0deg,transparent,transparent 1px,var(--Main-Color) 0,var(--Main-Color) 2px,transparent 0);
}

/* #################### User profile tab #################### */
/*"About me" text area background*/
.bioTextArea-dDGOeC {
  background-color: transparent;
  --channel-text-area-placeholder: var(--input-placeholder-text);
  border-color: rgb(var(--Neon-Rgb));
  box-shadow: inset 0px 0px 5px 1px rgb(var(--Neon-Rgb)), 0px 0px 15px 4px rgb(var(--Neon-Rgb));
}

/* User popout preview */
.preview-Z55SA3 {
  border-color: rgb(var(--Neon-Rgb));
  box-shadow: inset 0px 0px 5px 1px rgb(var(--Neon-Rgb)), 0px 0px 15px 4px rgb(var(--Neon-Rgb));
}
/* Disable Banner */
.bannerNitroUpsell-2iP18z {
  display: none;
}
.banner-3D8GgT {
  width: 0%;
}
/*"Avatar, Profile color, Preview, Profile Banner, About me" text paddings*/
.defaultMarginh5-3Jxf6f {
  padding-top: 5px;
  padding-left: 5px;
}

/*#################### Privacy and safety ####################*/
/*Request data button color*/
/*Button border and background*/
/*Normal*/
.lookOutlined-3yKVGo.colorBrand-I6CyqQ {
  color: var(--Main-Color);
  border-color: rgb(var(--Neon-Rgb));
  box-shadow: inset 0px 0px 5px 1px rgb(var(--Neon-Rgb)), 0px 0px 15px 4px rgb(var(--Neon-Rgb));
}
/*Hover*/
.lookOutlined-3yKVGo.colorBrand-I6CyqQ:hover {
  background-color: var(--Secondary-Color);
  border-color: rgb(var(--Neon-Rgb));
  box-shadow: inset 0px 0px 5px 1px rgb(var(--Neon-Rgb)), 0px 0px 15px 4px rgb(var(--Neon-Rgb));
}
/*Text*/
.contents-3ca1mk {
  color: var(--Main-Color);
}

/*#################### Server boost tab ####################*/
/*"Server boost" message*/
.marketingLogoIcon-3HQY2K {
  color: var(--Main-Color);
}

/*"Boost a server and get" & "Boosted servers can get" messages*/
.base-21yXnu.muted-eZM05q {
  color: var(--Main-Color);
}
/*All descriptions*/
.descriptionStandalone-3ChjDk {
  color: var(--Main-Color);
}

/*#################### Subscriptions tab ####################*/
/*"Your subscriptions" description text message */
.sectionDescription-2ealM1 {
  color: var(--Main-Color);
}
/*"Subscription credit" description text message */ 
.accountCreditDescription-1lEaJI {
  color: var(--Main-Color);
}
/*"Your subscriptions" "You have no active subscriptions" text message*/
.cardText-1KLO-g {
  color: var(--Main-Color);
}
/*"Subscription credit" "You have no unused credits"*/
.cardText-3dmnX6 {
  color: var(--Main-Color);
}

/*#################### Gift inventory ####################*/
/*"Reedem codes" text area input*/
.input-2g-os5 {
  color: var(--Main-Color);
  background-color: transparent;
  border-color: none;
}

/*#################### Biling ####################*/
/*Transaction history*/
/*"Date", "Description" & "Amount"*/
.theme-dark .paymentPane-ut5qKZ {
  background-color: transparent;
  color: var(--Main-Color);
}
/*Under container details and background*/
.theme-dark .paginator-1eqD2g {
  background: transparent;
}
.theme-dark .bottomDivider-ZmTm-j {
  background-color: transparent;
}

/*"Psst! Looking to redeem a Discord key? We've moved it to" message and card*/
.theme-dark .codeRedemptionRedirect-2hYMSQ {
  color: var(--Main-Color);
  background-color: transparent;
  border-color: rgb(var(--Neon-Rgb));
  box-shadow: inset 0px 0px 5px 1px rgb(var(--Neon-Rgb)), 0px 0px 15px 4px rgb(var(--Neon-Rgb));
}

/*#################### Activity status ####################*/
/*Add a new game popout*/
.theme-dark .addGamePopout-2SKNIV {
  background: linear-gradient(rgba(0, 0, 0, 0.7),rgba(0, 0, 0, 0.6)) , var(--background-black-and-white1) 50% 50%/cover !important;
  border-color: rgb(var(--Neon-Rgb));
  box-shadow: inset 0px 0px 5px 1px rgb(var(--Neon-Rgb)), 0px 0px 15px 4px rgb(var(--Neon-Rgb));
}
/*"Select" background card*/
.lookFilled-1GseHa.select-1Ia3hD {
  background-color: transparent;
  border-color: rgb(var(--Neon-Rgb));
  box-shadow: inset 0px 0px 2px 1px rgb(var(--Neon-Rgb)), 0px 0px 5px 1px rgb(var(--Neon-Rgb));
}
/*Select background game popout*/
.popout-1KHNAq {
  background: linear-gradient(rgba(0, 0, 0, 0.7),rgba(0, 0, 0, 0.6)) , var(--background-black-and-white1) 50% 50%/cover !important;
}

/*
$$\      $$\                       $$\     $$\                               
$$$\    $$$ |                      $$ |    \__|                              
$$$$\  $$$$ | $$$$$$\  $$$$$$$\  $$$$$$\   $$\  $$$$$$\  $$$$$$$\   $$$$$$$\ 
$$\$$\$$ $$ |$$  __$$\ $$  __$$\ \_$$  _|  $$ |$$  __$$\ $$  __$$\ $$  _____|
$$ \$$$  $$ |$$$$$$$$ |$$ |  $$ |  $$ |    $$ |$$ /  $$ |$$ |  $$ |\$$$$$$\  
$$ |\$  /$$ |$$   ____|$$ |  $$ |  $$ |$$\ $$ |$$ |  $$ |$$ |  $$ | \____$$\ 
$$ | \_/ $$ |\$$$$$$$\ $$ |  $$ |  \$$$$  |$$ |\$$$$$$  |$$ |  $$ |$$$$$$$  |
\__|     \__| \_______|\__|  \__|   \____/ \__| \______/ \__|  \__|\_______/
In guild channels*/
/*Mentioned background (the yellow name)*/
.mentioned-Tre-dv {
  position: relative;
  background-color: var(--background-primary);
}
.mentioned-Tre-dv:before {
  background-color: var(--background-primary);
}

/*Unread mentioned badge after channel in guild*/
.mentionsBadge-3H1BKJ {
  pointer-events: none;
}
.numberBadge-37OJ3S base-3IDx3L baseShapeRound-3epLEv children-1MGS9G {
  background-color: black!important;
  width: 16px;
}

/*
$$$$$$$$\           $$\                           $$\                 $$$$$$$$\           $$\       
$$  _____|          \__|                          $$ |                \__$$  __|          $$ |      
$$ |       $$$$$$\  $$\  $$$$$$\  $$$$$$$\   $$$$$$$ | $$$$$$$\          $$ |    $$$$$$\  $$$$$$$\  
$$$$$\    $$  __$$\ $$ |$$  __$$\ $$  __$$\ $$  __$$ |$$  _____|         $$ |    \____$$\ $$  __$$\ 
$$  __|   $$ |  \__|$$ |$$$$$$$$ |$$ |  $$ |$$ /  $$ |\$$$$$$\           $$ |    $$$$$$$ |$$ |  $$ |
$$ |      $$ |      $$ |$$   ____|$$ |  $$ |$$ |  $$ | \____$$\          $$ |   $$  __$$ |$$ |  $$ |
$$ |      $$ |      $$ |\$$$$$$$\ $$ |  $$ |\$$$$$$$ |$$$$$$$  |         $$ |   \$$$$$$$ |$$$$$$$  |
\__|      \__|      \__| \_______|\__|  \__| \_______|\_______/          \__|    \_______|\_______/ 
Main container background*/
.theme-dark .container-2cd8Mz {
  background-color: transparent;
}
/*Activity cards background "In a voice channel"*/
.theme-dark .inset-SbsSFp {
  background-color: transparent;
}
.theme-dark .outer-2JOHae.active-1W_Gl9, .theme-dark .outer-2JOHae.interactive-2zD88a:hover {
  background-color: transparent;
}

/*
$$$$$$$\                  $$\ $$\           $$\        $$$$$$\    $$\                 $$\                         
$$  __$$\                 $$ |\__|          $$ |      $$  __$$\   $$ |                $$ |                        
$$ |  $$ | $$$$$$\   $$$$$$$ |$$\  $$$$$$\  $$ |      $$ /  \__|$$$$$$\    $$$$$$\  $$$$$$\   $$\   $$\  $$$$$$$\ 
$$$$$$$  | \____$$\ $$  __$$ |$$ | \____$$\ $$ |      \$$$$$$\  \_$$  _|   \____$$\ \_$$  _|  $$ |  $$ |$$  _____|
$$  __$$<  $$$$$$$ |$$ /  $$ |$$ | $$$$$$$ |$$ |       \____$$\   $$ |     $$$$$$$ |  $$ |    $$ |  $$ |\$$$$$$\  
$$ |  $$ |$$  __$$ |$$ |  $$ |$$ |$$  __$$ |$$ |      $$\   $$ |  $$ |$$\ $$  __$$ |  $$ |$$\ $$ |  $$ | \____$$\ 
$$ |  $$ |\$$$$$$$ |\$$$$$$$ |$$ |\$$$$$$$ |$$ |      \$$$$$$  |  \$$$$  |\$$$$$$$ |  \$$$$  |\$$$$$$  |$$$$$$$  |
\__|  \__| \_______| \_______|\__| \_______|\__|       \______/    \____/  \_______|   \____/  \______/ \_______/ 
Idle status color to white status color*/
.status-2DiCMd {
  width: 100%;
  height: 100%;
  background-color: var(--Black-Color);
}
.pointerEvents-9SZWKj {
  pointer-events: auto;
  background-color: rgb(0,0,0) !important;
  color: rgb(0,0,0) !important;
}

/*
$$$$$$$\                                                                              $$\     
$$  __$$\                                                                             $$ |    
$$ |  $$ | $$$$$$\   $$$$$$\  $$$$$$\$$$$\   $$$$$$\  $$$$$$$\   $$$$$$\  $$$$$$$\  $$$$$$\   
$$$$$$$  |$$  __$$\ $$  __$$\ $$  _$$  _$$\  \____$$\ $$  __$$\ $$  __$$\ $$  __$$\ \_$$  _|  
$$  ____/ $$$$$$$$ |$$ |  \__|$$ / $$ / $$ | $$$$$$$ |$$ |  $$ |$$$$$$$$ |$$ |  $$ |  $$ |    
$$ |      $$   ____|$$ |      $$ | $$ | $$ |$$  __$$ |$$ |  $$ |$$   ____|$$ |  $$ |  $$ |$$\ 
$$ |      \$$$$$$$\ $$ |      $$ | $$ | $$ |\$$$$$$$ |$$ |  $$ |\$$$$$$$\ $$ |  $$ |  \$$$$  |
\__|       \_______|\__|      \__| \__| \__| \_______|\__|  \__| \_______|\__|  \__|   \____/ 
Permanent things that you always see.
Titlebar top buttons colors. Close, rezise and hide*/
.winButton-3UMjdg {
  color: var(--Main-Color);
}
/*Hide discord text from titlebar*/
.wordmarkWindows-2dq6rw {
  display: none;
}

/*Close pannel "ESC" button*/
/*normal*/
.closeButton-PCZcma, .keybind-13vtq8 {
  color: var(--Main-Color);
}
.closeButton-PCZcma:hover, .keybind-13vtq8:hover {
  color: var(--Secondary-Color);
}
.closeButton-PCZcma:hover, .closeButton-PCZcma:hover+.keybind-13vtq8 {
  color: var(--Secondary-Color);
}

/*Message Input Area*/
.channelTextArea-1FufC0 {
  margin-bottom: 24px;
  background: linear-gradient(rgba(0, 0, 0, 0.8),rgba(0, 0, 0, 0.7)) , var(--loop-gif3) 10% 10%/cover !important;;
}

/*Atachements*/
/*Files*/
.attachment-1PZZB2 {
  border-color: rgb(var(--Neon-Rgb));
  box-shadow: inset 0px 0px 5px 1px rgb(var(--Neon-Rgb)), 0px 0px 15px 4px rgb(var(--Neon-Rgb));
  background: linear-gradient(rgba(0, 0, 0, 0.6),rgba(0, 0, 0, 0.8)) , var(--loop-gif) 50% 50%/cover !important;
}

/*"You are viewing older messages" popout*/
.jumpToPresentBar-1cEnH0 {
  border: none;
  background: linear-gradient(rgba(0, 0, 0, 0.6),rgba(0, 0, 0, 0.4)) , var(--background-black-and-white1) 50% 50%/cover !important;
}
/*"You are viewing older messages" color*/
.barButtonMain-2GIx4o {
  color: var(--Main-Color);
}
/*"Jump To Present" color*/
.barButtonAlt-TQoCdZ {
  color: var(--Main-Color);
}

/*Emoji popout*/
.emojiPickerInExpressionPicker-2nOwH8 .emojiPicker-6YCk8a {
  background: linear-gradient(rgba(0, 0, 0, 0.5),rgba(0, 0, 0, 0.8)) , var(--loop-gif5) 50% 100%/cover !important;
}
/*Emoji popout FROM message (icon click)*/
.emojiPicker-6YCk8a {
  background: linear-gradient(rgba(0, 0, 0, 0.5),rgba(0, 0, 0, 0.8)) , var(--loop-gif5) 50% 100%/cover !important;
}
/*Sticker & gif popouts*/
.emojiPickerInExpressionPicker-2nOwH8, .wrapper-1NB3WY, .container-3u7RcY {
  background: linear-gradient(rgba(0, 0, 0, 0.5),rgba(0, 0, 0, 0.8)) , var(--loop-gif5) 50% 100%/cover !important;
}
/*Gif popout, favorite fade*/
.theme-dark .categoryFadeBlurple-1l49_Q, .theme-light .categoryFadeBlurple-1l49_Q {
  background-color: transparent;
}

/*Nitro gift popout*/ /*Still need to work for the buttons and other thins*/
.theme-dark .root-g14mjS {
  background: linear-gradient(rgba(0, 0, 0, 0.5),rgba(0, 0, 0, 0.8)) , var(--loop-gif5) 50% 100%/cover !important;
  -webkit-box-shadow: 0 0 0 1px rgb(32 34 37 / 60%), 0 2px 10px 0 rgb(0 0 0 / 20%);
  box-shadow: 0 0 0 1px rgb(32 34 37 / 60%), 0 2px 10px 0 rgb(0 0 0 / 20%);
}
.tier2HeaderBackground-2XINxm {
  background-image: transparent!important;
}
.theme-dark .footer-31IekZ {
  background-color: transparent;
}

/*Pinned messages popout*/
.messagesPopoutWrap-3zryHW {
  background: linear-gradient(rgba(0, 0, 0, 0.8),rgba(0, 0, 0, 0.7)) , var(--loop-gif5) 50% 50%/cover !important;
}
/*Popout: the pinned message that u wanna pin*/
.theme-dark .message-G6O-Wv {
  background-color: transparent;
}
/*Inbox messages popout*/
.container-2ebMPP {
  background-color: black;
  border-color: rgb(var(--Neon-Rgb));
  box-shadow: inset 0px 0px 5px 2.5px rgb(var(--Neon-Rgb)), 0px 0px 15px 4px rgb(var(--Neon-Rgb));
}
/*Threads popout*/ 
.browser-mnQ1T7 {
  background-color: black;
  border-color: rgb(var(--Neon-Rgb));
  box-shadow: inset 0px 0px 5px 2.5px rgb(var(--Neon-Rgb)), 0px 0px 15px 4px rgb(var(--Neon-Rgb));
}

/*Click on friend profile then hover on photo ["View Profile" fix]*/
.avatarHint-k7pYop {
  position: absolute;
  top: 0%;
  left: 0%;
  opacity: 0;
}

/*Left click on friends tab popout*/
.menu-1QACrS {
  background: linear-gradient(rgba(0, 0, 0, 0.8),rgba(0, 0, 0, 0.7)) , var(--loop-gif5) 50% 50%/cover !important;
  border-color: rgb(var(--Neon-Rgb));
  box-shadow: inset 0px 0px 5px 2.5px rgb(var(--Neon-Rgb)), 0px 0px 15px 4px rgb(var(--Neon-Rgb));
}
/*Button clicked*/
.colorDefault-CDqZdO:active:not(.hideInteraction-2jPGL_) {
  background-color: transparent;
  color: var(--Main-Color);
}
/*Hover on buttons*/
.colorDefault-CDqZdO.focused-3qFvc8 {
  background-color: transparent;
  color: var(--Main-Color);
}

/*Click on emoji for informations (in channels/dms)*/
.popoutContainer-2wbmiM {
  width: 288px;
  border-color: rgb(var(--Neon-Rgb));
  box-shadow: inset 0px 0px 5px 2.5px rgb(var(--Neon-Rgb)), 0px 0px 15px 4px rgb(var(--Neon-Rgb));
  background: black;
}

/*Triple code blocks text format*/
.markup-eYLPri code {
  scrollbar-color: var(--Secondary-Color);
  background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.9)) , var(--background-black-and-white2) 50% 50%/cover no-repeat!important;
  border-color: rgb(var(--Neon-Rgb));
  box-shadow: inset 0px 0px 5px 1px rgb(var(--Neon-Rgb)), 0px 0px 15px 4px rgb(var(--Neon-Rgb));
}
/*Single and double code block text format*/
.markup-eYLPri code.inline {
  border: none!important;
  box-shadow: none;
}

/*Timestamps everywhere*/
.content-3spvdd {
  color: var(--text-muted);
  background: black;
  border: var(--border2);
  padding: 3px;
}
.divider-2rZFJK {
  border-top: var(--border2);
}

/*Emoji searching, matching When typing for an emoji in chat "ex: :wink"*/
.theme-dark .autocomplete-3NRXG8 {
  background: var(--Black);
  border-color: rgb(var(--Neon-Rgb));
  box-shadow: inset 0px 0px 5px 1px rgb(var(--Neon-Rgb)), 0px 0px 15px 4px rgb(var(--Neon-Rgb));
}
/*Found searched emoji, matched emoji*/
.theme-dark .selected-3H3-RC {
  background-color: transparent;
  border: var(--border2);
}

/*CTRL+F Search & find messages popout*/
.theme-dark .container-2McqkF {
  background: linear-gradient(rgba(0, 0, 0, 0.6),rgba(0, 0, 0, 0.6)) , var(--background-black-and-white1) 50% 50%/cover !important;;
}
/*Also in this popout, the last thing thing from a button*/
.option-ayUoaq:after {
  display: none!important;
}
/*CTRL+F After search popout*/
.searchResultsWrap-5RVOkx {
  background-color: black;
  border: var(--border2);
}
.theme-dark .focused-2FU0YH {
  background-color: transparent;
}

/*Disable home icon*/
.homeIcon-r0w4ny {
  display: none;
  width: 28px;
  height: 20px;
}

/*Custom background for home icon and for guilds with no photos*/
.childWrapper-1j_1ub {
  -webkit-transition: background-color .15s ease-out,color .15s ease-out;
  transition: background-color .15s ease-out,color .15s ease-out;
  background: linear-gradient(rgba(255, 0, 0, 0.4),rgba(255, 0, 0, 0.3)) , var(--loop-gif-diamond) 50% 100%/cover !important;
  color: var(--text-normal);
}

/*Screen share popout*/
/*Applications & Screens text colors*/
/*selected*/
.theme-dark .selected-2xa993 {
  color: var(--Main-Color);
  border-bottom: 2px solid var(--Main-Color);
}
/*normal*/
.item-LN5zvA {
  color: var(--Main-Color);
}
/*Go live button background color*/
.lookFilled-yCfaCM.colorBrand-I6CyqQ:disabled {
  background-color: var(--Secondary-Color);
}

/*Screen share popout after clicking on Go live button*/
/*"What you are streaming & Streaming channel" text, background, border colors*/
.card-m7VgZ8 {
  color: var(--Main-Color);
  border: none;
  background: transparent;
}
/*"What you are streaming" icons color*/
.selectedIcon-277z4I {
  color: var(--Main-Color);
}
/*"Streaming channel" icon color*/
.channelIcon-1BydE- {
  color: var(--Main-Color);
}

/*Reactions popout from "See reactions" background*/
.theme-dark .container-KM8BU6 {
  background-color: transparent;
}
.theme-dark .reactors-1VXca7 {
  background: linear-gradient(rgba(0, 0, 0, 0.5),rgba(0, 0, 0, 0.8)) , var(--loop-gif5) 50% 100%/cover !important;
}
.theme-dark .scroller-2GkvCq { 
  background-color: transparent;
}

/*User popout cards, fix "User info, Activity border-bottom"*/
.top-K_jibn .selected-g-kMVV.themed-2-lozF.item-3XjbnG, .top-K_jibn .themed-2-lozF.item-3XjbnG:active {
  border-bottom: none;
}
.top-K_jibn .selected-g-kMVV.themed-2-lozF.item-3XjbnG, .top-K_jibn .themed-2-lozF.item-3XjbnG {
  border-bottom: none;
}


