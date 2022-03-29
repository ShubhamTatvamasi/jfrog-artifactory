# GPG Key

Install gpg package for macOS:
```bash
brew install gpg
```

Generate key:
```bash
gpg --full-generate-key
```

Parameter | Values
---|---
key type | RSA and RSA
keysize | 4096
valid till | 0
Real name | artifactory.shubhamtatvamasi.com
Email address |
Comment |

List all keys:
```bash
gpg --list-secret-keys
```

Export public and private key
```bash
gpg --output public.artifactory.shubhamtatvamasi.com.pgp --armor --export artifactory.shubhamtatvamasi.com
gpg --output private.artifactory.shubhamtatvamasi.com.pgp --armor --export-secret-key artifactory.shubhamtatvamasi.com
```

Delete key:
```bash
gpg --delete-secret-keys artifactory.shubhamtatvamasi.com
```


