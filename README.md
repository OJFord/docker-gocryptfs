# gocryptfs

All credit for the file-system itself to rfjakob/gocryptfs.

## Usage

Image is available at:
```
docker.io/ojford/gocryptfs
```

Passphrase should be specified in:
```
$GOCRYPTFS_PSWD
```

List of mounted CIPHERDIRs should be given at:
```
/etc/gocryptfs/crypts
```

The decrypted file-systems will be mounted symmetrically at:
```
/mnt/
```

`fusermount -u` is *not* run automatically.


## Licence

MIT.
