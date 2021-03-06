# [Platform Specific Features](../) > Google Assistant

Learn more about Google Assistant specific features that can be used with the Jovo Framework.

* [Introduction to Google Assistant Specific Features](#introduction-to-google-assistant-specific-features)
* [Output](#output)
  * [Multiple Reprompts](#multiple-reprompts)
  * [Screen Surfaces](#screen-surfaces)
* [Data](#data)


## Introduction to Google Assistant Specific Features

> Find an introduction to how Google Assistant works here: [Getting Started > Voice App Basics > Google Assistant](../../01_getting-started/voice-app-basics.md#google-assistant).

You can access the `googleAction` object like this:

```javascript
let google = this.googleAction();
```

## Output

This section provides an overview of Google Assistant specific features for output. For the basic concept, take a look here: [App Logic > Output](../../04_app-logic/03_output). 

### Multiple Reprompts

Google Assistant allows to add multiple reprompts that are spoken out in order if there is no response by the user. Here is the official reference by Google: [Static Reprompts](https://developers.google.com/actions/assistant/reprompts#static_reprompts).

The reprompts can be added to the [`ask`](../../04_app-logic/03_output#ask) method by using an array.

```javascript
this.ask(speech, [reprompt1, reprompt2, goodbyeMessage]);
```

The first two messages are usually reprompt messages, the third one is used to say goodbye to the user.

### Screen Surfaces

You can find out more about visual output here: [Platform specifics > Google Assistant > Visual](./visual.md)

## Data

You can find out more about your Google Action user's data here: [Platform specifics > Google Assistant > Data](./data.md)