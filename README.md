# Writehub

Github, but for writers!

## Notes

`less-watch-compiler styles styles`

Probably going to use styled-components mainly, then fine adjustments to things like spans and the like with LESS.

Look into storing .txt files on their own, rather that attempting to translate - possibly .doc files incase they use MSWord? Only issue is storage, I'd like to minimize the storage requirements because it's pure text, but what about storing the text in a way that doesn't modify the styling - if applicable?

The absolute basics - I want it to be a storage container for .txt files, where you can push and pull content. There needs to be an easy way of pushing and pulling this content, though, so maybe a downloadable GUI? Maybe it grabs updates based on file changes, similar to Google Drive? Definitely the ideal route, but there is a lot of work that goes into that - possibly a stretch?

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
