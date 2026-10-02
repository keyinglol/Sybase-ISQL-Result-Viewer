# Sybase isql Result Viewer

An offline, single-file HTML tool that turns fixed-width Sybase `isql` query output into a readable table.

## Use

1. Download or clone this project.
2. Open `sybase-result-viewer.html` in a modern web browser.
3. Paste the `isql` output, including the dashed column separator. The `(N row(s) affected)` footer is optional.
4. Select **Format table**. Select **Clear** to reset the page.

No installation, server, or database connection is required.

## What it supports

- Sybase `isql` output with a dashed separator beneath the column headers.
- Multiple result rows, provided each row fits on one output line.
- Query prompt lines such as `1>` and `2> go`.
- Spaces inside values, including descriptions and dates.

Wrapped or malformed rows are reported instead of being shown as a potentially incorrect table. If a row is wrapped, try widening the terminal and rerunning the query.

## Privacy

Formatting happens locally in the browser. The page does not send pasted queries or results to a server.

## Limitations

This initial version is designed for ordinary, unwrapped `isql` output. Other output formats may not parse correctly.
