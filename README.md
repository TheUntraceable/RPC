<div align="center">
  <br />
  <p>
    <a href="https://www.npmjs.com/package/@theuntraceable/discord-rpc"><img src="https://img.shields.io/npm/v/discord-rpc.svg?maxAge=3600" alt="NPM version" /></a>
    <a href="https://www.npmjs.com/package/@theuntraceable/discord-rpc"><img src="https://img.shields.io/npm/dt/discord-rpc.svg?maxAge=3600" alt="NPM downloads" /></a>
    <a href="https://david-dm.org/discordjs/RPC"><img src="https://img.shields.io/david/discordjs/RPC.svg?maxAge=3600" alt="Dependencies" /></a>
  </p>
  <p>
    <a href="https://nodei.co/npm/discord-rpc/"><img src="https://nodei.co/npm/discord-rpc.png?downloads=true&stars=true" alt="NPM info" /></a>
  </p>
</div>

# Discord.js RPC Extension

### [Documentation](https://discord.js.org/#/docs/rpc/)

### ~~[Rich Presence Example](https://github.com/TheUntraceable/RPC/blob/master/example)~~ Will fix soon.

### __Browser__ Example

```javascript
const clientId = '743122320838623338';
const scopes = ['rpc', 'rpc.api', 'messages.read'];

const client = new RPC.Client({ transport: 'websocket' });

client.on('ready', () => {
  console.log('Logged in as', client.application.name);
  console.log('Authed for user', client.user.username);

  client.selectVoiceChannel('81384788862181376');
});

// Log in to RPC with client id
client.login({ clientId, scopes });
```