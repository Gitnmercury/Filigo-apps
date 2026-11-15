# Privacy of Filigo

**In short: your documents never leave your computer.** No account, no cloud, no telemetry, no advertising, no
automatic update.

## What the software sends over the Internet

Nothing. At startup, the software cuts all network access inside its own program: even by mistake, it could not send
anything. Its source code is visible so that anyone can check this.

Two actions open another program, only when you click: the contact address (your email program) and, where relevant, a
web page (your browser).

## Updates: only if you ask

The software never checks by itself whether a newer version exists. If you choose Help > Check for updates and answer
"Yes" to the message shown, it connects to GitHub (api.github.com), and to nothing else, to read the number of the
latest published version. It sends the name and version of the software, like any request to a website; GitHub sees
your IP address. No document, name, recipient or history is sent. The connection is open for the time of this check,
then closed again.

## Word, OpenDocument and text files

For these files, the software asks Microsoft Word or LibreOffice, if installed on your computer, to convert them to
PDF. This conversion happens on your computer. Word and LibreOffice are separate programs with their own settings:
depending on these, they may for instance load an image linked in a document from the Internet. PDFs and photos use
neither Word nor LibreOffice.

## What is stored on your computer

| File | Content | How to delete it |
|---|---|---|
| `.filigo.json` (home folder) | appearance settings: color, opacity, size, theme | delete the file |
| `.filigo_historique.json` (home folder) | history: date, recipient, purpose and location of the copies | "Clear history" button in the pane, or delete the file |

The watermark text is never saved in the settings. The history is readable only by you: `0600` permissions on Linux, access restricted to your Windows account on Windows. The temporary files
of a conversion are deleted as soon as it is finished.

## Watermarked copies

The watermark is part of the image: it cannot be removed like a layer. The hidden information of the original file
(GPS position of a photo, device, author, title) is removed. The copy carries neither the publisher's name nor the
software's. Its suggested name is that of the original followed by `_filigrane`: you can change it when saving.

A watermark makes fraudulent reuse of a copy harder and more visible; it cannot prevent it in every case. Keep your
originals.

## Contact us (Help › Contact us)

Filigo sends nothing by itself: the message is prepared in your mail program and you send it yourself. You can attach a short
technical summary with no personal data: the Filigo version and, in ranges, your system (Windows 10, 11, Linux, Mac), memory, number
of cores, screen width, language, theme and Word converter. It is written as a short code (for example `FG1-S2R4C3E3L1T2W1-V1.4.0`) and
the window shows what it means before sending. A bug report can go without it; feedback cannot be sent without it, so that we can
interpret it. What you type is passed to the publisher to handle your message, and for that only. If you type your address, it is also
attached, **encrypted**, on the same line as the technical code: only the author can read it with their private key, and the window tells
you before sending. Filigo never reads an address from anywhere else than this field (neither your Windows account nor your mail program).

## Contact

Anthony BELKACEM EI, 200 rue de la Croix Nivert, 75015 Paris, France. Questions: apps@ohtna.fr
