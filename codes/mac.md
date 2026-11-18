## clear the quarantine flag

Builds are unsigned (no Apple Developer ID). After dragging MarkText into Applications, clear the quarantine flag once:

```shell
xattr -d com.apple.quarantine /Applications/MarkText.app
```