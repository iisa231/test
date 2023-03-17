Deploy LINE Bot Python Examples on Render

This repo can be used to deploy python examples in the line-bot-sdk-python on Render.
Prerequisites

Make sure you have the following:

    A dedicated Messaging API channel for your bot.
    A Render account that doesn't require credit card to sign up.

Deployment

    Fork this repo.

    Update render.yaml to comment/uncomment the services of LINE bot examples you want to deploy.

    Cieck to deploy

    Deploy to Render

    You will be prompted to input LINE channel secret and access token. You can find them on the LINE Developers Console. Channel secret is on the channel's Basic settings tab. Channel access token is on the channel's Messaging API tab.

    Once the bot servcie is live, find the service onrender URL (e.g., https://line-bot-python-<something unique>.onrender.com) on the Dashboard. Append /callback to the service URL to build the webhook URL (e.g., https://line-bot-python-<something unique>.onrender.com/callback). Paste the webhook URL to the Webhook settings section on the LINE channel's Messaging API tab on the LINE Developers Console. Also enable Use webhook on the same section.

    Add the LINE Official Account associated with your bot as a friend on LINE by scanning the QR code on the Messaging API tab of your channel settings on the LINE Developers Console.

    That's it. Send your LINE Official Account a text message on LINE and confirm that it responds with the same message.

Notes

    If your LINE bot app files are in the same repo as render.yaml, you don't need to specify repo in the render.yaml. You can find more information in the Render Blueprint spec.
