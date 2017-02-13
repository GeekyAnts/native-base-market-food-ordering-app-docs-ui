# GitStrap CLI Tools

* Globally install GitStrap CLI
```
npm install -g gitstrap-cli
```

* Clone and Setup Upstream and Origin
  ```
  gitstrap init <gitstrap-repo> <my-repo> <folder-name>
  ```
  The above line of command functions as listed below:
  * ``` my-repo ``` should be an existing repository.
  * Clones [Swiggy App](http://market.nativebase.io/view/react-native-swiggy-app-theme) (upstream) on user local system with same git-branch as that of upstream, say ``` master ```.
  * Sets the upstream ([Swiggy App](http://market.nativebase.io/view/react-native-swiggy-app-theme)) and origin (my-repo) on user local system respectively.
  * Push to user remote repo.
  * ``` folder-name ``` is optional argument of gitstrap init command.
    * Without _folder-name_ : Clones the theme into your current location of directory.
    * With _folder-name_ : Clones the theme into the specified location of your directory.

* Sync Update from GitStrap Repo
  ```
  gitstrap sync <upstream-branch>
  ```
  The above line of command functions as listed below:
  * Pulls from upstream i.e., ```master``` (from default git-branch)
  * Merges into user local repo i.e., ```master``` (same git-branch as that during clone)
  * This command by default pulls and merge the same branch of upstream repo with that of user local repo.
  * ```upstream-branch``` is optional argument of _gitstrap sync_ command.
  This lets you choose between your git-branch for sync.
  _Example:_
  * If you want to sync [Swiggy App](http://market.nativebase.io/view/react-native-swiggy-app-theme)'s ```master``` with your repo's ```development```, include ```upstream-branch``` with gitstrap sync command.
  * ```git checkout development```

  ```gitstrap sync master```
