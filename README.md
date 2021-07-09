This is an extension for Drive Badger. It provides a sample `bitlocker.keys` file, containing a list of Bitlocker recovery keys.

Drive Badger is able to automatically detect and decrypt Bitlocker-encrypted partitions, but only using recovery keys.
It doesn't support PIN, password, FVEK files, TPM interactions etc., as this would be hard or impossible to automate.

### Installing

Do NOT clone this repository directly. Instead, **fork it** (possibly multiple times), or create similar repositories from stratch
(empty repository with just `bitlocker.keys` file is enough).

Next, clone each of them as `/opt/drivebadger/config/keys-bitlocker-yourchosenname` local directory on your Drive Badger persistent partition.

This way, you are able to update all cloned repositories in the future by a single command `/opt/drivebadger/update.sh`.

### More information

- [Drive Badger main repository](https://github.com/drivebadger/drivebadger)
- [Drive Badger wiki](https://github.com/drivebadger/drivebadger/wiki)
- [description, how configuration repositories work](https://github.com/drivebadger/drivebadger/wiki/Configuration-repositories)
