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
- Multiple result rows, including rows and headers wrapped across matching fixed-width output lines.
- Query prompt lines such as `1>` and `2> go`.
- Spaces inside values, including descriptions and dates.

Malformed or incomplete rows are reported instead of being shown as a potentially incorrect table. Wrapped output is supported when each row follows the same line layout as the dashed separator.

## Privacy

Formatting happens locally in the browser. The page does not send pasted queries or results to a server.

## Limitations

The viewer is designed for fixed-width `isql` output. Other output formats may not parse correctly.
