# client
The @open-pwa/client is a unified API to talk to Open PWA Hosts via Javascript. That supports diffrent Transports

## Transports
- window.postMessage - (Used to talk to the Open PWA Platform when running inside a window that is opened by the Open PWA Platform)
- window.io - socket io 
- window.WebSocket
- window.fetch
- window.XMLHttpRequest
- <script src=""></script>
- window.PeerConnection

## Open PWA Client - API
 Will be enough in 99% of cases it will trigger the open-pwa protocol handler and request to open the current window
```
const openPwa = openPwaAuth(sdp)
const client = openPwa.get(window.location); // This will run 
// This code will not run outside of the Open PWA Application that is intended by design!
client.api.install(manifest)
```



