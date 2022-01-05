This project is in alpha state.  
It intends to replace https://github.com/hoehermann/purple-gowhatsapp/.

## Configuration

Environment Variables:

These are read when the plug-in loads (before a connection is established):

* `PURPLE_GOWHATSAPP_DATABASE_DIALECT`  
  default: `sqlite`  

* `PURPLE_GOWHATSAPP_DATABASE_ADDRESS`  
  default: `file:purple_user_dir/whatsmeow/store.db?_foreign_keys=on`  
  Folder must exist, `store.db` is created automatically.
  The file-system must support file locking and be responsive, else the database driver will not work.

## Windows specific

CMake will try to set-up a development environment automatically. 
The project can be opened using Microsoft Visual Studio 2022.

Additional dependencies:

* [go (32 bit)](https://go.dev/dl/go1.17.5.windows-386.msi)
* [gcc (32 bit)](https://osdn.net/projects/mingw/)

go and gcc must be in %PATH%.
