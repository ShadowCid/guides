# FF6WC Gated Tracker Setup
The following guide must be complete in its entirety for the tracker to work: 

### [Setup SNI](./sni.md)
<br>
<br>

# Step 0 - Connect your device to SNI
- Complete Steps 1-5 in the [SNI guide](./sni.md)
- Ensure SNI is running

# Step 1 - Open your game
- Start the game

# Step 2 - Open the tracker
Visit https://tracker.ff6worldscollide.com/
- If receiving a disconnect message, it is possible an error has occurred

<br>

# Step 3 Test Connection
## Successful Connection 
You will see the following if the tracker is successfully connected: 

![connected successfully](https://imgur.com/Ym9pCDm.png)

---------------

## Unsuccessful Connection - SNI and Tracker

 You will see the following if there is a connection issue between the tracker and SNI: 
 
 ![tracker error](https://imgur.com/op8MxPL.png)

If you are seeing this ensure step 0 is completed and the game is running.

If you have completed step 0 it could be you are running a newer version of SNI which the auto tracker has trouble connecting to. To resolve the issue you need to create an environment variable and then restart SNI. To create the environment variable
- Open start menu and search "environment" <br/> <img src="https://i.imgur.com/yRvWu6D.png" style="width:600px;" />
- Click on the Environment Variables button <br/> <img src="https://i.imgur.com/OQiJB6x.png" style="width:400px;" />
- Create a new user variable by clicking on the New button <br/> <img src="https://i.imgur.com/TjC3hhb.png" style="width:400px;" />
  - use the name `SNI_USB2SNES_LISTEN_ADDRS`
  - set the value to `0.0.0.0:23074,0.0.0.0:8080`
  - click `Ok` to create the variable.
- click `Ok` to save the change
- click `Ok` one more time
- close SNI and reopen it and restart at Step 1


## Unsuccessful Connection - SNI and Console/Emulator

 You will see the following if SNI is connected to the tracker, but there is a connection issue between SNI and your console or emulator: 
 
 ![tracker error2](https://i.imgur.com/diMAeU7.png)

If you are seeing this ensure step 0 is completed and the game is running.

# Help
If having issues connecting to SNI please do the following:

- Restart SNI
- Right click SNI > Click "Show Console"
- Restart the tracker and get to the "Disconnected" state
- Post the log to the [FF6WC discord](https://discord.gg/5MPeng5) `#trackers` channel
