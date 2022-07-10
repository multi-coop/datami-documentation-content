
## User options

<div>
  <img
    alt="TUTORIAL-ACTIONS-USER_OPTIONS"
    src="https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/tutorial/commented/tutorial-user_options.png"
    />
</div>

This block regroups many standard actions an user could expect from a service aiming to display and edit a file stored on a Git provider (Github or Gitlab).

The "user options" buttons are the following :

- **Reload** the file ;
- **Download** the file ;
- **Change your user token** ;
- **Check the user's commit branch(es)** ;
- **Copy the widget** ;
- **Change the language** ;

Let's see those more precisely.

### Reload the file

<div>
  <img
    alt="TUTORIAL-ACTIONS-RELOAD"
    src="https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/tutorial/commented/tutorial-04.png"
    />
</div>

As the file displayed in the widget is stored elsewhere (on a Github or Gitlab repository, or in a wiki), it could be useful to refresh the source data to check if any changes occured while you were editing it.

### Download the file

<div>
  <img
    alt="TUTORIAL-ACTIONS-DOWNLOAD"
    src="https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/tutorial/commented/tutorial-05.png"
    />
</div>

You can download the file on your computer or device just by clicking this button.

### Change your user token

<div>
  <img
    alt="TUTORIAL-ACTIONS-USER_TOKEN"
    src="https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/tutorial/commented/tutorial-06.png"
    />
</div>

By default Gitribute uses a "ghost user" token (like the account `multi-contributor` on Github), so you could contribute to a file without having to create an account.

The token is essential so you could "save" the changes you have made on the widget. This token is mandatory to make `POST` and `PUT` request to your Git provider's API.

But if you are familiar with Github or Gitlab (and if you already have an account on those) you can add change the token to put your own.

<div style="border: thin solid lightgrey;">
  <img
    alt="TUTORIAL-ACTIONS-USER_TOKEN-DIALOG"
    src="https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/tutorial/actions-token.png"
    />
</div>

### Check your commit branches

<div>
  <img
    alt="TUTORIAL-ACTIONS-BRANCHES"
    src="https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/tutorial/commented/tutorial-07.png"
    />
</div>

A "branch" selection dialog appears once you have saved your document. It means your contribution proposal has been sent to the owner for the source file, but is not "merged" yet onto the source file. 

<div style="border: thin solid lightgrey;">
  <img
    alt="TUTORIAL-ACTIONS-BRANCHES-DIALOG"
    src="https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/tutorial/contribution-branches.png"
    />
</div>

### Copy the widget

<div>
  <img
    alt="TUTORIAL-ACTIONS-COPY_WIDGET"
    src="https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/tutorial/commented/tutorial-08.png"
    />
</div>

More on this action in the next section...

### Change the language

<div>
  <img
    alt="TUTORIAL-ACTIONS-CHANGE_LOCALE"
    src="https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/tutorial/commented/tutorial-09.png"
    />
</div>

As you can imagine this button can change the language used in the widget.

<div>
  <img
    alt="TUTORIAL-ACTIONS-CHANGE_LOCALE-DIALOG"
    src="https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/tutorial/actions-language.png"
    />
</div>

> &nbsp;
> **_Note_** :
>  
> Changing the language can translate all texts from a Gitribute's widget itself, but can't change the data contained from the document itself.
>
> For instance if the mardown file displayed in the widget is written in swahili, its stays swahili. 
> &nbsp;

For now only french and english are available in Gitribute, but we would be glad if you propose to help us translate Gitribute to other languages (anyone speaking German, or Turkish, or Spanish, or Italian, or Arabic, or any other language... ?).

---
