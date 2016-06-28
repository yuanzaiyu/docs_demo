====================
Agora Native SDK for Android Reference Manual
====================

Introduction
====================
The Agora Web SDK provides open access to the Agora Global Network from any device that supports a standard WebRTC-compliant browser, without requiring downloads or plugins. See the separate documentation and SDK for Agora Web SDK.
The Agora Native SDK for Android allows your Java code to perform the following operations:
 	* **Session setup**: Join and leave shared Agora conferencing sessions (identified by unique channel names), where there may be many global users conferenced together or simply one other user for one-to-one communication. Your application code should create and manage unique channel names; these usually originate in user, session, and date/time information that your application is already managing.
 	* **Media control**: Enable and disable voice and video (allowing muting) and set various voice and video parameters that help the Agora SDK optimize communications. Many of the SDK operations are automated and do not require developer intervention if these parameter settings are not provided.
 	* **Device control**: Access the microphone or speakerphone, set the volume, select from alternative cameras, and set the video window display.
 	* **Session control**: Receive events when other users join or leave a conferencing session (channel), and understanding who's speaking, who's muted, and who's viewing the session. These events allow the application to decide when to make changes to the delivery of video and audio streams, and other application-specific user and status information.
 	* **Quality management**: Obtain statistics and quality indicators about network conditions, run built-in tests, submit ratings and complaints about sessions and enable different levels of error logging.
 	* **Recording**: Record audio or video and audio in one or multiple channels simultaneously. This function is only applicable to the users who have adopted the Dynamic Key schema.
 	* **Data Encryption**: Encrypt the audio and video packets. You cannot use the recording function when the data encryption function is enabled in a channel.

The Agora Native SDK for Android provides two Java abstract classes to deliver these features.

* The **RtcEngine** class provides all the methods that can be invoked by your application.
* The **IRtcEngineEventHandler** class enables callback event notifications to your application.
For details, see Agora Native SDK for Android API Reference.


Required Development Environments
----------------
Test

Required Libraries
----------------
Test

Required Keys
----------------

Getting Started
====================

Obtaining SDK
----------------
Download the latest SDK from http://cn.agora.io/download or contact sales@agora.io.

Obtaining a Vendor Key
---------------------


See:doc:'Agora Native SDK for iOS</source/iOS_SDK>'

term (up to a line of text)
   Definition of the term, which must be indented

   and can even consist of multiple paragraphs

next term
   Description.


中文标题
    代码::

        for (var i=0; i++;){
            console.log('hello');
        }
