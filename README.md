# Find My Phone Raycast

I lose my phone often, so I made this.

This is a Node.js script that uses Playwright to automate iCloud Find My and trigger a sound on your Apple device. It's perfect for people like me who misplace their phones and want a quick, automated way to make them ring—right from the command line or Raycast.

## Usage

```sh
git clone https://github.com/vsvaidya27/fmp-raycast
cd fmp-raycast
npm install
cp .env.example .env
# Edit .env with your real credentials
chmod +x fmp.js
```

## How it works

- Automates login to iCloud Find My using Playwright
- Selects your device by name
- Triggers the "Play Sound" feature to help you locate your device

**Note:** You'll need to provide your iCloud credentials and device name in the `.env` file. Sometimes a 2FA check may pop up, but usually they allow you to bypass this and manual intervention is not neccesary (since you often need the very thing you are trying to find for 2FA).