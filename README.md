# gocryptfs

All credit for the file-system itself to rfjakob/gocryptfs.

## Releases

Image is available at:
```
docker.io/ojford/gocryptfs
```

In addition to `latest`, tags are available as both:
```
<gocryptfs_version>
<gocryptfs_version>-<docker_gcfs_release_number>
```

So that, for example, `gocryptfs` version `1.7.1` has:
```
1.7.1
1.7.1-1
```
and any update to the packaging in this repository will result in updating:
```
1.7.1
1.7.1-2
```
but leave `1.7.1-1` untouched. 

## Usage

Passphrase should be specified in:
```
$GOCRYPTFS_PSWD
```

CIPHERDIRs should be mounted under:
```
/crypts/
```

By default a flat structure is assumed, so that each first level directory should be a CIPHERDIR, instead, a list may be given at:
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
