## DISCLAIMER: Credits for the API call C# code go to Sanshoo

#### References in the two API call C# Execute Code sub-actions

- System.dll
- System.Net.Http.dll

### If you have the [Source Copy plugin](<https://obsproject.com/forum/resources/source-copy.1261/>), you can use the Load Scene function to load the provided [NS] Goal Bars.json file into OBS. Otherwise, you can follow the following directions.

#### 1\. Create a nested scene

- [NS] Goal

#### 2\. Create these text sources within the nested scene

- `[TS] Follower Number` \- This text will be updated by Streamer Bot when you trigger the Follower Goal action
- `[TS] Follower Goal` \- This text can be changed by assigning the !setfollowergoal command and running `!setfollowergoal number`
- `[TS] Follow Goal Title` \- You can set the text to whatever you want, such as "Follower Goal"
- `[TS] Subs Number` \- This text will be updated by Streamer Bot when you trigger the Subs Goal action
- `[TS] Subs Goal` \- This text can be changed by assigning the !setsubgoal command and running `!setsubgoal number`
- `[TS] Subs Goal Title` \- You can set the text to whatever you want, such as "Subscriber Goal"

#### 3\. Create these color sources at 1000w x 100h px

- `[CS] Follow Progress Bar` \- Set the color in the `Follower Goal` action in Streamer Bot
- `[CS] Follow Bar` \- Set the color in OBS
- `[CS] Subs Progress Bar` \- Set the color in the `Subs Goal` action in Streamer Bot
- `[CS] Sub Bar`\- Set the color in OBS

#### 4\. Format the groups in OBS however you like and then you can nest this scene in your main scene.

# Import Code

`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`
