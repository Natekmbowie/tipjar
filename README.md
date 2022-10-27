# These instructions are a work in progress. Check back soon.


# Tip Jar
[Github Repository & Download](https://github.com/Natekmbowie/tipjar)

[Template 1](https://natekmbowie.github.io/tipjar/files/tipjar1.html)

[Template 2](https://natekmbowie.github.io/tipjar/files/tipjar2.html)

[Template 3](https://natekmbowie.github.io/tipjar/files/tipjar3.html)


An Open Source template for creators to recieve donations. All simple self contained HTML, no complicated scripts, and no tracking of any kind.

I was in the mood for working on something like this instead of doing other things I needed to get done, so what the heck. This is obviously overly generic, so I can't garuntee it's the best for you, but I figured I would lay it out in they way I would assume would be the best for the most people. You can modify it as much as you want, but below I will lay out step by step instructions that should allow you to deploy something like this without needing to know coding (you'll have to edit a bit, but it will all be copy/paste or edited like a word doc).

The goal of this project, aside from allowing me to work on something, is to hopefully make it easy for any content creators to accept tips or donations with minimal effort and without having to pay for any hosting or do any coding. Let's decrease the need for ads, support creators, and allow them control of their own little corner of the internet :)

Oh, and all default links are just filled in with placeholder stuff - e.g. QR codes to the Wikipedia page on Rick Rolls. We'll all replace that in a moment.

## Reccomended Tools
Notepad ++ for Minor Text/Code Edits

Kompozer for Page Edits

the-qrcode-generator.com for QR Code Generation

Coinomi -or- Exodus Wallet for Crypto Donations

Wallet of Satoshi for Bitcoin Lightening Donations

## Step 0 Web Host Setup
The first step you getting a Tip Jar page set up is to figure out where you wish to host it. This will work on almost any host you can set up, some of which are free. If you already have a website that allows you to uplaod files then you can ignore this step.

A Few Options Include
* Paid Shared Hosts (e.g. Hostgator)
* Github Pages (free)
* NeoCities (free)
* IPFS (a protocol not a host, but Pinata will host for free)

That said, if you don't know much about any of those and want my advice I'd say go with GitHub Pages. You can [check out their about page](https://pages.github.com/), but it's not too complicated to get set up. Make a GitHub account, choose to create a "repository" and name it whatever you like, and select the public option. Once created, go to settings, pages, and enable the pages setting (use the "Main" branch unless you've changed it or created multiple).

Now, optionally, get your own domain and point it to Github. This will allow you to change hosts without needing to change the URL you share. Using registrars like NameSilo you can apply the Github template in one click so there's no configuration required.

## Step 1: Donations Options Setup
Next, you want to set up your donation sources if you havn't already. Things like how to set up Patrion/Utrion, Paypal, Librapay, or Buy me a Coffee are all outside of the scopes of this (but hopefully fairly straitforward). That said, if you don't have the ability to recieve crypto yet and want to add the crypto portions of the site then read on.

Start by downloading a crypto wallet such as CoinOmi or Exodus (I'd go with CoinOmi, but either is fine). Create your account, back up your seed phrase, and add all the coins you want to the wallet. From here you can choose that specific coin, choose the recieve option, and copy the address. People will send crypto to this address.

Next, you can downlaod your Bitcoin Lightening wallet of choice, such as Wallet of Satoshi. In that case, "back up" your wallet by creating an account via email, choose recieve, click the "Lightening Address" tab, and copy the long string of text at the bottom of the screen. People will send crypto to this address.

Note: If you want to stick a particular wallet and don't have a device compatible with them, you can always try running then in Bluestacks or something.

## Step 2: File Download
Once you have your donation options all set, go to [the main Tip Jar repository](https://github.com/Natekmbowie/tipjar), click code, and choose download as a zip. Extract the zipped folder and open the extracted contents. Open the /files folder and confirm you see tipjar1.html, tipjar2.html, and tipjar3.html and tipjar_files. Open the tipjar pages 1-3 and pick which one you like the most (though we can edit them further later). Delete the two you do not want and rename the one that you want to *tipjar.html*. Here is where we can start to make changes to the content. 

## Step 3: Image Replacements
The first content you will likely want to replace is some images. You will want an image to represent your merch and an image to represent your favorite way to donate with a credit card (assuming you will use those options). They can be whatever you want, but just make sure they are square. It's best they're not too huge in resolution (under 500x500 might be best to save space), but they will automatically be scaled down to the correct size when loaded in a web browser.

You will also want to generate three QR codes. Go to the QR code generating website and create one QR code of your Bitcoin Address, one of your Bitcoin Lightening Address, and one of your Monero address (assuming you are using them all) by pasting in the address then downloading the generated QR code.

Once you have all five images, name them the following names:

* "credit.png" for the image representing a donation with a credit card
* "merch.png" for the image representing merch purchases
* "btcdonate.png" for the donate with Bitcoin QR Code
* "btcldonate.png" for the donate with Bitcoin on the Lightening Network QR Code
* "xmrdonate.png" for the donate with Monero QR Code

Once you have the images renamed, copy them one by one into the tipjar_files folder. Each time you do it should say there is already a file there with that name and ask you if you want to replace it, make sure you select to replace it each time. Once you have done that for each you can open the tipjar.html file in a web browser and make sure that it is showing the new images (if it does not, try hitting refresh).

You can follow this step to replace any other image or file in the project.

## Step 4: Code Edits
Once you have the images fixed, now you need to make some minor edits to some code. This will probably be the most tricky looking, but it should be pretty strait forward. Open your text editor of choice (such as NotePad++) and make sure text wrap is off. You can do this in NotePad++ by clicking "View" and making sure that word wrap is not selected. Open the file tipjar.html in your text editor and make the changes listed below. For example, replacing *example.com* with your home page (say *yourpage.com* or *youtube.com/c/yourchanel*). In that case you would change that specific bit of text and NOT change any other text (for example, if there are quotation markes around example.com LEAVE THEM IN when you replace example.com with something else).

* in line 9 replace *https://example.com* with your home page. This could be the home page link to your website (multiple options, see 7-A or 7-B), or it could be a link to your main social media account. Just paste in the link you want people to go to when they click the "home" button.
* in line 12 replace *Donate to [name] to help support their work* with the text you want to show above the donation options. You can, however, also edit this in Step 6.
* in line 22 replace *https://example.com* with the link to your Merch store or other place to buy things from you (assuming you have one)
* in line 27 replace *https://example.com* with the link to your favorite donation service that supports credit cards (assuming you have one)

Now, save the changes and close the file. You can edit a lot more if you want to experiment, but these edits are all that must be done and are pretty much garunteed not to break things.

## Step 5: Edit Pop-Up Pages
With the main page mostly finished up, you can now edit the pop-up pages. Luckily these can be done without touching any code. Open your HTML editor (such as Kompozer. The four pages we will edit here are the btc.html, xmr.html, other.html, and othercrypto.html - all of which can be found in the tipjar_files folder. For each file open it in your editor and make the following changes:

* btc.html: replace [bitcoin address] with your Bitcoin Address, and [Lightening address] with your Bitcoin Lightening Address you got earlier. The QR code should already be correct since you updated the image in step 3.
* xmr.html: replace [xmr address] with your Monero address you got earlier. Again, the QR code should be correct.
* other.html: here is where you can add links to various other donation services and the like. In Kompozer, add links to what you would like by clicking the link icon, entering the text you wish the link to display, the URL that you want the user to go to, and open in new tab from the dropdown menu.
* othercrypto.html: this is where you can keep misc crypto addresses. Assuming you went with what I set as default, Bitcoin will have a main spot because it's most popular, Bitcoin lightening because it's great for tiny transactions (say a 10c transaction with no fees), and Monero because it's fairly popular (especially with the privacy community) and also private. Adding a bunch of other crypto addresses of your choosing will allow more options even if they're probably way less likely to be used. You can just set the names of each crypto you want to include and paste in the address for it, no need for QR codes since the goal is just to provide a bunch of misc options for anybody who wants them. Like other.html, you can edit it in Kompozer like a text/word document instead of dealing with code.

## (optional) Step 6: Main Page Edit
While you don't need to take this step, and this step is probably the most likely to break stuff, with all other edits done now is your chance to open the main page (tipjar.html) and make any additional changes you want from withing a graphical editor instead of doing it by code (unfortunately most code changes listed above have to be done through code only). Optional changes include:

* double clicking the *home* link and changing where it points (as apposed to doing it in step 4 manually)
* changing the about text that introduces you (or removing it entirely)
* deleting unused buttons and their corresponding images (just delete them with backspace like you would with an image in Word/Libre Office)
* changing the background and text colors (in the format menu of Kompozer) - I changed mine to match the color scheme of my website

## Step 7: Upload
Finally, the moment of truth! Upload the main page to your website host, and then create a new folder called tipjar_files and then upload all the files from the folder on your computer that you finished working on. Once you are done uploading make sure you double check every link, crypto address, and QR code is correct. Once that's done you can share the link. The exact link you share depends on how you choose to structure your new site.

### Step 7-A: Website Setup (Home Page + Tip Jar Page)
With option A, you can set up a basic home page, or are already hosting a site and just want to add the tips page to it. If you are already hosting an existing site you should know how to take it from here. If you do not have a site but want to make one, then create a homepage from scratch (if using Kompozer, just create a new page and fill it out from there). It can say anything you want it to, and link to anything you want it to. Once you are done, save your home page as index.html and upload that as well as your tipjar.html and tipjar_files content. 

If you have a custom domain your home page can be found by typing your domain (say your domain.com) and your tips page can be found at yourdomain.com/tipjar.html If you are using GitHub pages then your home page can be found at [username].github.com/[repositoryname] and your tips page can be found at [username].github.com/[repositoryname]/tipjar.html (replacing your domain.com, [username], or [repositoryname] with the values you chose). Same goes for NeoSites, or an IPFS gateway link, and so fourth.

### Step 7-B: Website Setup (Tip Jar Only)
A website is, in my opinion, a great thing to have for anybody who creates any sort of content - no matter how casual. Regardless, if you only want a tips page and no home page, then once the file is ready to be uploaded just rename tipjar.html to index.html (you can rename it before or after uploading). Nothing should break, and when you go to your main site (e.g yourdomain.com, [username].github.com/[repository], etc) you will be directed strait to the tips page. This will work perfectly fine, and you can always rename it back to tipjar.html and use index.html as a separate home page later, but you'll have to change any links you've shared or users will suddenly find themselves on your home page instead of your tips page if you add a different home page later to a site that previously used the tips page as the home page.

## Help & More
That summarizes the instructions. I hope that they were easy to accomplish and that the page works well for you if you end up using it. Sorry if the color scheme or default donation options are to generic or broad, but hopefully they're easy enough to change to what best fits what you're looking for. You can always find me @natebowie@mastodon.social on Mastodon (or @NathanBowie6 on Twitter, but I don't use it much). I might be offline or busy for stretches of time, but don't hesitate to ask questions if you want to.

## Credits
This template itself was made by me and is licensed under the MIT License. Use it for whatever you want to. The crude smiley face image is also made by me and licensed under the same license. The placeholder QR codes were generated by me with the-qrcode-generator.com, and are likely not copyrightable since they were auto generated (not legal advice though). The Bitcoin and Monero images were borrowed from their respective GitHub repositories, and the remaining two images (Purple Circle and Penny) are licensed under the Pixabay License (free to reuse, even for commercial use, with or without credit).
