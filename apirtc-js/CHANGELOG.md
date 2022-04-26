# Changelog

All Notable changes to apiRTC are documented in this file.

Latest version : [apiRTC Latest](https://cloud.apizee.com/apiRTC/v4.7/apiRTC-latest.min.js)

# [4.7.3](https://cloud.apizee.com/apiRTC/v4.7/apiRTC-4.7.3.min.js) - 2022-04-26

### Added

- Added Conversation#callVoIP
- Added CONVERSATION_WAITING_ROOM_PREFIX into apirtc.d.ts
- Added a separate apiRTC file with socket.io embedded
- Added UserAgent#getCPUArchitecture
- Added UserAgent#getDeviceVendor
- Added UserAgent#getDeviceModel
- Added UserAgent#getEngineName
- Added UserAgent#getEngineVersion
- Added deviceVendor, deviceModel, cpuArchitecture, engineName and engineVersion to basic userData

### Fixed

- Fixed Promise rejection upon register
- Fixed UserAgent#getBrowser

# [4.7.2](https://cloud.apizee.com/apiRTC/v4.7/apiRTC-4.7.2.min.js) - 2022-03-01

### Added

- Added Conversation#sendMessage options.token optionnal parameter
- Added Stream background image

### Changed

- Fixed apirtc.d.ts file
- Fixed documentation errors

# [4.7.1](https://cloud.apizee.com/apiRTC/v4.7/apiRTC-4.7.1.min.js) - 2022-02-16

### Added

- Added Contact#fetchUserData

### Changed

- Desactivated Stream#applyConstraint
- Desactivated Stream#setCapability
- Changed sentry events location for mute/unmute to Core
- Changed Stream#applyConstraints
- Changed Stream#getSettings
- Changed Stream#getConstraints
- Changed Stream#getCapabilities
- Removed Stream#askRemoteCapabilityAuthorization
- Removed Stream#acceptRemoteCapabilityRequest
- Removed Stream#refuseRemoteCapabilityRequest

### Fixed

- Fixed types for messages history


# [4.7.0](https://cloud.apizee.com/apiRTC/v4.7/apiRTC-4.7.0.min.js) - 2022-01-25

### Added

- Added Stream#enableVideo
- Added Stream#disableVideo
- Added Stream#enableAudio
- Added Stream#disableAudio
- Added Stream#getAudioFlowStatus
- Added Stream#getVideoFlowStatus
- Added Stream#getRemoteAudioFlowStatus
- Added Stream#getRemoteVideoFlowStatus
- Added Stream events :
  - audioFlowStatusChanged
  - videoFlowStatusChanged
  - remoteAudioFlowStatusChanged
  - remoteVideoFlowStatusChanged
- Added Contact#fetchUserData

### Changed

- Deprecated Stream#muteAudio
- Deprecated Stream#unmuteAudio
- Deprecated Stream#muteVideo
- Deprecated Stream#unmuteVideo

# [4.6.5](https://cloud.apizee.com/apiRTC/v4.6/apiRTC-4.6.5.min.js) - 2022-01-24

### Fixed

- Fixed room mode transition.

# [4.6.2](https://cloud.apizee.com/apiRTC/v4.6/apiRTC-4.6.2.min.js) - 2022-01-12

### Added

- Added Stream#applyConstraint
- Added Stream#applyConstraints
- Added Stream#mergeReality
- Added Stream#unmergeReality
- Added Conversation#fetchMessageHistory new "options.token" possibility
- Added EventCenter#disableStorage

### Changed

- Fixed token option for Conversation#fetchMediaList
- Deprecated Stream#setCapability
- Removed all references to Apizee from ApiRTC
- Removed cookie usage to sessionStorage
- Forced parameter bandwidth type to number for WebRTC_Client#setVideoBandwidth
- Forced parameter bandwidth type to number for ApiCCWebRTCClient#setRemoteVideoBandwidth
- Forced parameter bandwidth type to number for ApiCCWebRTCClient#setOverallIncomingVideoBandwidth
- Forced parameter bandwidth type to number for ApiCCWebRTCClient#setOverallOutgoingVideoBandwidth
- Forced parameter bandwidth type to number for ApiCCWebRTCClient#setPerCallIncomingVideoBandwidth
- Forced parameter bandwidth type to number for ApiCCWebRTCClient#setPerCallOutgoingVideoBandwidth
- Forced parameter kbps type to number for UserAgent#setTargetBandwidthUsage

# [4.6.1](https://cloud.apizee.com/apiRTC/v4.6/apiRTC-4.6.1.min.js) - 2021-11-24

### Added

- Added error message for these browsers : Baidu, baidu, UCBrowser, QQ, QQBrowser and QQBrowserLite

### Fixed

- Fixed Stream methods to remotely use capabilities functions

# [4.6.0](https://cloud.apizee.com/apiRTC/v4.6/apiRTC-4.6.0.min.js) - 2021-11-17

### Added

- Added Stream#blur
- Added conversation moderation.
- Added remote possibility on Stream functions : getCapabilities, getSettings, getConstraints, setCapability
- Added Stream#askRemoteCapabilityAuthorization
- Added Stream#acceptRemoteCapabilityRequest
- Added Stream#refuseRemoteCapabilityRequest
- Added Stream events :
  - streamCapabilities
  - streamSettings
  - streamConstraints
  - remoteCapabilityRequest
  - remoteCapabilityRequestAccepted
  - remoteCapabilityRequestRefused

### Fixed

- Fixed Promise rejection upon register with access token.

### Changed

- Removed sdpSemantics plan-b forcing for SIP calls
- Removed CloudAPI from apiRTC to the npm package.
- Removed all Stream helpers to set a specific capability : i.e. setTorch, setZoom, setContrast, etc...
- Removed Stream#setCapabilities

# [4.5.6](https://cloud.apizee.com/apiRTC/v4.5/apiRTC-4.5.6.min.js) - 2021-11-05

### Fixed

- Fixed hangup on set local/remote description failure.

# [4.5.5](https://cloud.apizee.com/apiRTC/v4.5/apiRTC-4.5.5.min.js) - 2021-09-27

### Added

- Added checking on apiRTC loading when loading with NPM

# [4.5.4](https://cloud.apizee.com/apiRTC/v4.5/apiRTC-4.5.4.min.js) - 2021-09-24

### Added

- Added Cloud events.
- Added checking on apiRTC loading

# [4.5.3](https://cloud.apizee.com/apiRTC/v4.5/apiRTC-4.5.3.min.js) - 2021-08-18

### Added

- Added meshOnlyEnabled option for Conversation/Conference (Session#getOrCreateConversation)
- Added JoinResult for Conversation#join

# [4.5.2](https://cloud.apizee.com/apiRTC/v4.5/apiRTC-4.5.2.min.js) - 2021-07-27

### Fixed

- Fixed 1-to-1 call with Safari calling without sending any media

# [4.5.1](https://cloud.apizee.com/apiRTC/v4.5/apiRTC-4.5.1.min.js) - 2021-07-20

### Fixed

- Fixed preCall test to avoid mesh mode
- Fixed session presenceGroup update on join/leaveSession
- Fixed Edge version checking for Datachannel

### Added

- Added Conversation#getSubscribedStream
- Added Laser mode on whiteboard

# [4.5.0](https://cloud.apizee.com/apiRTC/v4.5/apiRTC-4.5.0.min.js) - 2021-06-04

### Fixed

- Fixed asymmetric 1-to-1 call with Firefox
- Fixed Stream#createStreamFromUserMedia with enhancedAudioActivated when audio constraint is true
- Fixed call stats for Chrome 91

### Added

- Added simulcast (Conversation)
- Added streamId on Conversation events:

    - audioAmplitude
    - error
    - onCallStatsUpdate
    - remoteStreamUpdated
    - slowLink

### Changed

- Changed Conversation audioAmplitude event
- Deprecated Conversation#getAvailableStreamList
- PreCall test : added possibility to establish only one call for QoS testing with record

# [4.4.12](https://cloud.apizee.com/apiRTC/v4.4/apiRTC-4.4.12.min.js) - 2021-07-27

### Fixed

- Fixed 1-to-1 call with Safari calling without sending any media

# [4.4.11](https://cloud.apizee.com/apiRTC/v4.4/apiRTC-4.4.11.min.js) - 2021-05-05

### Fixed

- Fixed asymmetric 1-to-1 call with Firefox
- Fixed call stats for chrome 91

# [4.4.10](https://cloud.apizee.com/apiRTC/v4.4/apiRTC-4.4.10.min.js) - 2021-04-22

### Fixed

- Fixed asymmetric 1-to-1 call with Firefox
- Added check against null for options argument

### Changed

- Optimisation of blur filter video quality

# [4.4.9](https://cloud.apizee.com/apiRTC/v4.4/apiRTC-4.4.9.min.js) - 2021-03-19

### Fixed

- escape removeAllowExtmapMixed for Safari v14.0+ (605)

# [4.4.8](https://cloud.apizee.com/apiRTC/v4.4/apiRTC-4.4.8.min.js) - 2021-02-17

### Added

- Added TextDetection AIE filter

### Changed

- Modification on backgroundSubstraction filters :
  - FPS optimisation when a filter is applied

# [4.4.7](https://cloud.apizee.com/apiRTC/v4.4/apiRTC-4.4.7.min.js) - 2021-02-12

### Fixed

- Fixed subscription storm.

### Added

- Added STUN/TURN config from Cloud
- Added logLevel config from Cloud
- Added Session#getPresenceGroup
- Added Session#getSubscribedPresenceGroup

### Changed

- Modification on presence :
  - Optimisation of join/leave presence group
  - Optimisation of sub/unsub presence group

# [4.4.6](https://cloud.apizee.com/apiRTC/v4.4/apiRTC-4.4.6.min.js) - 2021-01-04

### Fixed

- Fixed ConversationCall#replacePublishedStream
- Fixed callStatsUpdate trigger increase after ConversationCall#replacePublishedStream

### Added

- Added AIE development

### Changed

- Allowed MOS score for 1-to-1 calls

# [4.4.5](https://cloud.apizee.com/apiRTC/v4.4/apiRTC-4.4.5.min.js) - 2020-11-26

### Fixed

- Fixed Stream#getCapabilities and Stream#setCapability compability with navigators

### Added

- Added helpers to control stream track capabilities

# [4.4.4](https://cloud.apizee.com/apiRTC/v4.4/apiRTC-4.4.4.min.js) - 2020-11-02

### Fixed

- Fixed call restart after reconnection
- Fixed missing hangup event on subscribe side in case of unpublish
- Fixed Stream#startRecord for Firefox
- Fixed updateSubscribedStream (streamId)
- Fixed unsubscribeToStream (streamId)

### Changed

- Use RTCRtpSender#setParameters (instead of SDP AS/TIAS field) to limit bitrate

### Added

- Added callStats emiting for 1-to-1 call

# [4.4.3](https://cloud.apizee.com/apiRTC/v4.4/apiRTC-4.4.3.min.js) - 2020-10-20

### Added

- Added firstMediaDeviceListInitialization on UserAgent#mediaDeviceChanged event

### Fixed

- Fixed call establishment and call clean up after mode transition
- Fixed cloud request on IE11
- Fixed instanceId change on republish stream

# [4.4.2](https://cloud.apizee.com/apiRTC/v4.4/apiRTC-4.4.2.min.js) - 2020-10-13

### Added

- Added distributedBroadcastEnabled option for Conversation#publish
- Added RessourceLoader to check Js dependancy loading

### Fixed

- Fixed remote logging integration
- Fixed updateMedia process to add more checkings status

# [4.4.1](https://cloud.apizee.com/apiRTC/v4.4/apiRTC-4.4.1.min.js) - 2020-09-25

### Added

- Added forceAudioAndVideoMediaElementSeparation option on addStreamInDiv and removeElementFromDiv
- Added media stream filtration functionality

### Fixed

- Fixed call clean up on unrecoverable error
- Fixed callHangup on CallDisconnection for P2P calls
- Fixed setRecvOnly for audio and video when direction is already inactive

# [4.4.0](https://cloud.apizee.com/apiRTC/v4.4/apiRTC-4.4.0.min.js) - 2020-08-03

### Fixed

- Fixed Conversation hangup event
- Fixed apiCCId cookie on beforeunload
- Fixed exports to have exported interface for UMD module
- Fixed precall recording, recording only the passed test call
- Fixed Datachannel on Edge > version 79
- Fixed DataChannel 'opened' event

### Changed

- Changed Conversation#pushData scheduling: only one at a time

### Added

- Allowed multiple connections of same apiCCId in conference.
- Added alternative method ApiCCUserMediaStream#listenToAudio2 to analyze audio amplitude
- Added Stream#audioAmplitudeInfo event contained speaking/sound status besides amplitude info
- Updated Stream#enableAudioAnalysis sound analysis method
- Added active option for Session#getOrCreateConversation
- Added NPM package generation support

# [4.3.23](https://cloud.apizee.com/apiRTC/v4.3/apiRTC-4.2.23.min.js) - 2020-07-06

### Fixed

- Fixed Conversation#unpublish

# [4.3.22](https://cloud.apizee.com/apiRTC/v4.3/apiRTC-4.3.22.min.js) - 2020-06-19

### Fixed

- Fixed P2P stream replacement created with ua#createStreamFromMediaStream
- Fixed second stream creation with a second camera on Firefox

# [4.3.21](https://cloud.apizee.com/apiRTC/v4.3/apiRTC-4.3.21.min.js) - 2020-06-05

### Fixed

- Fixed unordered packets during data channel transfer
- Fixed camera switching on iOS < 13 (ideal/exact constraints issue)
- Fixed recording for PreCallTest
- Fixed updateMedia process to add more checkings on signaling status and add retry management
- Fixed session control on subscribeToStreams
- Fixed calls signaling message checking with callId and instanceId
- Clean stored call candidate after one minute timer
- Fixed getDisplayMedia detection on ios Cordova
- Fixed Conversation#join (on failure)
- Fixed eventlistener error on eventCenter for reactNative
- Fixed ConversationCall#startRecordingPublishedStream while in mesh mode
- Fixed ConversationCall#startStreaming while in mesh mode
- Fixed to remove turns config for Edge version <= 44

### Added

- Added Conference#getInfo

# [4.3.20](https://cloud.apizee.com/apiRTC/v4.3/apiRTC-4.3.20.min.js) - 2020-05-12

### Added

- Added optional TTL for Consersation#startRecording
- Added optional TTL for ConsersationCall#startRecordingPublishedStream
- Added a TTL of 900 seconds for recordings of precall test
- Added optional sourceType of Conversation#pushData
- Added possibility to configure VP9 as prefered codec on P2P call
- Added screenSharingCompliant and qoSStatCompliant parameters on UserAgent#getCapabilities

# [4.3.19](https://cloud.apizee.com/apiRTC/v4.3/apiRTC-4.3.19.min.js) - 2020-04-27

### Fixed

- clone data on subscribeToStreams
- Add checking on feature deactivation on sendPresenceGroupManagementCommand
- conversationSpace definition on register with login or token
- Fixed screenSharing on Edge in mesh mode

### Added

- Added streamId in hangup event (conversation)
- Added videoForbidInactive by default

### Changed

- change default value on publish(video + screen) for switch to audio only to 50kbps

# [4.3.18](https://cloud.apizee.com/apiRTC/v4.3/apiRTC-4.3.18.min.js) - 2020-04-15

### Changed

- Modified control of call life-cycle.
- Changed 'anonymous' default username by 'guest'
- userData management on reconnect to accelerate synchronization

### Added

- Extended mediaDeviceChanged event with data that contains devices with updated labels

# [4.3.17](https://cloud.apizee.com/apiRTC/v4.3/apiRTC-4.3.17.min.js) - 2020-04-02

### Fixed

- Fixed conversationSpace join in case of channel reconnect
- Fixed presenceGroup join and subscribe in case of channel reconnect

# [4.3.16](https://cloud.apizee.com/apiRTC/v4.3/apiRTC-4.3.16.min.js) - 2020-03-30

### Fixed

- Fixed publish call restart on reconnection in mesh mode.
- Fixed calling evalOutgoingVideoBandwithCap() on caller side for P2P calls

# [4.3.15](https://cloud.apizee.com/apiRTC/v4.3/apiRTC-4.3.15.min.js) - 2020-03-24

### Changed

- Change error format to display all information from WebRTC API on createStream promise
- start updateMedia() on iceDisconnection only on caller side

### Added

- Added info on mediaDeviceChanged event to inform whether the event is generated after getUserMedia success
- Added entryAllowed/entryDenied events to the conference

### Fixed

- Fixed unnecessary stopMaxCallRetriesTimer()
- Fixed Promise reject on Conversation#publish failure

# [4.3.14](https://cloud.apizee.com/apiRTC/v4.3/apiRTC-4.3.14.min.js) - 2020-03-03

### Changed

- setAudioSourceIdInConstraint() and setVideoSourceIdInConstraint() to use constraints.video.deviceId by default
  and 'ideal' instead of 'exact'
- Modified Contact#sendMessage: removed Cloud api call to save message, duplicate entry in database.
- Modified updatePresence right after being accepted in conference by moderator

### Added

- Added sequential CCS socket message handler in ApiCCSession#handleSequentialMessage()
- Added call reestablishment (Conversation) after network loss
- Added QoS videoMinBitrate and videoStartBitrate (Conversation#publish)
- Added advice on slowLink (Conversation)
- Added data channel checking in case of page refresh
- Change createUserMediaErrorEvent() error format to display all information from WebRTC API, add gum_config info
- Added info on EventCenter logs
- Added EventCenter in public API
- Added info concernant added and removed media devices to mediaDeviceChanged event at event.detail.diff property
  > > > > > > > master

# [4.3.13](https://cloud.apizee.com/apiRTC/v4.3/apiRTC-4.3.13.min.js) - 2020-02-11

### Changed

- Remove call restart when "no candidate where retrieved" event after evolution on SFU side (Subscribe iOS issue)
- Change default value of SFU Connector

### Fixed

- Remove unnessary cleaning on beforeUnload Function
- Add values checking for PreCallTest on observeStreamPublished() an observeStreamSubscribed()
- setGetUserMediaConfig() to avoid malformed constraints
- Remove reinitialization of GumConfig on getMediaDevices

### Added

- Added EventCenter that handles error, userMediaError events. Possibility to request errors remotely.
- Added updatePresence right after being accepted in conference by moderator

### Changed

- Deprecated WebRTC_Client#setVideoBandwidth

# [4.3.12](https://cloud.apizee.com/apiRTC/v4.3/apiRTC-4.3.12.min.js) - 2020-01-30

### Fixed

- Fixed UserAgent#createStream signature
- Update for reactNative support
- Rollback fetchNetworkInformation() on first version as Version 2 can use too much bandwith for testing
- Fixed video cap for conferences with 3 participants and more

# [4.3.11](https://cloud.apizee.com/apiRTC/v4.3/apiRTC-4.3.11.min.js) - 2020-01-24

### Added

- Added option to disable checksum during pushData.
- Added posibility to configure bandwidthRatingThresholds on fetchNetworkInformation()

### Changed

- Modify fetchNetworkInformation() method for better network testings

### Fixed

- Added check on event values on onRemoteTrackAdded
- Forced SDP plan-b for SIP outgoing Call on Chrome

# [4.3.10](https://cloud.apizee.com/apiRTC/v4.3/apiRTC-4.3.10.min.js) - 2020-01-15

### Added

- Added checking on setGetUserMediaConfig() to avoid malformed constraints : Cannot use both optional/mandatory
  and specific or advanced constraints
- Added QoS videoForbidInactive option for subscription call.
- Added instanceId to identify calls on call restart
- Update user agent parser
- Keep instanceId for conf calls in P2P mode

### Fixed

- Fixed bitrate call update during multiple 1-to-1 calls.
- Fixed switching camera issue when recording on Cordova.

# [4.3.9](https://cloud.apizee.com/apiRTC/v4.3/apiRTC-4.3.9.min.js) - 2019-12-11

### Fixed

- Fixed canceled after success pushData notification.

### Changed

- Modified Conversation#cancelJoin signature.

### Added

- Added automatic call status check.

# [4.3.8](https://cloud.apizee.com/apiRTC/v4.3/apiRTC-4.3.8.min.js) - 2019-12-10

### Changed

- Added cause in localStreamUpdated and remoteStreamUpdated events (Conversation).
- Added delay on outgoing video cap during mode transition.

### Added

- Added max duration for calls retries
- Added delay management on calls retries
- Added error CALL_ABORTED event on #Conversation and #Call

# [4.3.7](https://cloud.apizee.com/apiRTC/v4.3/apiRTC-4.3.7.min.js) - 2019-11-28

### Fixed

- Fixed presenceGroup max limitation length to 750

# [4.3.6](https://cloud.apizee.com/apiRTC/v4.3/apiRTC-4.3.6.min.js) - 2019-11-26

### Fixed

- Fixed screenSharing publish without any audio/video device.

# [4.3.5](https://cloud.apizee.com/apiRTC/v4.3/apiRTC-4.3.5.min.js) - 2019-11-20

### Added

- Added meshPublish info in data
- Added possibility to set mimeType and quality argument on Stream#SnapshotOptions

### Fixed

- Fixed video cap for recorded 1-1 call.
- Fixed Conversation#pushData promise rejection in case of ICE failed.

# [4.3.4](https://cloud.apizee.com/apiRTC/v4.3/apiRTC-4.3.4.min.js) - 2019-11-04

### Added

- Added call stats for publisher, in Conversation, in mesh mode.
- Added meshPublish info in callList for reconnectContext
- Added possibility to configure width and height on takesnapshot (V3 API)
- Added the mail property into the UserAgent user data.

### Changed

- Modified UserAgent#setOverallOutgoingVideoBandwidth, constraint applied immediately.
- Modified UserAgent#setPerCallOutgoingVideoBandwidth, constraint applied immediately.
- Modified pushData - wait for ack to determine success.
- Removed force sdpSemantics plan-b for Chrome >= 78

### Fixed

- Added asymmetric 1-to-1 recorded call.

# [4.3.3](https://cloud.apizee.com/apiRTC/v4.3/apiRTC-4.3.3.min.js) - 2019-10-10

### Added

- Added asymmetric 1-to-1 recorded call.
- Added cloudConversationId for Contact#call options.
- Added apiRTC.webRTCCompliant and apiRTC.isWebRTCCompliant().
- Added checking on getSupportedConstraints() method support on device.
- Added userMediaError on UserAgent.
- Added apiRTC.qoSStatCompliant and apiRTC.isQoSStatCompliant().
- Added UserAgent#getCapabilities(), UserAgent#getBrowser(), UserAgent#getBrowserMajorVersion(), UserAgent#getBrowserVersion()
- Added UserAgent#getOsName(), UserAgent#getOsVersion(), UserAgent#getBrowserInfo(), UserAgent#getBrowserDetails()

### Changed

- Modified CloudApi success condition (in 200-range).

#### Fixed

- Force HD resolution instead of fullHD for iOS 13 devices.
- Fixed enableActiveSpeakerDetecting threshold.
- Fixed stream#type on audio only subscribe.

# [4.3.2](https://cloud.apizee.com/apiRTC/v4.3/apiRTC-4.3.2.min.js) - 2019-10-01

#### Changed

- Changed default CCS connexion protocol to HTTPS

# [4.3.1](https://cloud.apizee.com/apiRTC/v4.3/apiRTC-4.3.1.min.js) - 2019-09-09

### Added

- Added apiLibType parameter on connection for conversationSpace checking.
- Added getCapabilities() on mediaDevice to get supported resolution ...etc... on media devices

#### Fixed

- Fixed clearDisputableEntry() issue on second media flow when switching from P2P mode to SFU

### From 4.2.33

#### Fixed

- Fixed audio addition on video-only 1-to-1 call for Safari.
- Fixed audio-only and video-only 1-to-1 call for Firefox.

# [4.3.0](https://cloud.apizee.com/apiRTC/v4.3/apiRTC-4.3.0.min.js) - 2019-09-05

### Added

- Removed the restrictions on the number of simultaneous joined conversations.
- Added composite activation (Conversation).
- Added compositeListChanged event (Conversation).
- Added replayListChanged event (Conversation).
- Added subscription of composite stream (Conversation).
- Added subscription of replay streams (Conversation).
- Added start-before-stop room mode transition.
- Added start/stop recording (Call).
- Added Session#error event

# [4.2.34](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.34.min.js) - 2019-09-16

Merged into 4.3.1

### Fixed

- Fixed audio-only and video-only 1-to-1 call for Firefox.

# [4.2.33](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.33.min.js) - 2019-09-09

Merged into 4.3.1

### Fixed

- Fixed audio addition on video-only 1-to-1 call for Safari.

# [4.2.32](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.32.min.js) - 2019-09-05

### Fixed

- Fixed audio addition on video-only 1-to-1 call for Firefox and Safari.

# [4.2.31](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.31.min.js) - 2019-08-20

### Fixed

- Fixed subsequent recorded calls.

# [4.2.30](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.30.min.js) - 2019-08-19

### Fixed

- Added possibility to take snapshot from an existing div (issue on iOS)

# [4.2.29](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.29.min.js) - 2019-08-07

### Fixed

- Fixed audio addition on video only 1-to-1 call for iOS.

# [4.2.28](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.28.min.js) - 2019-07-25

### Fixed

- Fixed switch camera after having add a video track to a audio only 1-to-1 call.
- Fixed screen sharing for Chrome 72/73.

# [4.2.27](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.27.min.js) - 2019-07-23

### Fixed

- Fixed switch camera in SFU mode.

# [4.2.26](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.26.min.js) - 2019-07-17

### Fixed

- Fixed whiteboard on IE.
- Fixed idPersistenceTimeout after page reload.
- Fixed getUserMedia constraints for video-only 1-to-1 call.

# [4.2.25](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.25.min.js) - 2019-07-08

### Added

- activateScreenSharing on UserAgent to enable screenStream creation in offline mode
- Stream#getLabels() to get the labels of devices sources used for the stream

### Fixed

- Fixed video addition on audio 1-to-1 call.
- Fixed destCallType for video only 1-to-1 call.

# [4.2.24](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.24.min.js) - 2019-07-01

### Fixed

- Fixed streamListChanged events during room mode transition.

# [4.2.23](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.23.min.js) - 2019-07-01

### Added

- Added user defined context for publish.
- Added Stream#createDisplayMediaStream() to support constraints parameters for getDisplayMedia()
  (add screenSharing compatibility on Opera, Vivaldi, Brave, Safari Preview ... )

### Changed

- Added use of ontrack chrome 64+.

### Fixed

- Fixed call restart with channel disconnection.
- Fixed pointer sharing activation after guest refesh.
- Fixed audio addition on video only 1-to-1 call (and reverse).

# [4.2.22](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.22.min.js) - 2019-06-28

### Fixed

- Fixed room mode transition.

# [4.2.21](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.21.min.js) - 2019-06-18

### Added

- Added ccsToken parameter in Session

### Fixed

- Fixed media type selection on incoming call.
- Fixed SIP number detection

# [4.2.20](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.20.min.js) - 2019-06-18

### Fixed

- Masked unwanted streamListChanged events during room mode transition.
- Issue on media device presence status

# [4.2.19](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.19.min.js) - 2019-06-12

### Fixed

- Fixed switch camera on Safari iOS.
- Add checking on constraints format in setAudioSourceIdInConstraint and setVideoSourceIdInConstraint
- Fixed missing audio/video tracks from remote after switch camera.

### Added

- Added Token parameter on userAgent#register()

# [4.2.18](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.18.min.js) - 2019-06-11

### Changed

- Replaced PUT/DELETE methods by POST method and added \_method parameter accordingly, in CloudApi.

### Fixed

- Fixed destCallType set to audio (instead of audioOnly).
- Fixed audio-only publish call when getUserMedia is done during call establishment.

# [4.2.17](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.17.min.js) - 2019-06-04

### Added

- Added audio/video mute info in streamListChanged event (Conversation).
- Added getUserMedia timeout for Chrome.

### Changed

- Modified fetch-retry parameters for Conference#setTags.
- Fixed composite recording after room mode transition.

# [4.2.16](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.16.min.js) - 2019-05-16

### Added

- Added streaming management on ConversationCall.
- Added idPersistenceTimeout parameter for UserAgent#register.

### Changed

- UserAgent#setOverallIncomingVideoBandwidth accepts illegal value (0 or less) to disable the limit.
- UserAgent#setOverallOutgoingVideoBandwidth accepts illegal value (0 or less) to disable the limit.
- UserAgent#setPerCallIncomingVideoBandwidth accepts illegal value (0 or less) to disable the limit.
- UserAgent#setPerCallOutgoingVideoBandwidth accepts illegal value (0 or less) to disable the limit.

### Fixed

- Fixed getStats for Firefox 63 and newer.
- Fixed selected candidate for Chrome based browsers.

# [4.2.15](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.15.min.js) - 2019-05-07

### Added

- Added metadata param on cloudApi#saveGroupChatMessage
- Added metadata to group chat message.
- Added tags management.

# [4.2.14](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.14.min.js) - 2019-04-26

### Added

- Added bandwidth reservation process.
- Added overwrite option for Conversation#pushData.
- Added ttl (time to live) option for Conversation#pushData.
- Added videoStartQuality for conference publish.
- Added transfer start timeout for Conversation#pushData.
- Added better pc_config management and add mp2.apizee.com
- Added possibility to configure width and height on stream#takeSnapshot()
- Added Conversation#getContactsNumber()

### Changed

- Change screen sharing stream type to _STREAM_TYPE_VIDEO_.
- Change conference waiting room implementation.
- Removed H.264 restriction for Safari 12.1 and higher.
- Added delay before joining waiting room.

### Fixed

- Added room ID check upon session update.
- Reject promise on addMedia()
- ReplacePublishedStream promise take addMedia() result into account
- Fixed roomJoined parameter value to enable whiteboard restart
- Fixed subscription to an unmuted (initially muted) feed.
- Fixed Manage case when mediaDevice are detected on userAgent and mediaDeviceChanged handler is not yet setted
- Fixed takeSnapshot modif and documentation

# [4.2.13](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.13.min.js) - 2019-04-11

### Fixed

- Fixed issue on UserAgent#getUserMediaDevices() on Safari 12.1
- Fixed issue on call renegotiation on Safari 12.1

# [4.2.12](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.12.min.js) - 2019-04-10

### Added

- Added Conference#eject.
- Added ReceivedConversationJoinRequest export.
- Added (Conversation/Conference) messageNotDelivered event.

### Fixed

- Fixed call restart.
- Fixed destCallType value : add checking on setRemoteCallProfile to process on publish or shareScreen message
- Fixed update adapter.js - issue with publish on Safari
- Fixed mediaConstraints for createOffer on old chrome version (< 55)

# [4.2.11](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.11.min.js) - 2019-04-04

### Added

- Added userAcceptOnIncomingScreenSharingCall parameter on UserAgent#register() to enable invitation management
  on screenSharing incoming calls
- Added for screenSharing on acceptCall() : forcing unidirectionnal call
- Added Contact#incomingScreenSharingCallInvitation
- Added Session#incomingScreenSharingCallInvitation
- Added filtering if a second 200OK is received for a call (call forking)
- Added recordingStopped event in Conversation/Conference.
- Added Conversation#isRecorded
- Added Conversation#getRecordingInfo
- Added ConversationCall#isRecorded
- Added ConversationCall#getRecordingInfo
- Added Session#joinConversationSpace()
- Added Session#leaveConversationSpace()
- Added SIP info in StreamInfo (Conversation)

### Changed

- Made CloudApi#setCloudURL static.
- Added additional info in recording related events.
- Fixed (Conversation) transferEnded event.
- Fixed CloudApi for headers.
- Added apiCCId forgetting on authenticated session disconnection.

# [4.2.10](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.10.min.js) - 2019-03-21

### Fixed

- Fixed blurLevel issue on takesnapshot()

# [4.2.9](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.9.min.js) - 2019-03-20

### Fixed

- Fixed conversationSpace initialisation in case of apiRTC re-init
- Remove unuseful "call not found" warning

# [4.2.8](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.8.min.js) - 2019-03-18

### Added

- Added checkMutingStateForUserMedia to control muting state in P2P conference.
- Added support of conversationSpace
- Added screenSharing with getDisplayMedia API for Chrome > 72
- Added Promise return on stopNewWhiteboardSession()
- Added control on apiCCId (128 characters maximum)
- Adding static code analysis

# [4.2.7](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.7.min.js) - 2019-02-21

### Added

- Added apiKey format control.
- Added Conversation#getStreamInfo
- Added videoOnly parameter on Conversation#PublishOptions and Conversation#SubscribeOptions
- Added chatbot messaging.
- Added strip of rtcp-fb parameters on updateSDPcodecs

### Fixed

- Fixed waiting room.
- Fixed browser detection in checkCandidateTypes

# [4.2.6](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.6.min.js) - 2019-02-15

### Added

- Added osName osVersion into joinSession message.
- Added new configuration of composite recording.

### Merged 4.1.38

#### Added

- Added control to avoid Datachannel activation on Edge as it is not supported.

# [4.2.5](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.5.min.js) - 2019-02-12

### Fixed

- Fixed bug on video-only and screen sharing.

# [4.2.4](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.4.min.js) - 2019-02-11

### Added

- Added Conversation#cancelPushData.

### Fixed

- Fixed mute/unmute for remote stream.
- Fixed checking on Whiteboard join

# [4.2.3](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.3.min.js) - 2019-01-30

### Added

- Added facingMode option on UserAgent#createStream

### Fixed

- fix PreCall test
- fix on takeSnapshot to use the size of live video

### Merged 4.1.37

#### Fixed

- Fixed issue : only one instance of babel-polyfill is allowed

# [4.2.2](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.2.min.js) - 2019-01-15

### Modified

- Changed peer connection configuration for Firefox 53 and newer.

### Merged 4.1.36

#### Fixed

- Fixed CallType on events when using a screenSharing stream

### Merged 4.1.35

#### Modified

- Call getMediaDevices() in userMediaSuccess on all browsers (was only done for Safari and Edge)
- Setting video Bandwidth default values to 3Mo for overallIncoming and overallOutgoing (used for conference)

# [4.2.1](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.1.min.js) - 2019-01-14

# Modified

- Replaced renegotiation by unpublish/publish to avoid audio-video desync during switch camera.

# [4.2.0](https://cloud.apizee.com/apiRTC/v4.2/apiRTC-4.2.0.min.js) - 2018-12-19

### Added

- Added support for multiple conversations.
- Added setting videoBandWidth after publish (on live).
- Added pointer sharing on Session.
- Added possibility to upload logs to Cloud

# [4.1.34](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.34.min.js) - 2019-01-15

### Modified

- Changed peer connection configuration for Firefox 53 and newer (TURNS).

# [4.1.33](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.33.min.js) - 2019-01-11

### Added

- Force sdpSemantics to 'plan-b' for Chrome >= 72
- Deactivate user id conversion to numeric by default
- Add registerInformation#idConversionActivated parameter to keep the possibility to convert user id

# [4.1.32](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.32.min.js) - 2018-12-21

### Fixed

- Fixed callConfiguration setting management on meshPublish

# [4.1.31](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.31.min.js) - 2018-12-10

### Fixed

- Fixed moderation on guest side (access-ack).
- Fixed callType for screenSharing call.
- Fixed page unload detection on Mobile Safari for correct disconnection and apiCCId preservation

# [4.1.30](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.30.min.js) - 2018-12-04

### Fixed

- Fixed support for audio-only and video-only user media grab.
- Fixed call restart after screenSharing extension installation on Chrome
- Fixed screenSharing extension installation management for Chrome 71

# [4.1.29](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.29.min.js) - 2018-11-28

### Added

- Added "Muted" and "NoStream" values to QoS quality scores.

### Fixed

- Fixed resolution parameter for videoQuality model.
- Fixed Stream recording. Issue when playing recorded files on Windows.

# [4.1.28](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.28.min.js) - 2018-11-23

### Fixed

- Fixed camera checking and selection on Safari iOS (2).
- Added check on startCallStatsMonitoring for Safari : only supported on Chrome and Firefox for now.

# [4.1.27](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.27.min.js) - 2018-11-22

### Added

- Added check on WebRTCClient#enableQos() : only supported on Chrome and Firefox for now.
- Added check on WebRTCClient#enableCallStatsMonitoring() : only supported on Chrome and Firefox for now.
- Added check on WebRTCClient#enableQualityEvaluating() : only supported on Chrome and Firefox for now.
- CloudAPI#setCloudURL()

### Fixed

- Fixed WebRTCClient#getMediaDevices() to update UserAgent#getUserMediaDevices().
- Fixed micro selection on Safari iOS.
- Fixed camera checking and selection on Safari iOS.

# [4.1.26](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.26.min.js) - 2018-11-20

### Fixed

- Fixed call restart and stream protection.
- Fixed deactivation of active speaker on iOS-Cordova.

# [4.1.25](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.25.min.js) - 2018-11-20

### Added

- Added check on CallStatsMonitoring : only supported on Chrome and Firefox for now.
- Added Conversation#audioAmplitudeUpdate event.

# [4.1.24](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.24.min.js) - 2018-11-15

### Added

- Added Stream#addInDiv() Stream#removeFromDiv() helpers to manage adding video in DOM.
  These methods includes support of Safari autoplay policies constraints to avoid WebRTC audio/video plays issues.
- Added Conversation#hangup event.

### Fixed

- Switch Camera on iOS.
- Fixed auto subscribe restart after failure. Use Conversation#streamAdded and Conversation#streamRemoved to update DOM.

# [4.1.23](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.23.min.js) - 2018-11-12

### Added

- Added UserAgent#enableCallStatsMonitoring
- Added UserAgent#enableActiveSpeakerDetecting

### Changed

- addStream() and removeStream() to use addTrack / replaceTrack API by default
- enhancedAudioActivated : add checking to activate only on Chrome

### Fixed

- Compatibility with Vivaldi Browser v1 and v2
- Removed entry from userMediaStreamTable after failure

# [4.1.22](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.22.min.js) - 2018-10-30

### Added

- Added call auto restart when no candidate is found (Safari 12 without getUserMedia).

### Added

- Added active speaker detecting

### Changed

- Modified PeerConnection event for Safari 12 (ontrack instead of onaddstream).

### Fixed

- Fixed renegotiation for subscriber in mesh conference.

# [4.1.21](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.21.min.js) - 2018-10-18

### Added

- Added descriptor for ICE error.
- Added event for distant ICE error.

# [4.1.20](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.20.min.js) - 2018-10-12

### Added

- Added Conference#cancelJoin.
- Added enabling video quality events on Session
- Added frame resolution statistics for sent stream

### Modified

- Enabled dataChannel on Safari version 11 and later

# [4.1.19](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.19.min.js) - 2018-10-09

### Added

- Added recording (userStream/composite) in Conversation.
- Added Conference#cancelJoin.

### Modified

- Enabled dataChannel on Safari version 11 and later

### Fixed

- Fixed firing MediaDeviceChanged Event on UserAgent's instantiation
- Fixed bug of wrong subscribe to replay.

# [4.1.18](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.18.min.js) - 2018-10-02

### Added

- checking call state on updateSubscribedStream() to avoid SDP negotiations error

### Modified

- fire "CallEstablished" event on set remoteDescription success

### Fixed

- add control on userData value
- add error value on createScreensharingStream() promise reject

# [4.1.17](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.17.min.js) - 2018-09-26

### Fixed

- Fix for Hangup on iOS Cordova

# [4.1.16](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.16.min.js) - 2018-09-25

### Added

- add screenSharing support on Edge (only available on Windows 10 Pro or Enterprise)

### Fixed

- Fixed issue on call establishment with Edge (call peer to peer and publish to conference)
- Fixed issue with Chrome 55

# [4.1.15](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.15.min.js) - 2018-09-20

### Modified

- Remove subscribeToMedia and unsubscribeToMedia from API Doc. These methods are not useful.
- Improve mediaDevice change detection for Safari and Edge. Add posibility to activate apiRTCMediaDeviceDetectionEnabled on Safari

# [4.1.14](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.14.min.js) - 2018-09-12

### Added

- mediaDeviceChanged event support by apiRTC on Chrome/Android as not supported by browser (parameters apiRTCMediaDeviceDetectionEnabled, apiRTCMediaDeviceDetectionDelay)
- add enhancedAudioActivated parameters on CreateStreamOptions

# [4.1.13](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.13.min.js) - 2018-09-10

### Fixed

- Fixed on userData update when user already in contact list

### Modified

- Get active session if no session is passed as options parameter for Conversation#checkAccess

# [4.1.12](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.12.min.js) - 2018-09-04

### Added

- Added conference waiting room messages for exchange with izeeconf.
- Added 'statusChange' event in Invitation (Available for all kinds of invitation)
- Added Invitation status : Constants.INVITATION_STATUS_CANCELLED
- Added Invitation status : Constants.INVITATION_STATUS_ENDED
- Added cancel() on SendInvitation for FileTransferInvitation - sendFile()
- type parameter on Invitation

### Fixed

- Correction for fileInfo value on Invitation
- Correction of remoteId on 'hangup' event
- Correction of callId value on 'userMediaStop' event

### Modified

- Added convId parameter for fetchEnterpriseInformations
- Added sessionId parameter as value returned by fetchEnterpriseInformations

### Deprecated

- 'expired' event on ReceivedCallInvitation : check 'statusChange' event
- 'expired' event on ReceivedDataChannelInvitation : check 'statusChange' event
- 'response' event on SentInvitation : check 'statusChange' event

# [4.1.11](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.11.min.js) - 2018-08-22

### Fixed

- Fixed IE11 console issue
- Fixed subscribe audio only and video only in P2P conference.

### Added

- Added ApiCCWebRTCClient#updateMediaTypeOnCall
- Added videoOnly option for Conversation#subscribeToStream
- Added Conversation#updateSubscribedStream

# [4.1.10](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.10.min.js) - 2018-08-21

### Fixed

- avoid exception on loadJs if file is requested twice
- Fixed IE8 / IE11 support (avoid devices detection, update call management)
- Added audio/video mute support for P2P conference.

# [4.1.9](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.9.min.js) - 2018-08-20

### Fixed

- Cleaning whiteboard elements on start() and stop()
- Whiteboard drawingId on annotation
- Fixed issue on contact creation when userAgent is not completely instantiated
- Fixed issue on contactListUpdate when session is not completely instantiated

# [4.1.8](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.8.min.js) - 2018-08-11

### Added

- Added UserAgent#fetchGeolocationInformation in DTS file
- Added Conversation#getStatus
- Added Stream#getOwner
- Added the possibility to initialize some userData parameters at register
- Added streamId in localStreamUpdated event fired by Conversation

### Fixed

- Removed Stream#isLocal in DTS file
- Added missing return in UserAgent#getUsername and UserAgent#getPhotoUrl
- Added missing Stream#callId property in DTS file
- Fixed Stream#streamId property type in DTS file
- Fixed remoteStreamUpdated event firing order

### Modified

- Removed \_contactCache on Conversation
- Modification of Contacts management on users presence :
  - Optimisation of connectedUsersListUpdate event management
  - Remove updatePresence event process
  - Remove throttle on Contacts list update
  - Avoid creation of Contact for own user

### Fixed

- removed Conversation#contactListUpdate as not filtered by conversation and events contactJoined / contactLeft are more precise
- add filtering of incomingCall event for conference calls

# [4.1.7](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.7.min.js) - 2018-08-07

### Added

- Added (transfer) id for transferBegun, transferProgress and transferEnded events (Conversation)
- Added Conversation#isPublishedStream
- Added audio/video update from audio-only and video-only calls in Conversation
- Added MCUAvailableStreamUpdate event (Core)
- Added Conversation#checkAccess
- Added access-ack on moderation granted
- Added Session#getOrCreateConference
- Added check for electron application

### Modified

- Added possibility to get a blob instead of dataURI from takeSnapshot
- Added isRemote property on Stream
- Speed up data channel transfer to cloud
- Added wait for CCS ack before closing data channel after transfer
- Removed call auto-accept when no audio and video present
- Added convId optional parameter to Enterprise#fetchSiteAgents
- Added moderator info in Conversation#checkAccess result
- Modified special receiveData listener in Conference
- Fixed missing return after reject in CloudApi#cloudRequest
- Fixed missing values in Conversation#checkAccess result

### Fixed

- Added UserAgent#getDefaultDevices in DTS file
- Set stream parameter as optional for Conversation#publish in DTS file
- Added UserAgent#getUserMediaDevices in DTS file

# [4.1.6](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.6.min.js) - 2018-07-20

### Added

- Added UserAgent#fetchGeolocationInformation
- Added CloudApi (public)

### Fixed

- Fixed fileTransfer for file of type string

# [4.1.5](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.5.min.js) - 2018-07-17

### Fixed

- Fixed error during data call when audio/video is globally muted.
- Added clean up of mesh published stream on leaveSession.
- Fixed Conversation#destroy and Conference#destroy.
- Fixed error when publishing audio-only stream in P2P conference.

# [4.1.4](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.4.min.js) - 2018-07-11

### Modified

- Added class UserData to represent user data of user agent and contact.
- Fixed dataChannel transfer (onclose not supported on firefox).
- Modified total hang up order.
- Added clean up of MCU session on leave.

# [4.1.3](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.3.min.js) - 2018-07-06

### Added

- Generation of lib version min.debug

### Fixed

- apiDBActivated is now activated by default (case of connection/deconnection)

# [4.1.2](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.2.min.js) - 2018-07-05

### Added

- Added tests for mute/unmute during calls.
- Added remoteStreamUpdated event in Call.

### Modified

- Added listeners clean up in Call.
- Added remoteId in userMediaSuccess event.

# [4.1.1](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.1.min.js) - 2018-07-05

### Added

- Session#getOnlineContactsArray()
- PreCallTest() function

### Modified

- apiDBActivated is now activated by default

### Fixed

- createStream with videoInputId false was creating a video stream

# [4.1.0](https://cloud.apizee.com/apiRTC/v4.1/apiRTC-4.1.0.min.js) - 2018-06-29

### Added

- ReceivedCallInvitation#getCall()
- Events Contact#incomingCall
- Events Contact#incomingScreenSharingCall
- Events Session#incomingScreenSharingCall
- Events Call#userMediaError
- Events Call#desktopCapture
- Call creation when invitation is received
- Session#getOrCreateContact()
- Session#getCall()
- Session#getCalls()
- Session#getContactsArray()
- Stream#getLocalStreams()
- Stream#getStream()
- Contact#shareScreen()
- Possibility to configure captureSourceType on Stream#createScreensharingStream

### Fixed

- Fixed call.callConfiguration merge on acceptCall
- Checking if audioReceived present for QoS statistics.
- Fixed mute/unmute (state variable duplication)
- Fixed tryAudioCallAfterUserMediaError
- Fixed mute state for muted call establishment.

### Modified

- Removed use of MediaStream#clone.
- Added check for roomId on ApiCCWebRTCClient#joinMCUSession
- Deprecation of Session#getContact() replaced by Session#getOrCreateContact()
- Cleaning of Stream#createScreensharingStream
- Modified localStreamUpdated and remoteStreamUpdated event firing.

# [4.0.14](https://cloud.apizee.com/apiRTC/v4.0/apiRTC-4.0.14.min.js) - 2018-06-29

### Fixed

- Remove typeof control on inviteInRoom
- Fixed when a video stream is used to establish call and call is audioOnly : call was using video
- Fixed SDPManager#setSendOnlyForAudio
- Fixed SDPManager#setSendOnlyForVideo
- Fixed SDPManager#setSendOnly
- Fixed SDPManager#setRecvOnlyForAudio
- Fixed SDPManager#setRecvOnlyForVideo
- Fixed SDPManager#setRecvOnly

### Modified

- Modified Call#replacePublishedStreams: resolve the returned promise only when the action is done.

### Added

- Added Call#stopPublishedStreams

# [4.0.13](https://cloud.apizee.com/apiRTC/v4.0/apiRTC-4.0.13.min.js) - 2018-06-26

### Added

- Added ConversationCall, created by Conversation/Conference on publish.
- Added ConversationCall#replacePublishedStream.
- Added Conversation#destroy to release conversation resources.
- Added Conference#destroy to release conference resources.

### Modified

- Added callbacks parameters for Call#replacePublishedStream.
- Removed remaining reference of previous UserMediaStream in WebRTC_Client#addMedia.

# [4.0.12](https://cloud.apizee.com/apiRTC/v4.0/apiRTC-4.0.12.min.js) - 2018-06-25

### Added

- Added pointer sharing roomType.
- Added nickname in options for anonymous UserAgent#register.

### Fixed

- Whiteboard optimisation :
  - History is now managed by CCS in case of disconnection / reconnection
  - Whiteboard cursor is deactivated by default (invisible))
  - Added capabilities detection on userAgent to deactivate cursor on iOS
  - Not sending cursor information when cursor is set to invisible
  - Avoid redraw when not necessary

# [4.0.11](https://cloud.apizee.com/apiRTC/v4.0/apiRTC-4.0.11.min.js) - 2018-06-20

### Added

- Added possibility to set userAccept on incoming dataCall on User Agent (RegisterInformation).

### Modified

- Removed 'Conversation.' prefix from Conversation.
- Added timeout for webRTCClientCreated event firing.
- Fixed undefined address for turn server.

### Fixed

- Fixed issue on webRTC library usage when using Safari and cordova is defined

# [4.0.10](https://cloud.apizee.com/apiRTC/v4.0/apiRTC-4.0.10.min.js) - 2018-06-14

### Added

- Added QoS preferences for Conversation#publish
- Added uuid from CCS on groupChatMessage sending

### Fixed

- Fixed Call#replacePublishedStreams for mute/unmute
- Fixed updatePresence request to cloud for conference

# [4.0.9](https://cloud.apizee.com/apiRTC/v4.0/apiRTC-4.0.9.min.js) - 2018-06-07

### Added

- Added Events Conversation#disconnectionWarning
- Added Events Conversation#error
- Added UserAgent#enableMeshRoomMode()
- Added UserAgent#fetchProfileInformation()
- Added UserAgent#getPhotoUrl()
- Added events on Stream
  - Added Stream#activeStateChange
- Added events on Conversation
  - Conversation#localStreamUpdated
  - Conversation#remoteStreamUpdated
  - Conversation#slowLink
- Added possibility to set turn server address on User Agent (RegisterInformation). This parameter is a global parameter : all established calls will use this turn server.
- Added possibility to set turn server address on Conversation#publish() (PublishOptions) . This parameter is only set for the published call.
- Added possibility to set turn server address on Conversation#subscribeToStream() (SubscribeOptions) . This parameter is only set for the subscribed call.
- Added possibility to set turn server address on Conversation#pushData() (PushDataOptions) . This parameter is only set for the data call.

### Fixed

- Fixed parameter token update on deconnection/reconnection

# [4.0.8](https://cloud.apizee.com/apiRTC/v4.0/apiRTC-4.0.8.min.js) - 2018-05-30

### Added

- Added control to avoid Stream constructor usage, please use a static method of class Stream such as : createStreamFromUserMedia, createStreamFromMediaStream, createScreensharingStream
- Cleaning code on deprecated usage of selectedUserMediaStreamId
- Added Events Session#reconnecting
- Added possibility to configure contactDisconnectionDelay (RegisterInformation)

### Fixed

- Fixed Session events list checking to add : 'disconnect' and 'error'

# [4.0.7](https://cloud.apizee.com/apiRTC/v4.0/apiRTC-4.0.7.min.js) - 2018-05-28

### Added

- Added possibility to configure ccs connection retries number and delay (RegisterInformation)

### Fixed

- Fixed issue on removeGroupDataFromConnectedUsersList when user leave conference

# [4.0.6](https://cloud.apizee.com/apiRTC/v4.0/apiRTC-4.0.6.min.js) - 2018-05-24

### Added

- Added UserAgent#externalJsLoadingStatus event to be informed on external Js status : loaded, error or retry. This can be an insteresting information to detect network failure.
- Added UserAgent#ccsConnectionStatus event to be informed on CCS connection status : connected, disconnected, error, retry
- Added possibility to configure external Js loading retries number and delay (RegisterInformation)
- Added result to joinMCUSessionAnswer event

### Modified

- Optimize bandwidth test duration

### Fixed

- Fixed issue on stream cleaning when replacePublishedStream is used

# [4.0.5](https://cloud.apizee.com/apiRTC/v4.0/apiRTC-4.0.5.min.js) - 2018-05-17

### Added

- MediaDevice Manager to improve getting media devices and update when a device is added or removed
- UserAgent#getUserMediaDevices
- UserAgent#getDefaultDevices

### Fixed

- Fixed UserAgent#RegisterInformation : remove presence group subscription when joining : this is done using parameter subscribeTo
- Fixed issue on presenceGroupManagement when disconnect/reconnect
- Fixed issue on UserAgent#fetchNetworkInformation
- Fixed issue to use requirejs : conflict with webpack
- update bandwidthRatingThresholds

### Modified

- Change asynchronous js loader in order to have retries and error management

### Removed

- Removed Presence group subscription to visitor - agent when connecting with apiKey : presence & subscribe group must be unset by default

# [4.0.4](https://cloud.apizee.com/apiRTC/v4.0/apiRTC-4.0.4.min.js) - 2018-04-26

### Modified

- Stream#startRecord now return a promise
- Stream#stopRecord now return a promise with Blob of recorded stream
- Stream#pauseRecord now return a promise
- Stream#resumeRecord now return a promise

### Added

- Constants.ERROR_STREAM_RECORD : used to identify error on stream recording

# [4.0.3](https://cloud.apizee.com/apiRTC/v4.0/apiRTC-4.0.3.min.js) - 2018-04-24

### Fixed

- Stream release when a stream is provided on call and conversation
- Stream muting/unmuting (audio & video) when a stream is provided on call and conversation
- Fixed screensharing for Firefox : default captureSourceType is now "screen"
- Fixed parameter restarted on deconnection/reconnection on UserMediaSuccess Event
- Fixed call restarting with MCU when disconnection
  - restart on bye "disconnect" reason
  - userMediaStream presence and active state checking on restart
- Fixed usage of plugin functions for iOS/cordova

### Modified

- Check apiKey modification on apiCCId checking when reloading page
- Update events handlers on CCS connection
- Modified ApiCCWebRTCClient#updateMediaDeviceOnCall: replaced stream parameter (deprecated) by userMediaStreamId.

### Added

- Added warning when no candidate are retrieved from ice agent on call
- Added support for WebRTC evolution API on Firefox-59 and Chrome-65 on addStream() and removeStream()
- Added checking of media device presence before using it on getUserMedia when a deviceId is set
- Added detection of media device update:
  - Added UserAgent#mediaDeviceChanged event
- Added management of connection error on register :
  - Cloud CCS connection error and retries
    - Added retries on cloud request
    - Added cloudFetchRetries, cloudFetchRetryDelay configuration parameters on registerInformation
  - CCS connection : authentication error
  - Events on Session
    - Added Session#disconnect
    - Added Session#error
- Added support for media update (renegotiation).
- Added UserAgent#createStreamFromMediaStream in order to create a Stream from a mediaStream

### Removed

- Removed Session#disconnectionWarning event
- Removed UserAgent#getDefaultDevices

# [4.0.2](https://cloud.apizee.com/apiRTC/v4.0/apiRTC-4.0.2.min.js) - 2018-04-06

### Fixed

- typo : Hangup reason 'User_Refuse_Call' replaced by 'User_Refused_Call'
- Added mimeType in blob return by stopRecord()

# [4.0.1](https://cloud.apizee.com/apiRTC/v4.0/apiRTC-4.0.1.min.js) - 2018-04-06

### Modified

- Optimization : Stream#startRecord() : change default recording mimeType to 'video/webm;codecs=vp8' instead of 'video/webm;codecs=vp9'

### Added

- Added posibility to configure mimeType on Stream#startRecord()
- Added Stream#pauseRecord
- Added Stream#resumeRecord
- Added checking of apiKey when getting apiCCId from cookie
- Support presenceGroup and subscribeToPresenceGroup modifications on disconnect / reconnect

### Fixed

- Fixed tryAudioCall after userMediaError

# [4.0.0](https://cloud.apizee.com/apiRTC/v4.0/apiRTC-4.0.0.min.js) - 2018-03-23

This version is the merge of ApiRTC and ApiRTC2 : Project name is apiRTC and version is v4.0.0 (former apiRTC version is 3.18.9)

Compatibility with apiRTC2 projects is maintained :

- ApiRTC2 keyword is preserved even if ApiRTC is preferred
- Only the library path change : https://cloud.apizee.com/apiRTC/vX.X

API of ApiRTC v3 is also maintained in order to keep compatibility with existing applications.

### Modified

- Major change with apiRTC2/ApiRTC merging

### Fixed

- apiRTCManager and Session event cleaning on disconnect()
- clean Conversation event cleaning on leave()

### Replaced

- Typo : persistantDataUpdated event by persistentDataUpdated

<hr/>

# [Changelog for older apiRTC version](https://dev.apirtc.com/apiRTC_V3/changeLog.html)
