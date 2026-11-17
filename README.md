# Discord JS Button Command System - For SAMP

A Discord bot project built with **Node.js** and **Discord.js v13**, featuring a modular structure for commands, buttons, slash commands, and modal interactions.

The project also integrates a MySQL database connection for data management.

## Features

- **Command Handler** — Organized command handling system.
- **Slash Commands** — Support for Discord slash command interactions.
- **Button Interactions** — Modular button interaction handlers.
- **Modal Interactions** — Support for Discord modal submissions.
- **Event Handler** — Separate event handling structure.
- **MySQL Integration** — Database connection using a MySQL connection pool.
- **Embed Utilities** — Reusable response helpers for success, error, usage, and permission messages.
- **Error Logging** — Webhook-based error reporting.

## Tech Stack

- **Runtime:** Node.js
- **Language:** JavaScript
- **Discord Library:** Discord.js v13
- **Database:** MySQL
- **Environment Variables:** dotenv

## Project Structure

```text
discord-js-button-command-bot-system/
├── Buttons/
│   └── Button Register/
├── Commands/
│   └── info/
├── Events/
├── Handler/
├── Modals/
├── SlashCommands/
├── Functions.js
├── Merpati.js
├── Mysql.js
├── config.json
├── package.json
└── package-lock.json
```

## Requirements

Before running the project, make sure you have:

- Node.js and npm installed.
- A Discord application and bot token.
- A MySQL database server.
- The required Discord bot permissions and intents.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Anjaya-PureFrame/discord-js-button-command-bot-system.git
   ```

2. Navigate to the project directory:

   ```bash
   cd discord-js-button-command-bot-system
   ```

3. Install dependencies:

   ```bash
   npm install
   ```

4. Install Nodemon if it is not already available:

   ```bash
   npm install --save-dev nodemon
   ```

## Configuration

### 1. Environment Variables

Create a `.env` file in the project root:

```env
TOKEN_BOT=your_discord_bot_token
```

Never commit your actual bot token or webhook credentials to GitHub.

### 2. MySQL Configuration

Update the `config.json` file with your MySQL connection details:

```json
{
  "mysql": {
    "connectionLimit": 5,
    "host": "localhost",
    "user": "your_mysql_user",
    "password": "your_mysql_password",
    "database": "your_database_name"
  }
}
```

Make sure the database exists before starting the bot.

## Running the Bot

Start the bot using:

```bash
npm start
```

The project uses Nodemon in its start script to run `Merpati.js`.

## Dependencies

Some of the main dependencies used in this project:

- `discord.js`
- `discord-modals`
- `discord-html-transcripts`
- `dotenv`
- `mysql`
- `mongoose`
- `samp-query`

See `package.json` for the complete dependency list.

## License

The package metadata currently specifies the ISC license. Refer to the repository's license file or confirm the intended licensing terms before redistributing this project.

---

**Discord JS Button Command System**  
Built with JavaScript and Discord.js.
