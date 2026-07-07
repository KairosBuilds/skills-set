# Examples

## Example 1: Single Video Download
```
Input: "Download YouTube video in 1080p"
URL: https://youtube.com/watch?v=abc123
Actions:
1. Parse video ID: abc123
2. Get available formats (1080p available)
3. Download: video.mp4 (1080p, 125MB)
4. Verify file integrity
5. Save to ./downloads/
```

## Example 2: Audio Extraction
```
Input: "Extract audio from video as MP3"
URL: https://youtube.com/watch?v=xyz789
Actions:
1. Download best audio stream
2. Convert to MP3 (320kbps)
3. Add metadata (title, artist)
4. Save: audio/xyz789.mp3
```

## Example 3: Playlist Download
```
Input: "Download tutorial playlist"
URL: https://youtube.com/playlist?list=PLabc
Actions:
1. Parse playlist (12 videos)
2. Download each video in 720p
3. Name format: 01-title.mp4, 02-title.mp4...
4. Report progress: 5/12 complete
```
