# FAQ - Running Residence on Spigot / Paper 1.18.1

Zrips Discord @ https://discord.gg/dDMamN4

This page should help explain what I personally think is the way to run Residence version 5.x on Spigot-, and Paper 1.17.1 and below.

```
------------------------------------------
Residence version 5.0.1.3
CMILib version 1.1.1.0
Server: Paper(187) 1.18.1-R0.1-SNAPSHOT
Economy: CMIEconomy Vault: 1.7.3-b
------------------------------------------
```

## <g-emoji class="g-emoji" alias="information_source" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/2139.png">ℹ️</g-emoji> Note ahead.

- This is about Residence 5.x and Spigot or Paper server version 1.18.1 mainly, apply to 1.17.1 and other lower versions accordingly.

- CMI version 9.1.x is recommended as an Economy engine, but other older economy engines like EssentialsX-economy as well. 
- More info about Residence + Economy: URL-TODO

- CMI Lib version 1.1.1.0 or newer is required.
- Zrips' libraries and other resources are linked below.

### <g-emoji class="g-emoji" alias="information_source" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/2139.png">ℹ️</g-emoji> Backup

- First, I strongly recommend before making any changes to your live server to take it offline with /stop and make a complete backup of the full directory, do not forget to backup your MySQL databases if you use any. 

### <g-emoji class="g-emoji" alias="information_source" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/2139.png">ℹ️</g-emoji> Test setup

- Before you actually update your live server it's recommended to have a test instance you can try stuff out on. This way you can detect issues and concerns early and learn to address those. Without risking your live server!
- If this testing takes hours and days and you have new live data because players keep playing, obviously take the live server offline and backup again, before making the final changes.

### <g-emoji class="g-emoji" alias="information_source" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/2139.png">ℹ️</g-emoji> Before we start to install and/or upgrade Residence 5

- `/stop` your server. Do the backup thing, and make a test server.

- Go to SpigotMC and download Residence if you haven't yet. And use BuildTools.jar from SpigotMC to build the latest version of Spigot 1.18.1 or download Paper 1.18.1 from their site.

- If you are not yet running CMILib then it will automatically download it. If this isn't the case due to firewalls or whatever reason, you can also manually download it here: <https://www.spigotmc.org/resources/87610/>

- Now that we have the latest files and are installing or upgrading from an older version to a new version, and we have a backup. It's time to replace any existing jars.

### <g-emoji class="g-emoji" alias="information_source" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/2139.png">ℹ️</g-emoji> First time Installalation

If you already are running Residence, you can skip this and go straight to Upgrading (see below).

- Put the downloaded Residence `.jar` in the plugins/ directory. 

- Start the server and let it complete loading.

- Keep an eye on the console, the `latest.log` will also have all the details. If something goes wrong, take note. And try to figure out what is up and try again. 

- If you spot any bugs, confirm them, and report them to Zrip's Github as a new issue.

- When the server has started, Residence will automatically download languages, CMI Lib and you're ready to **Finish** (see below)

### <g-emoji class="g-emoji" alias="information_source" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/2139.png">ℹ️</g-emoji> Upgrading Residence

If you are installing it for the first time, go to the Installing steps above and skip the upgrading steps.

- Keep the existing `~/plugins/Residence/` folder, do not delete it.

- Keep the existing `~/plugins/CMILib/` folder, do not delete it.

- If you don't have the CMILib folder, don't worry, it will create it for you.

- If you have the old CMILib version, don't worry, Residence will auto-upgrade it, and we will clean up after.

- Remove the old Residence `.jar` you're using from the plugins/ directory. 

- Put the freshly downloaded Residence `.jar` in the plugins/ directory. 

- Start the server and let it complete loading.

- Keep an eye on the console, the `latest.log` will also have all the details. If something goes wrong, take note. And try to figure out what is up and try again.

- When the server has started, you're ready to **Finish** (see below)

- If your plugins/ directory has the old CMILib `.jar` files, it is okay to remove them now. Keep the new .jar of course.

### <g-emoji class="g-emoji" alias="information_source" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/2139.png">ℹ️</g-emoji> Finishing up.

Okay, you've backed everything up, you've made a test setup, and you've either fresh installed or upgraded Residence. Just one more thing before you can play with this test setup that is now running.

- I always recommend one extra /stop and start .. so you can keep an eye on the console (or `latest.log`) again and make sure there's no weird errors.

And that's it! You're done.

What a list huh, okay, now you have experience, you have tested, and you can do it again: but on the live server! Have fun with Residence.

#### <g-emoji class="g-emoji" alias="information_source" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/2139.png">ℹ️</g-emoji> What about 1.16.5?

Personally I feel this is now outdated, and replaced by 1.18.1 or newer, please upgrade first, but yes, Residence works on 1.17.1 as well. And other lower versions.

#### <g-emoji class="g-emoji" alias="information_source" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/2139.png">ℹ️</g-emoji> Resources

SpigotMC's Buildtools.jar can be found here <https://hub.spigotmc.org/jenkins/job/BuildTools/>

`Residence v2` Residence resource page
<https://www.spigotmc.org/resources/11480/>

`CMI Vault` Economy-compile for best results
<http://www.zrips.net/wp-content/uploads/2020/07/Vault-1.7.3.jar>

`CMI Injector` Use your own Vault? Use this economy injector
<http://www.zrips.net/wp-content/uploads/2020/07/CMIEInjector1.0.2.3.jar>

`CMI Library` Base Library (Required by CMI and Residence)
<https://www.spigotmc.org/resources/cmilib.87610/>
More info about CMILib <https://github.com/mrfdev/CMI/blob/master/Resources/FAQ/cmi-library.md>

`Spigot website` This is where you can get buildtools and make a spigot 1.18.1 jar
<https://hub.spigotmc.org/jenkins/job/BuildTools/>

`Paper website` This is where you can get Paper's 1.18.1 jar
<https://papermc.io/downloads>

More information about Residence: https://www.zrips.net/Residence/, here you can find info about permissions, chat titles, signs and other Residence features. 
