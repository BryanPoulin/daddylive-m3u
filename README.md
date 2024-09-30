# DaddyLive Live TV & Sports Playlists

Add DaddyLive TV & Sports streams to your IPTV application using the M3U playlists provided in this repository. There are four different playlist formats available, each tailored for specific applications or media players.

## Playlist Formats:

- **playlist.m3u8:**
  A standard M3U playlist. If you're using this playlist, make sure your IPTV application allows the setting of a custom `Referer` and `User-Agent` header. The headers must be set in order to access the streams. Failure to set these required headers will result in a 403 error when attempting to stream.
  
  **Playlist:** `http://example.com`  
  **EPG URL:** `http://example.com`  
  **Referer:** `https://lewblivehdplay.ru`
  **User-Agent:** `Mozilla/5.0 (iPhone; CPU iPhone OS 17_6_0 like Mac OS X) AppleWebKit/605.2.10 (KHTML, like Gecko) Version/17.6.0 Mobile/16F152 Safari/605.2`     

- **tivimate_playlist.m3u8:**
  This playlist is specifically formatted for use with TiviMate. To use it, simply load the URL provided in this repository into Tivimate as an "M3U Playlist." No additional setup is needed as Tivimate handles the required headers for playback.
  
   **Playlist:** `http://example.com`  
   **EPG URL:** `http://example.com`  
   **Referer:** `Included` 
   **User-Agent:** `Included` 

- **kodi_playlist.m3u8:**
	This playlist is designed for Kodi, utilizing `#KODIPROP` properties to handle the necessary stream settings, including the required headers. It is optimized for Kodi's PVR IPTV Simple Client, ensuring compatibility with your Kodi setup. This format is primarily designed for Kodi, but it may or may not be compatible with other applications.
	
   **Playlist:** `http://example.com`  
   **EPG URL:** `http://example.com`  
   **Referer:** `Included` 
   **User-Agent:** `Included` 

- **vlc_playlist.m3u8:**
  Optimized for VLC Media Player. This playlist uses VLC-specific formatting to ensure streams play correctly, including setting the necessary headers via `#EXTVLCOPT`. This format is primarily designed for VLC, but it may or may not be compatible with other applications.
  
   **Playlist:** `http://example.com`  
   **EPG URL:** `http://example.com`  
   **Referer:** `Included` 
   **User-Agent:** `Included` 

If none of these playlists work with your IPTV application, you can try using the m3u8-playlist-proxy (coming soon). This proxy acts as a middle layer to help resolve potential issues with playing the playlists, especially if your IPTV app doesn't support setting the required headers.

## Usage Instructions:

1. Choose the playlist format that suits your application or media player.
2. Add the playlist URL to your IPTV application.
3. Ensure that your application supports the required settings, such as setting the `Referer` header for streams to play.

## Playlist and EPG Syncing:

The playlist and EPG data are updated every 4 hours. Since streaming data can change frequently, it’s recommended to sync the refresh of both your playlist and guide information simultaneously in your IPTV application. If you notice 'No information' being displayed in the guide, try manually refreshing the EPG within your application to ensure the most up-to-date data is loaded.

## Sports:

Basketball, Football, American Football, Hockey, Baseball, Motor Sports, Fight (UFC, Boxing), Tennis, Rugby, Golf, Billiards, AFL, Darts, Cricket, Other

## Disclaimer:

This repository has no control over the streams, links, or the legality of the content provided by dlhd.so (including all mirror sites). It is the end user's responsibility to ensure the legal use of these streams, and we strongly recommend verifying that the content complies with the laws and regulations of your country before use.

