# Discord Hacker
Forked hrx404
# Discord Console Hacks

<details>
  <summary>Click here</summary>
  

## Info

As stated in hxr404's Disclaimer I don't promote using any kind of client modifications. Please don't use the code found here for illegal / hacking purposes, or you might risk seeing this error message:<br>

![image](https://user-images.githubusercontent.com/55095883/134189043-4da003de-4829-4d60-888a-6014ebb5c2b8.png)

  

## How to use these Hacks

It only works on Desktop Versions (Windows, Linux, MacOS), not on Mobile
1. Press CTRL + SHIFT + I to toggle Developer Tools (Discord is electronjs wich is basically google chrome)
2. Click on "Console" if not already selected
3. Paste the script in
4. Press enter

  ## Enable Staff Mode

<details>
<summary>Enables some hidden features and sets your client to staff mode</summary>
 
This will trick your client into thinking that you are Discord Staff (by modifiying the flags)
and also enables the secret experiments and Developer Options Menu (where you can get secret unrelesed discord updates, 
emulate a different client, generate build overrides etc.)
Credit for the Settings hack to https://gist.github.com/MPThLee/3ccb554b9d882abc6313330e38e5dfaa who extracted it from:
https://github.com/samogot/betterdiscord-plugins (The original Creator)

```js
window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.default && m.default.getCurrentUser !== undefined) {return m.default.getCurrentUser().flags += 1;}if (m.getCurrentUser !== undefined) {return m.getCurrentUser().flags += 1}}}]);window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.default && m.default.isDeveloper !== undefined) {Object.defineProperty(m.default, "isDeveloper", {get: (a) => 1,set: (a) => a,configurable: true}); console.log("%cWorked!", "font-size: 50px");return console.log(`%cYou now have Developer Options and a Staff badge. You can find the Developer Settings in the Settings's bottom tab!`, "font-size: 16px")}if (m.isDeveloper !== undefined) {Object.defineProperty(m, "isDeveloper", {get: (a) => 1,set: (a) => a,configurable: true}); console.log("%cWorked!", "font-size: 50px");return console.log(`%cYou now have Developer Options and a Staff badge. You can find the Developer Settings in the Settings's bottom tab!`, "font-size: 16px")}}}]);
```

</details>

![discorddevoptions](https://user-images.githubusercontent.com/55095883/116668009-29223780-a99d-11eb-9387-625f10c64196.png)

<sup>Developer Options Setting</sup>
<br>

## Get all Badges

<details>
  <summary>This script enables all Badges on you client.</summary>

Note that other users won't see the badge<br>

```js
window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.default && m.default.getCurrentUser !== undefined) {return m.default.getCurrentUser().flags = -1;}if (m.getCurrentUser !== undefined) {return m.getCurrentUser().flags = -1}}}]);window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.default && m.default.getCurrentUser !== undefined) {return m.default.getCurrentUser().public_flags += 1;}if (m.getCurrentUser !== undefined) {return m.getCurrentUser().public_flags += 1}}}]);
```

</details>

![preview](https://user-images.githubusercontent.com/55095883/110086787-191e1b00-7d93-11eb-8f0f-2b3a76210155.png)

<br>
<sup>This isn't a fake screenshot your client will really display this.</sup>
<br><br>

## Easy Edit mode

<details>
<summary>you can use this to make Fake Screenshots without having to do Inspect Element each time</summary>

```js
document.designMode = 'on'
```

</details>
<br>

## Free Discord Nitro (hack)

<details>
  <summary>Get some Nitro features without buying Nitro</summary>
 
Tricks your client into thinking you have Nitro. Converts the API request into non-nitro requests, so Discord won't notice that yoou don't have Nitro.
Be extra careful with scripts that claim to do this, this script is the only working one. If you find a copy of this script, not directly provided by me or this repo, pls report it to me, its probably a scam.<br>
Credit to https://github.com/An00nymushun/DiscordFreeEmojis for the Emoji handling part.<br>
Note that not every feature is supported as, some things that run Server Side can't be simulated.
But basic features (like animated emojis) should work.

```js
/*
I removed the code bc this shouldn't go public. Ppl would just copy and paste this anywhere and bad ppl would backdoor it.
Also I don't want Discord to fix this.

This script was replaced by Discord Oxygen.
*/
```
</details>

![grafik](https://user-images.githubusercontent.com/55095883/116668188-5d95f380-a99d-11eb-96cf-a0e2dfc6bb23.png)

<sup>The Subscription Overview. The Account used for the Screenshot **didn't** buy Nitro</sup>
<br>

## View NSFW Channels

<details>
  <summary>Displays NSFW Channels On A below 18 account.</summary>
<br>
  
Only use this script if you are 18+!
```js
var findModule=(item)=>window.webpackChunkdiscord_app.push([[Math.random()],{},(req)=>{for(const m of Object.keys(req.c).map((x)=>req.c[x].exports).filter((x)=>x)){if(m.default&&m.default[item]!==undefined)return m.default}}])
findModule('getCurrentUser').getCurrentUser().nsfwAllowed = true
```

</details>
  
![grafik](https://raw.githubusercontent.com/PndaBoi/pndaboi/main/6zsLEjYET0.png)

<br>
<sup>Before Running The Script ^^</sup><bbr>
<br>
  
![grafik](https://raw.githubusercontent.com/PndaBoi/pndaboi/main/ypzEY7Yw0u.png)

<br>
<sup>After Running The Script ^^</sup><bbr>
<br>
  


## Get hidden Channel ID's

<details>
  <summary>Displays the ID's of channel that you can't see without hacks.</summary>

```js
window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.default && m.default.getPrivateChannelIds !== undefined) {return console.log(m.default.getPrivateChannelIds())}if (m.getPrivateChannelIds !== undefined) {return console.log(m.getPrivateChannelIds())}}}]);
```

</details>

![grafik](https://user-images.githubusercontent.com/55095883/116670257-cda57900-a99f-11eb-8f96-7d8d54754535.png)

<br>
<sup>Example Output of this command</sup><bbr>
<br>
  

## Changing Password

<details>
  <summary>Change the Password of the Account, thats currently logged in.</summary>

  

```js
  let oldpassword = "";
  let newpassword = "";

  window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.default && m.default.getToken !== undefined) {fetch("https://discord.com/api/v9/users/@me", { "credentials": "include", "body": "{\"password\":\"" + oldpassword + "\",\"new_password\":\"" + newpassword + "\"}", "method": "PATCH", "headers": { "Authorization": m.default.getToken(), "Content-Type":"application/json" }}); return}if (m.getToken !== undefined) {fetch("https://discord.com/api/v9/users/@me", {"credentials": "include","body": "{\"password\":\"" + oldpassword + "\",\"new_password\":\"" + newpassword + "\"}","method":"PATCH","headers": {"Authorization": m.getToken(), "Content-Type":"application/json"}});return}}}]);
```

</details>
  
  ## Add guild features
<details>
  <summary>Enable server features... Replace 'FEATURE' with something like 'PARTNERED' or 'VERIFIED'<br><img src="https://user-images.githubusercontent.com/55095883/121220849-4a702080-c885-11eb-965c-317749da0196.png"></img>

<img src="https://user-images.githubusercontent.com/55095883/121219947-7b9c2100-c884-11eb-99f1-e0a8525512a9.png"></img><img src="https://user-images.githubusercontent.com/55095883/121220469-e9484d00-c884-11eb-816f-2d3b9f46a585.png"></img>)
</summary>

Unknown Author.

```js
let serverid = "";
let feature = "";

window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.default && m.default.getGuilds !== undefined) {return m.default.getGuild(serverid).features.add(feature)}if (m.getGuilds !== undefined) {return m.getGuild(serverid).features.add(feature)}}}]);
```

</details>

## Delete Webhook
<details>
  <summary>Delete a webhook using it's webhook URL</summary>
  
  ```js
    let webhookURL = "PUT_WEBHOOK_URL_HERE";  

    await fetch(webhookURL, {
      "method": "DELETE",
    });
  ```
</details>

## Phone, Email verification bypass

<details>
  <summary>Bypass Phone and email verification in server, this cannot let you send message but you still can connect and and talk in voice channels
</summary>


```js
window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.default && m.default.getCurrentUser !== undefined) {return m.default.getCurrentUser().phone = '+1234567890';}if (m.getCurrentUser !== undefined) {return m.getCurrentUser().phone = '+1234567890'}}}]);
window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.default && m.default.getCurrentUser !== undefined) {return m.default.getCurrentUser().email = 'email@email.com';}if (m.getCurrentUser !== undefined) {return m.getCurrentUser().email = 'email@email.com'}}}]);
window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.default && m.default.getCurrentUser !== undefined) {return m.default.getCurrentUser().verified = true;}if (m.getCurrentUser !== undefined) {return m.getCurrentUser().verified = true}}}]);
```

</details>

## Change Client Color

<details>
  <summary>Changes Your Client Color To Your Liking.<br><img src="https://cdn.discordapp.com/attachments/841333120870645760/858800547958882334/unknown.png"></img>
</summary>

Unknown Author.
```js
__SECRET_EMOTION__.injectGlobal(`
    * {
--background-primary: #000000;
    --background-secondary: #000000;
--background-secondary-alt: #070707ff;
--background-accent: #252525;
--background-floating: #242424ff;
    --scrollbar-thin-track: #000000;
    --channeltextarea-background: #151515;
    }
`)
```

</details>

</details>


# The Framework

<details>
  <summary>Click here</summary>
  
  Now in a seperate repo: https://github.com/hxr404/discord-oxygen
  
The Framework is a new project, wich combines every Console Hack into a single script.<br>
Simply Include the source code (.js file) into your Discord Client (Desktop or Web).<br>
You can either do this by pasting it into your Console (CTRL + SHIFT + I, CTRL + V, ENTER)<br>
Or by adding it as a Userscript. (You need a Browser Extension, for Firefox I recommend Firemonkey)<br>

## How it works

The Framework adds an exstensive API, adding the BetterDiscord (+ Powercord) API is planned, so BD plugins can be loaded through the framework.
Its similar to a modloader of a game, except for it is preconfigured and all good mods are already installed (Open a PR or issue if you want to merge your mods to mainstream)
Its modularized and each module runs seperatetly in its own Block Scope, not like the Old Nitro hack.
This should prevent Discord from fixing it, as it no longer depends on hardcoded modifications.

## Features:

<details>
  <summary>Screenhots will be added here</summary>
</details>
 

## History

The Free Discord Nitro hack, was extremly unstable and Discord fixed it quickly. Thats when I started working on the Framework. It was the improved Discord Nitro.
It is much more performant, offers better UX and made development way easier. After successfully merging the old Nitro hack, I continued improving Nitro with more features. And then I thought: why only adding default Nitro features? There are much more awesome features that can be useful as well. And since the Framwerork is modularized, it took about 5 Minutes merging the other Console hacks. And like this a new project was born.
  
  
</details>
