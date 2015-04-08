# Introduction #

[ErlVoIP](ErlVoIP.md) is a voice over IP server written in Erlang. [ErlVoIP](ErlVoIP.md) will use SIP and RTP as the promary protocols to create connections between the PSTN and SIP clients.

[ErlVoIP](ErlVoIP.md) will also have a vocie mail and call processing server. This will allow calls to be redirected based on key pad information from the connected telephone.

Because this project is being design as part of the [Erlang Internet Framework](http://erlsoft.org/about/), this VoIP server will have access to [ErlMail](http://erlsoft.org/modules/erlmail/) for Email modules and [ErlWeb](http://erlsoft.org/modules/erlweb/) for web server modules. This means that features like emailing a voice mail message to a client will be easily included and a web based configuration applicaiton will also be part of the [design goals](DesignGoals.md).