# Introduction #

This project is to create an open source standards based [Voice over IP](VoIP.md) server in Erlang. Some design considerations are:

  * Completley based in Erlang
  * All open source code written for this project
  * Standards compliants using SIP and RTP as the primary protocols

Goals or milestones:

  * Connecting to a SIP provider for conenction to the PSTN
  * Ansering a call and playing a message; only action is to play a recorded message and then hand up
  * Interaction with the telephone keypad to perform other actions
  * Connection to a phone client, allowing phone calls from the server to and from the PSTN
  * Voicemail system that will reocrd messages and inform the client about message that are waiting

## Features ##

A person call from the PSTN and connects to [ErlVoIP](ErlVoIP.md). The call is routed based on the CallerId to perform certain actions at different times of the day or different status of the clients phone.

Some of thos actions could be:

  * Unknown phone numbers will go directly to vociemail from 5PM at night till 8am in the morning
  * Favored phone numbers will ring though 24/7
  * If the phone has a DND feature no calls will get through except favored phone nubmers

An auto-attendant will be provided so that [ErlVoIP](ErlVoIP.md) can be extended in the way the funcationality works.

Some other general feeatures that will be added eventually are:

  * Ring Groups
  * Call forwarding
  * Voice mail forwarding
  * Confernce calling

Many more features will be added as the project matures, but this covers the main features that the original design team feels are high priorites to create. These features will be configurable and created in a modular fashion so that they can be extended to overridden without needing to recompile [ErlVoIP](ErlVoIP.md).

## Erlang Internet Framework Integration ##

Since [ErlVoIP](ErlVoIP.md) is part of the [Erlang Internet Framework](http://erlsoft.org/about/), it will be abel to easily use the other applicaiton in the [Erlang Internet Framework](http://erlsoft.org/about/) to create more features. Some ideas on those are:

  * Use [ErlMail](http://erlsoft.org/modules/erlmail/) to email voice messages
  * Use [ErlWeb](http://erlsoft.org/modules/erlweb/) to create a web based configration application
  * use [ErlWeb](http://erlsoft.org/modules/erlweb/) to create a way to access vocie mail messages





