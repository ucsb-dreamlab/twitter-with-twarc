---
title: Setup
---
> ## Data
>
> The data we will be using in the workshop is to practice working with twitter 
> data. Please download the data files `hashtag_gasprices.jsonl` and `dehydratedCapitolRiotTweets.txt` and keep it in an accessible place (such as your desktop). We used 
> twarc to search for all mentions of the hashtag `#gasprices` and created this 
> . The Capitol Riot tweets is a dataset from Kaggle.
> - [tweets containing #gasprices data download link](https://drive.google.com/file/d/1hzBuHOuI-ZIfvrT1-rfUj34XaqFfJX9d/view?usp=sharing)
> - [Capitol Riot Tweets download link](https://drive.google.com/file/d/1S0yYZpBgLGEiKDAUeKepuU5IaZiW2gFA/view?usp=sharing)
> - [One Tweet download link](https://drive.google.com/file/d/1MNZRzCQPBKjvWCch7GvTywBFKvDstBcN/view?usp=sharing)
>
> Google Drive may change the file extensions when you download these.
> Make sure you that hashtag_gasprices and one_tweet are `.jsonl`, NOT `.jsn`.
> capitol_riots.txt really is `.txt`.
> <br/>
> You can force this by right 
> clicking on the page link, choose `save as`, then choose "all file types" 
> and remove the ".txt" ending and keep the ".jsonl" choose the appropriate
> filename extension.
>
{: .prereq}


> ## Additional Utilities
> 
> We will also be using an extended set of utilities that will help explore the data 
> collected through twarc. <br/> [twarc utilities download 
> link](https://github.com/UCSBCarpentry/twitter-with-twarc/blob/gh-pages/files/utils.zip?raw=true)
>
> Make sure you download and unzip this folder onto your desktop. Later in the workshop, we will upload this set of tools to our JupyterHub. 
>
{: .prereq}



### Getting the Necessary Privileges

Generally, we would call this 'getting your API key', but like many API's, the process of getting access to Twitter's has
become a complicated process. These instructions should create a new developer account with *Essential Access* privileges.

To get started, you will need:
* #### [A Twitter Account](https://twitter.com/){:target="_blank" rel="noopener"}:
Valid email account and cell phone number to receive texts are necessary.
* #### [Developer Account](https://developer.twitter.com/en){:target="_blank" rel="noopener"}:
You must create the Twitter account first, in order to link to the Developer account.

Getting developer access requires you to validate yourself as a human, so the
form is particular about having a valid phone number and email address added to your Twitter account. This is so Twitter can authenticate a user.

Once you are logged on to Twitter, sign into  
the [Developer Portal](https://developer.twitter.com/en){:target="_blank" rel="noopener"}

Fill out the application questions as listed here:

> ## Essential Access 
>
> Make sure this page is titled 'Just a few questions to get you Essential Access'.
> <br/>
> We are not applying for elevated or academic researcher access. 
>
{: .keypoints}

<img src="fig/setting-up-dev.PNG" width="500">

  
  - What country are you based in?
  - What's your use case? Choose `Teacher`
  - Will you make Twitter content or derived information available to a government entity or a government affiliated entity? `No` (recommended)
  - Click through the user agreement and verify your email.

### Making your Project and App

Right after verifying your email, you will be taken to your Developer Portal Dashboard and 
prompted to create a new *Project*. Every instance of Twarc is a *Twitter App* and 
Twitter Apps live inside of *Projects*. After selecting 'Exploring the API' as your use 
case, you will be given "Essential Access". Essential Access allows you to have one 
project with one App inside of it.

<img src="fig/dashboard.PNG" width="500">


Fill out the four questions to create your first Twitter App. It will ask you for the project name, use case, and description. The project name is your App. App names must be unique across the entire platform, so
if you get an error, choose a more unique name.
These can be edited and amended later if you choose to change something in the App. 

<img src="fig/what-you-api.PNG" width="600">

<img src="fig/project-description.PNG" width="500">

### Acquiring Keys and Tokens

After you have completed setting up your project, you will see the App details below. You can edit the name and app icon if you'd like to personalize it.

<img src="fig/twarc-app.png" width="500">

Under the project name, you will see *Settings* and *Keys and Tokens* tab. You will need to navigate to *Keys and Tokens* to generate your 5 keys and tokens. 
You will need to click the _generate_ button to get each of your keys and tokens. They are not automatically made for you so you must generate them the first time.

If you forget to save, or lose your tokens, you can click _regenerate_ to regenerate your keys and tokens, and a new set is made for you. 
However, if you do regenerate any keys and tokens, you'll need to reenter them when you try to access the API again.  

<img src="fig/dev-keys-tokens.png" width="500">


> ## Necessary Keys and Tokens
>
> ***SAVE*** these keys in an accessible place like a password manager or in a document. You will not see these 
> keys again, so this is essential. You should have: 
>
> * API Key 
> * API Secret 
> * Authentication Bearer Token 
> * Access Token
> * Access Token Secret
>
> You will have succeeded when you have these 5 keys and tokens
>
> ***If you are having problems generating the 5 tokens please [email us](mailto:collaboratory@library.ucsb.edu) immediately or else you will not be able to follow along
> with the lessons***
> 
{: .prereq}



<!--

### User Authentication Settings

After generating your tokens and keys, you need to authenticate to use the API. This can be found under Projects & Apps > Project > App.
Navigate to the User Authentication set up in the Settings Page and complete the following:
- Turn on OAuth 2.0
- Type of App: Single Page App
- Callback URL/Redirect URL: https://127.0.01/
- Website URL: https://ucsbcarpentry.github.io/

Save OAuth 2.0 Client ID and Client Secret

<img src="fig/Oauth-2.jpg" width="500">

-->

{% include links.md %}
