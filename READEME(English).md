# Desktop Notes

I got fed up with wading through ads just to find a Windows sticky notes app that worked the way I wanted. So I built one myself, with a little help from AI.

Desktop Notes lets you keep multiple sticky notes on your Windows desktop. It supports live Markdown formatting, reminders, automatic launch at sign-in, and sync across Windows PCs through a shared cloud folder.

[简体中文](README.md)

## Download and install

1. Download `DesktopNotesSetup-V1.0.0.exe` from this repository's **Releases** page.
2. Run the installer and choose the default location or a folder of your own.
3. Open Desktop Notes from the installer, the desktop shortcut, or the Start menu.

To upgrade, right-click the system tray icon, select **Exit (退出)**, and install to the same folder. Your notes are stored in `%LocalAppData%\DesktopNotes\notes.xml`.

## Work with notes

- Click **New Note (新建便签)** to add a note. Drag the top bar to move it or drag an edge to resize it.
- The top-right controls pin the note on top, minimize it, or hide it. To delete the note, click **Delete (删除)** in the toolbar.
- Double-click the desktop shortcut to bring back notes with text or reminders. To see blank notes as well, choose **Show All Notes (显示所有便签)** from the tray menu.
- Click the zoom percentage or hold `Ctrl` and scroll over the text to zoom from 75% to 250%. Each note remembers its own zoom level.
- Use **Format (格式)** to change the background or text color and format selected text. Edits are saved automatically.

## Markdown and keyboard shortcuts

Type `**bold**`, `*italic*`, `==highlight==`, or wrap inline code in backticks. Formatting appears as soon as you type the closing marker. At the start of a line, type `#`, `-`, or `>` followed by a space to create a heading, bullet, or quote. Live conversion applies as you type. Use the Format menu to style pasted text.

| Shortcut | Action |
| --- | --- |
| `Ctrl+B` | Bold |
| `Ctrl+I` | Italic |
| `Ctrl+U` | Underline |
| `Ctrl+Shift+H` | Highlight |
| `Ctrl+Shift+C` | Inline code |
| `Ctrl++` / `Ctrl+-` / `Ctrl+0` | Zoom in / zoom out / reset to 100% |

## Reminders

Each note can have multiple one-time reminders.

- **Add a reminder.** Click **Reminders (提醒)**, enter a date, time, and description, then click **Add (添加)** and **Save (保存)**.
- **Create a reminder from text.** Select a phrase such as `明天下午三点半开会` (meeting tomorrow at 3:30 PM), then click **Reminder Suggestions (提醒建议)**. Review the suggested time and description before adding it. Time recognition is designed for Chinese date and time expressions.
- **Edit or delete a reminder.** Select it in the reminder list. Change the time or description and click **Edit Reminder (修改提醒)**, or click **Delete Reminder (删除提醒)**. Either action saves the change and closes the dialog.

Reminders use your PC's local time zone. When a reminder is due, Windows shows a tray notification if notifications are enabled. Click it to open the corresponding note. If the app was closed when the reminder was due, it processes the reminder the next time it starts.

## Launch at sign-in

Open **Settings (设置)** and enable **Launch at Sign-in (开机自启动)**. The most recently used note with text or reminders opens when you sign in to Windows. Enable **Start Minimized (自启动时最小化)** if you prefer to keep it out of the way.

## Sync across PCs

Install Desktop Notes and your cloud storage client on each PC. Go to **Settings (设置) → Note Sync (便签同步) → Choose Sync Folder (选择同步文件夹)** and select the same dedicated cloud folder on each device.

Note text, formatting, and reminders sync across PCs. Window position, size, zoom, and sign-in settings are stored separately on each device. The sync menu shows the current folder and sync status and lets you sync immediately or turn sync off. If the app detects changes to the same note on both devices, it keeps a separate copy for review.

