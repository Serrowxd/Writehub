# Writehub

Github, but for writers!

## Notes

`less-watch-compiler styles styles`

Probably going to use styled-components mainly, then fine adjustments to things like spans and the like with LESS.

Look into storing .txt files on their own, rather that attempting to translate - possibly .doc files incase they use MSWord? Only issue is storage, I'd like to minimize the storage requirements because it's pure text, but what about storing the text in a way that doesn't modify the styling - if applicable?

The absolute basics - I want it to be a storage container for .txt files, where you can push and pull content. There needs to be an easy way of pushing and pulling this content, though, so maybe a downloadable GUI? Maybe it grabs updates based on file changes, similar to Google Drive? Definitely the ideal route, but there is a lot of work that goes into that - possibly a stretch?

**Ideas**

- Full-Screen Text Editor (in-browser).
- Real-time saving of edits with back-ups and version control when editing in the website.
- Daily Updates for modifications done or files uploaded to the server (github graph kinda).
- `if (version !== upload) { makeBackup() } else { window.alert("No changes detected") }`
- As above, automatic checking onChange or onClick with the "Sync" button that checks for local changes.

For the storage of files, I think I'm going to use Python to read and then store the raw text from any file submitted, which will be used to populate sections.

Possibly look into directly storing the files themselves, then giving read/write access to the editor? I'd like to avoid having the files stricly managed by website, rather I'd like it to be a way of storing writing and having proper version control incase you lose some of your work by accident.

## **TODO**

#### Client

- Landing
- Login / Logout
- Profile
- Storage of Writing, maybe the ability to read and store .txt files?

#### Server

- CRUD
- Reading and storing .txt files that are pulled in from the client.
- Storing text without modifying it.
- Title, Description, Storage by Chapter.
- **Possibly do it in Python?**
