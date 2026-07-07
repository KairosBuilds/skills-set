# Execution Rules

## Download Quality
1. Default: best quality available (mp4)
2. Options: 4k, 1080p, 720p, 480p, 360p
3. Audio: best audio quality for extraction
4. Respect platform rate limits and terms of service

## Format Handling
1. **Video**: mp4, mkv, webm, avi
2. **Audio**: mp3, m4a, flac, wav, opus
3. Use ffmpeg for format conversion
4. Preserve metadata when possible

## Playlist Handling
1. Default: first video only
2. Playlist mode: sequential download with index prefix
3. Respect playlist size limits
4. Handle private/deleted videos gracefully

## Error Handling
1. Network timeout → retry with backoff
2. Video unavailable → report and skip
3. Format not available → fallback to next best
4. Corrupted download → restart from checkpoint
