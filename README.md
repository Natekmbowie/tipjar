# These instructions are a work in progress. Check back soon.


# Tip Jar
An Open Source template for creators to recieve donations. [see the Github Repository here](https://github.com/Natekmbowie/tipjar) or [check out an example here](https://natekmbowie.github.io/tipjar/files/tipjar.html).

I was in the mood for working on something like this instead of doing other things I needed to get done, so what the heck. This is obviously overly generic, so I can't garuntee it's the best for you, but I figured I would lay it out in they way I would assume would be the best for the most people. You can modify it as much as you want, but below I will lay out step by step instructions that should allow you to deploy something like this without needing to know coding (you'll have to edit a bit, but I'll try to make sure it's easy enough that you can do it quickly and easily).

The goal of this project, aside from allowing me to work on something, is to hopefully make it easy for any content creators to accept tips or donations with minimal effort and without having to pay for any hosting or do any coding. Let's decrease the need for ads, support creators, and allow them control of their own little corner of the internet :)

Oh, and all default links are just filled in with placeholder stuff - e.g. QR codes to the Wikipedia page on Rick Rolls. We'll all replace that in a moment.

## Reccomended Tools
Notepad ++ for Minor Text/Code Edits

Kompozer for Page Edits

the-qrcode-generator.com for QR Code Generation

Coinomi -or- Exodus Wallet for Crypto Donations

Wallet of Satoshi for Bitcoin Lightening Donations

## Step 0 Web Hosts Setup
The first step you getting a Tip Jar page set up is to figure out where you wish to host it. This will work on almost any host you can set up, some of which are free.

Your A Few Options Include
* Paid Shared Hosts (e.g. Hostgator)
* Github Pages (free)
* NeoCities (free)
* IPFS (a protocol not a host, but Pinata will host for free)

That said, if you don't know much about any of those and want my advice I'd say go with GitHub Pages. You can [check out their about page](https://pages.github.com/), but it's not too complicated to get set up. Make a GitHub account, choose to create a "repository" and name it whatever you like, and select the public option. Once created, got to settings, pages, and enable the pages setting (use the "Main" branch unless you've changed it or created multiple).

Now, optionally, get your own domain and point it to Github. This will allow you to change hosts without needing to change the URL you share. Using registrars like NameSilo you can apply the Github template in one click so there's no configuration required.

## Step 1: Donations Options Setup
Next, you want to set up your donation sources if you havn't already. Things like Patrion/Utrion, Paypal, Librapay, or Buy me a Coffee are all outside of the scopes of this. That said, if you don't have the ability to recieve crypto yet and want to add the crypto portions of the site then read on.

Start by downloading a crypto wallet such as CoinOmi or Exodus (I'd go with CoinOmi, but either is fine). Create your account, back up your seed phrase, and add all the coins you want to the wallet. From here you can choose that specific coin, choose the recieve option, and copy the address. People will send crypto to this address.

Next, you can downlaod your Bitcoin Lightening wallet of choice, such as Wallet of Satoshi. In that case, "back up" your wallet by creating an account via email, choose recieve, click the "Lightening Address" tab, and copy the long string of text at the bottom of the screen. People will send crypto to this address.

Note: If you want to stick a particular wallet and don't have a device compatible with them, you can always try running then in Bluestacks or something.

## Step 2: File Download
Once you have your donation options all set, go to [the main Tip Jar repository](https://github.com/Natekmbowie/tipjar), click code, and choose download as a zip. Extract the zipped folder and open the extracted contents. Open the /files folder so and confirm you see tipjar.html and tipjar_files. Here is where we can start to make changes to the content.

## Step 3: Image Replacements
The first content you will likely want to replace is some images. You will want an image to represent your merch and an image to represent your favorite way to donate with a credit card (assuming you will use those options). They can be whatever you want, but just make sure they are square. It's best they're not too huge in resolution (under 500x500 might be best to save space), but they will automatically be scalled down to the correct size when loaded in a web browser.

You will also want to generate three QR codes. Go to the QR code generating website and create one QR code of your Bitcoin Address, one of your Bitcoin Lightening Address, and one of your Monero address (assuming you are using them all) by pasting in the address then downloading the generated QR code.

## Step 4: Code Edits

## Step 5: "Other" Page and "Other Crypto" Page

## Step 6: Main Page Edit

## Step 7: Upload

### Step 7-A: Website Setup (Home Page + Tip Jar Page)

### Step 7-B: Website Setup (Tip Jar Only)

## Help & More
