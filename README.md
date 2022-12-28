# Omegle Location finder
 
This code defines a new implementation of the RTCPeerConnection class, which is used in web real-time communication (WebRTC) applications. It overrides the addIceCandidate method, which is called when a new ICE candidate is received by the peer connection.

The modified addIceCandidate method first logs the received ICE candidate to the console, then checks if the candidate is of the srflx (server reflexive) type. If it is, the code calls the getLocation function with the IP address of the ICE candidate as an argument.

The getLocation function uses the ipgeolocation.io API to retrieve geolocation information for the given IP address. It does this by making a GET request to the API's ipgeo endpoint, passing in the IP address and an API key as query parameters. The API key should be replaced with a valid key obtained from the ipgeolocation.io website.

The getLocation function then logs the retrieved location information to the console in the following format:




# Note
Please replace "your-api-key-here" with an API key from https://ipgeolocation.io/.
