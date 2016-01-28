hls-analyzer
============

HLS debug player simulates a viewer and check basic settings of the streaming server.

1. Downloads the master playlist
2. Downloads the bitrate playlists
3. Download all .ts segments for every bitrate
4. Performs DNS check on the host of the HLS URL
5. Perrorms traceroute on each IP returned by the DNS check
6. Uses ffprobe to analyze each HLS segment
7. Uses mediainfo to dump metadata about the ts segments
8. Measures TTFB for HLS segments
9. Archives all segments on disk
10. Continous mode with VLC to test buffering, stops
11. Is the stream compatible with the HLS specification
12. MPEG-TS discontinuity check on segments
