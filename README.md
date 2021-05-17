# [Table of Contents](#table-of-contents)
- [Table of Contents](#table-of-contents)
- [Quick Start](#quick-start)
- [General Streaming Setup](#general-streaming-setup)
  - [2FA Set-Up (Not Required)](#2fa-set-up-not-required)
  - [Stream Settings](#stream-settings)
- [Uploading to YouTube](#uploading-to-youtube)
- [Using Streaming Templates](#using-streaming-templates)
  - [Streamelements OBS.live](#streamelements-obslive)
  - [Streamlabs](#streamlabs)
- [Editing Assets](#editing-assets)
- [Tournament Creation](#tournament-creation)
# Quick Start
This README is to provide a quick guide to start streaming content for the Williams College PC Gaming Channel. If you just need access to files, feel free to look around the repository. If you have any questions, please take a look through this guide before sending me any messages.
# General Streaming Setup
Twitch streaming on the official Williams College PC Gaming account requires either direct access to the account or a streamkey attached to the account. Ask a user with access to the official account to give you broadcasting rights. They will need your twitch account as well as the email associated with the account in order to send you a stream key and moderation rights. The account credentials are found in the google drive. 

## 2FA Set-Up (Not Required)
A requirement of having Twitch Affiliate status is that 2-FA is enabled. Twitch 2-FA is administered via Authy which does have multiple device support so if you need access to the actual Twitch account (i.e. if you are a club president, running the broadcast for an event, or something of similar import), request to be added from a person who has their Authy account enabled with Twitch. Add your name to the list below once you have been given access and verified that your 2FA codes are functional.
<details>
    <summary>List of people with 2-FA access</summary>
    - Benjamin Bui
</details>

## Stream Settings
Streams should be aiming for a video bitrate of 6000 Kbps. The base canvas resolution should be set to 1920x1080 even if the monitor you are recording from is of higher resolution. This is prevent improper scaling of overlays and other on-stream assets. Output resolution should also be set to 1920x1080. To stream to the channel, either log in to twitch using your streaming application or copy-paste the stream-key given into your broadcast software settings. 
# Uploading to YouTube
The url of the Williams College PC Gaming YT channel is https://www.youtube.com/channel/UCS2EqCcyiMEaBnEtbOJvvJg. 

The account credentials are found in the google drive.

2-Factor Authentication is not currently enabled.

To Upload
1. Login to the Williams College PC Gaming YouTube Account.
2. Go to the YouTube Studio webpage and select "Create".
3. After choosing your file (Preferably mp4 with H.264 encoding and AAC audio), set your title, description, playlist if part of a series, and upload a thumbnail if available.
4. Video upload should default to "No, it's not made for kids" but if not, select this option.
5. Select the desired publishing option
    <details>
    <summary>Click here for a description of publishing options</summary>

   -Private videos can only be seen by those with access to the account and YouTube accounts explicitly allowed to access the video

   -Unlisted videos are only accessible by those with the link to the video. This option is useful when testing the quality of your upload and to detect copyright claims before the video is made public

   -Public videos are available immediately after the upload and processing is complete. 

   -Premieres upload and process the video but do not show the video until a date and time of your choosing. At that time,the video will play simultaneously for all viewers with chat enabled until the duration of the video has passed wherein it will behave like an ordinary public video

# Using Streaming Templates 
All of the below methods allow for customizing of templates after importing but aside from resizing individual assets, rewriting text, and other such minor changes, Adobe After Effects is needed to edit assets.
 ## Streamelements OBS.live
 Streamelements specific templates are located in `./templates/obslive/`. Streamelements users have a choice between using the web-based overlay editor doing so in the desktop client. As a general guideline, the web-based editor allows for easier collaboration and reduced client-side load. Using the template on the desktop client increases system load but eliminates framerate issues caused by lag to the Streamelements servers. I generally prefer to run my streams entirely client-side aside from twitch chat integrations. Templates included are for running client-side. Note, setting conditional transitions requires the [OBS Transition Matrix](https://obsproject.com/forum/resources/obs-transition-matrix.751/)

 To install templates using Streamelements or OBS
 1. Go into scene collections and select import. 
 2. Select the `.json` file in `./obs/` containing the desired templates 
 3. Note that some paths may not transfer properly and will need to be manually added or adjusted. 
 ## Streamlabs 
 Streamlabs specific templates are located in `./templates/slobs/`
To install templates using Streamlabs
1. Go into settings and click "Scene Collections"
2. Click on "Import Overlay File" and select the desired file
# Editing Assets
Editing individual assets beyond changing of fonts and resizing requires Adobe After Effects for video elements and Photoshop/Illustrator for still elements A brief guide for editing or creating your own effects can be found [here](./aep/editing_guide.md). Any new or edited logos should be added to `/psd-ai`.
# Tournament Creation
Moving forward, tournaments should be organized using Battlefy. Log into Battlefy through Google using the same credentials listed in section detailing how to upload YouTube videos. This account enables you to see both the set-up and results of all past tournaments in addition to create new tournaments.

IMPORTANT NOTE: If you are competing in ANY tournaments through Battlefy, make sure to log out of the Williams College account. I do not want to see Williams College PC Gaming Club end up as last place in a random Legends of Runeterra Tournament because someone wanted to play flex at the same time.

  <details>
  <summary>Instructions on creating a tournament</summary>
  <ol>
  <li> Click on Organize Tournaments in the sidebar and select Williams PC Gaming as the organization (This could be expanded in the future if there is sufficient demand for tournaments of different games)</li>
  <li>2. At the bottom, select New Tournament and choose the game the tournament will be played in</li>
  <li>3. Type in the name and approximate date and time the tournament should start.</li>
  <li>4. If you have a tournament code or are recreating a tournament structure made recently, you can clone your tournament. If not, proceed to set-up your tournament.</li>
  <li>5. Put in a way for participants to contact a tournament organizer, some important rules for proper conduct, and a schedule.</li>
  <li>6. Invitations can be done by giving players a one-time use link if the participants are already known or allowing any players with access to the link to sign up.
    <ul>
      <li>For team-based games like League of Legends, it is easier to just have the captains of teams sign up for the tournament as this prevents issues with creating teams if one player forgets to sign up on Battlefy</li>
    </ul>
  </li>
  <li> Create the necessary brackets for the tournament. Battlefy supports single/double elimination, single round robin, and single swiss formats
  <li> Battlefy has automatic random seeding built-in but you can also seed different parts of the tournament by bracket standings</li>
  <li> When completed, publish the tournament and send invitations to players as needed </li>
  </ol>
  </details>