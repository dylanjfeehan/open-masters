# Paged File
## Intro
`PagedFile` interface will enable clients to perform file i/o in terms of pages.  
### page operations:
- scan pages
- read a page
- add paged
- delete page
- obtain and release scratch page 

### paged file operations
- create paged file
- destroy paged file
- open paged file
- close paged file

### Components of the Paged Files
- BufferManager
- Error tables (mapping of code to message)
- FileHandle 
- HashTable
- PagedFileManager (handle open, close, create, delete)
- PageHandle
- Statistics

### Global Declarations
- internal.h
- redbase.h
- pf.h (classes)

### Interfaces
- Manager
  - BufferManager
  - internal
- FileHandle
  - BufferManager
  - internal
- PageHandle 
  - internal

### Utils
#### BufferManager
used by: 
- PagedFileManager
- FileHandle
uses: 
- statistics
- hashtable
- internal
