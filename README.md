//Setup:
console.log("Starting bot");
//Imports the discord.js API to interact with Discord
const { Client } = require("discord.js");
const client = new Client();
//Start a web server so Replit keeps the bot running
//const keep_alive = require('./keep_alive.js');
//Brings in the token from the .env file
const token = process.env.BOT_TOKEN;
//Using a variable for the prefix makes it easy to change later
const prefix = "";

//Confirm that the bot has logged in
client.on("ready", () => {
	console.log(client.user.username + " is online and ready for action!");
});

//Variables
//const COUNTING_CHANNEL_ID = 





//Commands
client.on("Selam", (Selam canım hoşgeldin.) => {
	//console.log(message);
	//Make sure the message is meant for the us:
	//Disregard if it was sent by a bot
	if(message.author.bot) return;
	//Disregard if it doesn't start with our prefix
	if(!message.content.startsWith(prefix)) return;

	//Takes takes off the prefix, leaving just the command itself
	var command = message.content.slice(prefix.length);
	
	if(command === "ping") {
    	return message.channel.send("pong");
	}
	
});

client.login(token); 1159207430354382919
