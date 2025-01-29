---
title: 'Sendy Webhook: Move Sendy Subscriber from One List to Another List after the Autoresponder email sent'
date: Tue, 23 May 2023 05:13:32 +0000
draft: false
tags: ['How To', 'how to', 'sendy']
slug: "sendy-webhook-to-move-subscriber-to-another-list-after-autoresponder-email-sent"
---

If you have been using [sendy.co email marketing software](https://sendy.co/?ref=NMGZZ) to send emails, then you might be noticed sendy now offers "**Trigger webhook**" features in the "**Rules**" section.

With that features, users can now **move subscribers from one list to another list after an autoresponder email has been sent**.

To achieve that feature, you only need a webhook script to capture data and subscribe to another list using sendy.co subscribe API.

I have been waiting for that feature for quite a long time.

I tried searching on sendy.co forum to find any possible sendy script to do this task.

But no use.

I even asked the developer as well… still no use.

I won't blame the developer for this because it's out of scope support request for him.

Finally, I decided to hire a developer to do this work.

But you know the time involved in hiring and getting it done.

I also tried finding a relevant skilled developer as well… but I couldn't find one with that.

So I decided to do it myself… and here is the result.

Finally, I developed Sendy.co Webhook script to add Subscriber to another list after any specific autoresponder email has been sent with the help of sendy subscribe API.

With that script, you can move users to any number of lists.

Imagine a sequence.

After the user finishes one autoresponder sequence, that Subscriber will move to another autoresponder sequence. You can move like any number of List/Autoresponder in that particular brand.

**Sendy Autoresponder Webhook Script to Move Users to another List after Autoresponder Email has Sent:**
--------------------------------------------------------------------------------------------------------

1) First [Download Sendy Webhook Script here](https://checkout.pkarun.com/checkout/52b1c33c4259131d72106d98fddfb16c) | For Indian Users - [Only Script](https://pkarun.mojo.page/sendy-autoresponder-webhook) | [Only Support](https://pkarun.mojo.page/sendy-webhook-support-only)

2) Open the sendy-autoresponder-webhook.php file

3) You need to change the below details

![](/sendy-webhook-to-move-subscriber-to-another-list-after-autoresponder-email-sent/images/sendy-webhook-configuration.png)

```
//----- Required Settings ----------//
	
	
$your_installation_url = 'https://sendydomain.com'; //Your Sendy installation URL (without the trailing slash) (REQUIRED)	
	
$api_key = '1qMxxxxxxxxxxxxxxxNP'; //Your Sendy API Key (REQUIRED)
	
$enter_autoresponder_email_id = '234'; //Enter Autoresponder Email ID (REQUIRED)

$list = 'ezxxxxxxxxxxxxxxxxxxxxQw'; //To Which list you want to move Subscriber? Enter that List ID (REQUIRED)
```

**$api\_key**: This is sendy.co API Key. You can access your sendy API key by going to the **Top right** >> **Settings** \>> **Your API key**.

![](/sendy-webhook-to-move-subscriber-to-another-list-after-autoresponder-email-sent/images/sendy.co-API-Key.png)

**$enter\_autoresponder\_email\_id**: After which autoresponder email you need to move the user to another list? Open that autoresponder email and notedown that email ID number. In the below case 159 is the autoreponder email ID.

```
https://sendydomain.com/autoresponders-report.php?i=3&a=9&ae=**159**
```

In the browser bar, you will notice "**&ae=**" at the end of the URL. That number is your autoresponder email id.

![](/sendy-webhook-to-move-subscriber-to-another-list-after-autoresponder-email-sent/images/sendy-autoresponder-email-id.png)

sendy autoresponder email id: 159

**$list**: Enter your sendy list ID to which you need to move Subscriber after sending the autoresponder email. You can get list ID by going to **Brands** \>> **View all lists** >> **ID** (mouse hover to show full ID)

![](/sendy-webhook-to-move-subscriber-to-another-list-after-autoresponder-email-sent/images/sendy-list-id.png)

4) Now upload that sendy webhook script to your server and take the URL path.

5) Now go to **Rules** >> **Create a new rule** >> **On autoresponder email sent** >> **Select a Lists** >> **Choose Autoresponder** >> **Trigger webhook** >> **Paste the path of your webhook script** on your server >> click "**+Add**" button

![](/sendy-webhook-to-move-subscriber-to-another-list-after-autoresponder-email-sent/images/sendy-on-autoresponder-email-sent.png)

As soon as your autoresponder email is sent, the user will automatically move to another list with the help of a webhook script.

### Want to Unsubscribe Users After Subscribing to another List?

If you need to unsubscribe a user/subscriber from the original list after moving Subscriber to another list, you can do that with the help of Rules.

1) Go to **Rules** \>> **Create a new rule** >> **On subscribe** >> **select the list** >> **Unsubscribe from list** >> **Select a list to unsubscribe**

![](/sendy-webhook-to-move-subscriber-to-another-list-after-autoresponder-email-sent/images/sendy-on-subscribe.png)

That's it.

When the user subscribes to another list, sendy will unsubscribe the user from the previous list.

### FAQ's:

****1) Can you offer support?****

Support is not required if you follow the instructions correctly. If you still need support, I can do it for additional charges.

**2) I need some custom features. Can you do it for me?**

No. Sorry.

**3) Do you offer a refund?**

No. Refund will not be offered on this script.

**4) Do I need Zapier Integration to use this webhook?**

You don't need any external services like zapier to use this feature.

**5) I have a question. How can I ask you?**

You can send an email to arun (at) pkarun.com. I will respond within 24hrs.

[Buy Sendy Webhook to Move Subscribers to another List after Autoresponder email as sent here.](https://checkout.pkarun.com/checkout/52b1c33c4259131d72106d98fddfb16c)

**For Indian Users** - [Only Script](https://pkarun.mojo.page/sendy-autoresponder-webhook) | [Only Support](https://pkarun.mojo.page/sendy-webhook-support-only)