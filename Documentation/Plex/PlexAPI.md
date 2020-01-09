# Plex API

The API of Plex between the clients and servers.

## Objects

### Connection

#### Attributes

| Name | Type | Description | Example |
| --- | --- | --- | --- |
| uri | string | URI of the connection | |

### Device

#### Attributes

| Name | Type | Description | Example |
| --- | --- | --- | --- |
| clientIdentifier | string | Client identifier of the device | |
| createdAt | int | Device created at timestamp | |
| device | string | ? | |
| id | int | ID of the device | |
| lastSeenAt | int | Device last seen at timestamp | |
| model | string | ? | |
| name | string | Name of the device | |
| platform | string | Platform of the device | |
| platformVersion | string | Platform version of the device | |
| product | string | Product type of the device | |
| productVersion | string | Product version of the device | |
| provides | string | ? | |
| publicAddress | ? | Public address of the device | |
| screenDensity | ? | Screen density of the device | |
| screenResolution | ? | Screen resolution of the device | |
| token | string | Token of the device | |
| vendor | ? | Public address of the device | |
| version | string | Version of the device | |

### MediaContainer

#### Attributes

| Name | Type | Description | Example |
| --- | --- | --- | --- |
| allowCameraUpload | boolean | Allow Camera Upload | |
| allowChannelAccess | boolean | Allow Channel Access | |
| allowSharing | boolean | Allow Sharing | |
| allowSync | boolean | Allow Synchronisation | |
| allowTuners | boolean | Allow Tuners | |
| backgroundProcessing | ? | | |
| certificate | ? | | |
| companionProxy | ? | | |
| countryCode | ? | | |
| diagnostics | ? | | |
| eventStream | ? | | |
| friendlyName | string | A friendly name for the server | My Plex Server |
| livetv | ? | | |
| machineIdentifier | string | Unique identifier for the server | |
| myPlex | boolean | | |
| myPlexMappingState | enum? | | mapped |
| myPlexSigninState | enum? | | ok |
| myPlexSubscription | boolean | | |
| myPlexUsername | ? | | |
| ownerFeatures | ? | | |
| photoAutoTag | ? | | |
| platform | string | Name of the platform | Linux |
| platformVersion | string | Version of the platform | 16.04.6 LTS (Xenial Xerus) |
| pluginHost | ? | | |
| publicAddress | ? | |
| pushNotifications | ? | | |
| readOnlyLibraries | ? | | |
| size | ? | | |
| streamingBrainABRVersion | ? | | |
| streamingBrainVersion | ? | | |
| sync | ? | | |
| transcoderActiveVideoSessions | ? | | |
| transcoderAudio | ? | | |
| transcoderLyrics | ? | | |
| transcoderSubtitles | ? | | |
| transcoderVideo | ? | | |
| transcoderVideoBitrates | ? | | |
| transcoderVideoQualities | ? | | |
| transcoderVideoResolutions | ? | | |
| updatedAt | ? | | |
| updater | ? | | |
| version | string | Version of the server | 1.18.3.2156-349e9837e |
| voiceSearch | ? | | |

### MediaProvider

#### Attributes

| Name | Type | Description | Example |
| --- | --- | --- | --- |
| baseURL | string | Base URL of this Media Provider | |
| identifier | string | ? | com.plexapp.plugins.library |
| protocols | string | ? | stream |
| title | string | ? | Bibliotheek |
| token | string | Token to use on this Media Provider | |
| types | string | ? | video,audio,photo |

### Server

#### Attributes

| Name | Type | Description | Example |
| --- | --- | --- | --- |
| address | ? | ? | |
| allLibraries | ? | ? | |
| host | ? | ? | |
| id | ? | ? | |
| machineIdentifier | ? | ? | |
| name | ? | ? | |
| numLibraries | ? | ? | |
| owned | ? | ? | |
| pending | ? | ? | |
| port | ? | ? | |
| product | ? | ? | |
| protocol | ? | ? | |
| protocolCapabilities | ? | ? | |
| protocolVersion | ? | ? | |
| serverId | ? | ? | |
| version | ? | ? | |

### SyncList

#### Attributes

| Name | Type | Description | Example |
| --- | --- | --- | --- |
| itemsCompleteCount | ? | ? | |
| totalSize | ? | ? | |
| version | ? | ? | |

## Routes

### GET `/api/home`

?

### GET `/api/home/users`

Get `User`s in your home.

### POST `/api/home/users`

Invite `User` to your home.

#### URL Parameters

| Name | Description | Required | Example |
| --- | --- | --- | --- |
| invitedEmail | ? | Yes | |

### GET `/api/invites/requested`

Get requested `Invite`s for your home.

### GET `/api/invites/requests`

Get requests to join another one's home.

### GET `/api/users`

Get `User`s and their shared `Server`s.

### GET `/api/v2/authentications/providers`

Get authentication providers (Google, Facebook, LastFM)

### GET `/api/v2/shared_servers/{id}`

?

### POST `/api/v2/user/settings`

Change settings for Plex Web.

### GET `/api/v2/user/{hash}/settings/opt_outs`

?

### GET `/clients`

?

### GET `/devices[.xml|.json]`

Get `Device`s.

### GET `/devices/{id}[.xml|.json]`

Get `Device` by id.

### DELETE `/devices/{id}[.xml|.json]`

Delete `Device` by id.

### GET `/media/providers[.xml|.json]`

Get `MediaProvider`s of the server.

### GET `/pms` (only https://plex.tv)

?

### GET `/pms/system` (only https://plex.tv)

?

### GET `/pms/system/library` (only https://plex.tv)

?

### GET `/pms/system/library/sections` (only https://plex.tv)

?

### /accounts

### /accounts/{id}

### /myplex/account

### /myplex/refreshReachability

### /updater/status

### /player/proxy/poll

### /sync/transcodeQueue

### /playQueues

### /status/sessions/background

### /playlists

### /playQueues/1

### /playlists/1/items

### /system/agents

### /system/agents/com.plexapp.agents.none/config/1

### /system/agents/contributors

### /system/agents/attribution

### /library/sections

### /activities

### /channels/all

### /system/agents

### /system/scanners/1

### /services/browse

### /services/browse/{base64}

### /library/sections/prefs

### /:/plugins/com.plexapp.agents.imdb/prefs

### POST /library/sections

#### URL Parameters

| Name | Description | Required | Example |
| --- | --- | --- | --- |
| name | Name of the Library Section | ? | |
| type | ? | ? | movie |
| agent | Agent of the Library Section | ? | com.plexapp.agents.imdb |
| scanner | Scanner of the Library Section | ? | Plex Movie Scanner |
| language | Language | Language | en |
| importFromiTunes | ? | ? | |
| enableAutoPhotoTags | ? | ? | |
| location | Location to scan media in | ? | |
