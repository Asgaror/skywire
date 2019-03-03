![skywire logo](https://user-images.githubusercontent.com/26845312/32426764-3495e3d8-c282-11e7-8fe8-8e60e90cb906.png)

# Skywire Whitelisting System 


#### Table of Contents
* [Introduction](#introduction)
* [Account Creation](#account-creation)
* [First Login](#first-login)
* [View Miners](#view-miners)
* [Usage](#usage)
* [Submit Applications](#submit-applications)
    - [Application DECLINED](#application-declined)
    - [Application DISABLED](#application-disabled)
    - [Auto-Application Creation](#auto-application-creation)
* [Transfer Miner](#transfer-miner)
* [Troubleshooting](#troubleshooting)

<div align="center">
<b>
Usage of the Skywire Whitelisting System is required to be eligible for testnet rewards.
</b>
</div>

## Introduction

We are happy to announce the new Skywire account system which will be used to upgrade the whitelisting & data management procedures of the Skywire testnet.

Previous data records were imported into the new system but you are advised to double check the data in the system. 
Important note for people that had a DIY miner and an official miner in the old mikecrm system: you will only get to keep one reward address in this new system. 
Please verify the imported Skycoin wallet address and change it if necessary.

Everyone using the system must first create a user account. You can access the signup form by following [this link](https://auth.skycoin.net)

Please note that there are two different websites you'll have to use:
* [auth.skycoin.net](https://auth.skycoin.net) for account creation, confirmation & password change
* [whitelist.skycoin.net](https://whitelist.skycoin.net) for accessing the Skywire Whitelisting System, i.e. your data

Once you verified your account via email you can use the new system with all it's advantages:
- you can change your Skycoin wallet address at will
- you can change the public keys associated with a miner as it becomes necessary
- you can upgrade whitelisted miner and add more boards to them 
- you can review the pictures associated with your miners
last but not least
- you can submit new applications and review your application status & receive email notifications
- and more features to come

One last reminder for everyone to join the [Skywire PSA channel on telegram](https://t.me/SkywirePSA) if you're not already a member.
<div align="center">
<em>If you're unable to login please contact support@skycoin.net.<br>
    Bug reports have to be submitted on telegram at the moment. Further updates will be released soon
</em>
</div>

## Account Creation
<div align="center">
<p>
<em> Please enter your email address in lowercase letters. <br>
Note: gmail.com email users are advised to remove any dots from the local part of their email addresses, i.e. example@gmail.com instead of ex.am.ple@gmail.com otherwise they'll be unable to login.</b>
</em>
</div>

When you first access the system you have to create your user account. We imported any existing data submitted using the form on skycoin.net/whitelist in the database but the account creation must be done by yourself.

**Connect to [auth.skycoin.net](https://auth.skycoin.net):**

<div align="center">
<img src="https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/whitelisting_login.png"
     alt="Login page."
/>
</div>

**Click on 'Sign up' please.**


![signup_form](https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/signup_form.png)
**Enter your data in the form.**

![signup_form_filled](https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/signup_form_filled.png)
**Click on 'Submit'.**

<div align="center">
<img src="https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/signup_popup.png"
     alt="Sign up submitted popup."
/>
<p>
<b>This popup will inform you that you action was performed properly.</b>
</p>
</div>

![signup_email](https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/signup_email.png)
**Example email from email address used for creating this guide.**
**Click on 'Confirm your account'.**

<div align="center">
<img src="https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/signup_confirmed_popup.png"
     alt="Sign up confirmed popup."
/>
<p>
<b>This popup will inform you that you action was performed properly.</b>
</p>
</div>



***



### First Login
<div align="center">
<p>
<em> Please enter your email address in lowercase letters. <br>
Note: gmail.com email users are advised to remove any dots from the local part of their email addresses, i.e. example@gmail.com instead of ex.am.ple@gmail.com otherwise they'll be unable to login.</b>
</em>
</div>

**Connect to [whitelist.skycoin.net](https://whitelist.skycoin.net):**

![whitelisting_login](https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/whitelisting_login_enter_data.png)

**Enter your data used on 'Sign up'.**

![whitelisting_login_filled](https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system//whitelisting_login_filled.png)
**Fill in your account data.**

![whitelisting_first_login](https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/whitelisting_first_login.png)
**The first screen you'll be looking at - an empty whitelist application form.**
**Click on 'Account Info'.**

![whitelisting_account_info_no_address](https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/whitelisting_account_info_no_address.png)
**If you're looking at this screen and no data is being displayed, please refresh the website.**

![whitelisting_account_info](https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/whitelisting_account_info.png)
**This is how the page should look after you refreshed it if not from the start.**
**Your email address and registered Skycoin wallet address is listed here.**
**Update the Skycoin wallet address as you like.**

<div align="center">
<img src="https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/whitelisting_address_changed_popup.png"
     alt="Address change popup."
/>
<p>
<b>Changed Skycoin wallet addresses are confirmed with this popup.</b>
</p>
</div>



***



### View Miners
<div align="center">
    <p>
        <em>
        If your miner(s) were approved before the account system was released and you submitted them using the previous form then you will be able to find your miners in this list. 
        Make sure your data is correct and adjust it if necessary!
        </em>
    </p>
</div>

**Connect to [whitelist.skycoin.net](https://whitelist.skycoin.net) and login.**

**To view your accepted and whitelisted devices please click on 'Miners'.**

![whitelisting_miners](https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/whitelisting_miners.png)

* **Your whitelisted miners can be found here.**
* **Note the attributes that you miners has:** 
    * MinerID is your individual miner ID.
    * Miner type is the type of your miner, i.e. either official or DIY.
    * Created at is the date on which your miner was approved.
    * Batch is only relevant for official miners and displays the batch of your official miner.
    * Is Active represents the status of your miner. You can choose to only list active or disabled miners.

![whitelisting_miner_overview](https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/whitelisting_miner_overview.png)


#### This is the overview of the whitelisted DIY miner.
* View the pictures associated with the miner.
* View and update the associated public keys with the miner.
* If you want to add more boards to your miner, your miner will automatically resubmit itself as described in this section. Attention!

<div align="center"><b>Read up thouroughly in the Auto-Application Creation section before surpassing the amount of whitelisted boards.</b></div>

### Usage
* Update whitelisted miners using the miner overview page
    * Update associated public keys
    * Add more boards by performing the steps outlined in the [Auto Application Creation](https://github.com/skycoin/skywire/wiki/Skywire-Whitelisting-System#auto-application-creation)

<div align="center"><b>Do not submit new applications for updating the public keys of a whitelisted miner<br> If you want to add boards please perform the outlined steps referenced in the list above.</b></div>

***


## Submit Applications
The following pictures will guide you how to submit an application.
Read up on the required information in [this section of the Skywire testnet rules article](https://github.com/skycoin/skywire/blob/master/testnet_rules.md#the-form).

![whitelisting_application_text_filled](https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/whitelisting_application_text_filled.png)

* **Enter the text of your whitelist application.**
* **Explanations can be found in the text entries.**

![whitelisting_picture_selection](https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/picture_selection.png)

* **Select the pictures which meet the requirements described on the [Skywire testnet rules article](https://github.com/skycoin/skywire/blob/master/testnet_rules.md).**

![whitelisting_application_example](https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/whitelisting_application_example.png)

* **Include at least three pictures that meet the requirements.**
* **The complete example application used to create this guide.**

![whitelisting_actual_application](https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/whitelisting_actual_application.png)

* **This is the actual application data which is used in this guide.**

<div align="center">
<img src="https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/whitelisting_application_submitted_popup.png"
     alt="Application submitted popup."
/>
<p>
<b>This popup will inform you that you action was performed properly.</b>
</p>
</div>


![whitelisting_application_submitted](https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/whitelisting_application_submitted.png)

* **Once your application was correctly submitted you will be looking at this screen.**

![whitelisting_first_login](https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/whitelisting_first_login.png)

* **Once your application was accepted you will be looking at this screen once again.**
* **Continue with the next section please to view your accepted miner.**
* **In case you are not looking at this screen, please go to Application DECLINED.**

*** 

#### Application DECLINED
In case your application was declined it means you have missed some of the requirements listed in the [Skywire testnet rules article](https://github.com/skycoin/skywire/blob/master/testnet_rules.md).
Any interaction with your application triggers email notification that updates you on the current status, make sure to check your email regularely if you have a PENDING application.
The screen in the system will look like this:

![whitelisting_application_declined](https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/whitelisting_application_declined.png)

* **As long as your application is being `DECLINED` and not `DISABLED` you are free to resubmit the form to fix any flaws.**

![whitelisting_application_declined_fixed](https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/whitelisting_application_declined_fixed.png)

***

#### Application DISABLED
In case your application was `DISABLED` you won't see an empty whitelist application form in the system. You have to check your emails to see the information about your `DISABLED` application. 
Once an application was `DISABLED` it's the best practise to contact support@skycoin.net if you want to further discuss your issue and attempt to resolve it.

User accounts that had one of their applications `DISABLED` is still free to open further applications. Only serious rule violations and misdeeds will lead to having your account disabled/miner deleted.

***

### Auto-Application Creation
<div align="center">
<p>
    <b>
    Any open application will be put in the background and on hold until the automated application was approved by an admin. Once that's done your previously open application
    will be restored into it's previous state.
    </b>
</p>
</div>

If you surpass the amount of whitelisted public keys associated with your miner by adjusting its public keys on the 'Miner overview' page, then it will automatically fill in the info for a new application with the additional public key(s) and submit it for you. 

<div align="center">
<p>
    <b>
    The automated application will submit the public key automatically. However, you do have to select new pictures that display the adjustments on your miner and update the application manually once more.
    </b>
</p>
</div>

The previous version of the miner remains active and ready to receive rewards without the additional public keys. Simply exchanging your currently submitted public keys does not trigger this action to be performed.

The amount of whitelisted public keys associated with the miner is being surpassed:
![whitelisting_miner_amount_surpassed](https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/whitelisting_miner_amount_surpassed.png)

* **Add an additional board to your miner by adding another public key.**
* **Click on 'Submit' once you're done.**

![whitelisting_miner_amount_surpassed_active_part](https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/whitelisting_miner_overview.png)

* **This is the version of the miner that remains active & ready to receive rewards. There's no information being displayed about the submission to add another public key to this miner.**
* **The additional public key(s) are added to a `PENDING` application which is displayed below.**

![whitelisting_miner_amount_surpassed_popup](https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/whitelisting_miner_overview_transfer_popup.png)

* Warning about the action you are about to perform. **Read this thouroughly.**

![whitelisting_miner_amount_surpassed_automated_resubmission](https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/whitelisting_miner_amount_surpassed_automated_application.png)

* **Automated application which has been submitted that includes the additional public key(s).**
<div align="cener">
<b>THIS IS WHERE YOU HAVE TO SELECT YOUR NEW PICTURES TO UPDATE THE APPLICATION!</b>
</div>

![whitelisting_miner_amount_surpassed_automated_resubmission_approved](https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/whitelisting_automated_application_approved.png)

* **Once an admin approved your automated application you can see your public keys included on the 'Miner overview' page.**

***

## Transfer Miner
If you login to your account and choose a miner in your miners list you'll see the option to *TRANSFER* the miner. 

![whitelisting_miner_overview_transfer](https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/whitelisting_miner_overview_transfer.png)

**Transfering a miner to another email address removes any entitlement for future rewards effectively immediately and cannot be reverted if you're not in control of the account to which the miner was transferred to.**

![whitelisting_miner_overview_transfer_popup](https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/whitelisting_miner_overview_transfer_popup.png) 

* **You will see a popup which provides information about the consequences of this action.**

***

## Troubleshooting
This section will include any common issues or hurdles people encountered.

### Can't reset user's password user action token expired
Please request a new password reset token by clicking on 'Forgot your password?' on the login page of the [auth.skycoin.net](https://auth.skycoin.net).

Input your email address without any periods in the local part (localpart@globalpart).

Check your inbox and assign a new password by following the link in the email you'll receive.

Login to the [Skywire Whitelisting System](https://whitelist.skycoin.net) and proceed with the steps starting [here](https://github.com/skycoin/skywire/wiki/Skywire-Whitelisting-System#first-login).

### "I cannot see any data in the system"
If you're logged into the system but cannot see your data except the option to change your password you're logged into _the wrong system_.

<div align="center">
<img src="https://raw.githubusercontent.com/Asgaror/skywire/binary_data_storage/pictures/whitelisting_system/menu_bar.png"
     alt="The correct menu bar of the Skywire Whitelisting System at whitelist.skycoin.net"/><br>
<em>The correct menu bar of the Skywire Whitelisting System at <a href="https://whitelist.skycoin.net">whitelist.skycoin.net</a></em>
</div> 
<br>
Please switch from <a href="https://auth.skycoin.net">auth.skycoin.net</a> to <a href="https://whitelist.skycoin.net">whitelist.skycoin.net</a> to login to the Skywire Whitelisting System. 
