# Mailbox_Notifier
The Mailbox Notifier project alerts a user when their mailbox is opened (e.g. to deliver the mail).  The particular use case here is a 
mailbox that is located out on a public street some distance from the residence that it serves.  Mail delivery in the area is unreliable and
it is helpful to be notified when the mail is delivered.  

The mailbox is instrumented with a magnetic reed switch door sensor and a battery-operated low power LoRa Sensor in a weatherproof enclosure.
Opening the mailbox triggers the low power LoRa Sensor to send a LoRa message to a central Hub that is located inside of the residence.  
LoRa technology ensures reliable communication over a substantial open-air distance and then through the interior walls of the residence.

The Hub uses Particle Cloud publish/subscribe technology in conjunction with a Google App Script to ultimately send an SMS text or a Pushover
notification to the user’s mobile phone, indicating that the mailbox has been opened (i.e. to deliver the mail).

This project can also be used to indicate when a remote gate or door is opened, or similar applications.

See the "Mailbox_Notifier_Overview_Document" for details.


