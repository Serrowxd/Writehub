# Writehub

Github, but for writers!

My goal is to make a version control system for Writers of all types. Losing your work after hundreds of hours of commitment is painful, as a writer I've experienced this more than once. I want to make version control of writing more popular, and allow for the storage and retrieval of content in a controlled environment - losing all your work because of a failed harddrive will be a thing of the past.

## Potential Stack

**Front-End: React/Redux** -- I feel React would be a fantastic addition here because it is going to be used as a single-page application. Information that is displayed will be shown as relevant to the user logged in, so having a constant state and the ability to reuse purpose-built components would allow for clean and efficient access.

**Back-End: NodeJS/Firebase && Django** -- I'm slightly torn here. I would like to use NodeJS because it interacts well with Firebase by default - so I would be able to use Node as my middleman before passing the information directly to Firebase to store. With Django I have the ability to utilize Python and an SQL structure - some of the Django middleware would allow me to quickly and efficiently read and make a direct copy of the submitted file to our local database for future edits via the website, as well as a quick and efficient way of managing users and their files. This reason alone isn't enough to make me want to switch, so for right now it's going to be deployed via Node & Firebase, but a future version will likely include Django.

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
