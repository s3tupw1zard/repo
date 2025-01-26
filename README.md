# apt

This is my own apt repository which I use for my own use.

I add things I cant find as deb file in official repositories or somewhere else.

## Installation of this repo:

### Ubuntu

#### Ubuntu 24.04 Noble Numbat

Create `/etc/apt/keyrings` if not existing:

```bash
sudo mkdir -p /etc/apt/keyrings
```

Download gpg key file into `/etc/apt/keyrings`:

```bash
sudo wget -O /etc/apt/keyrings/s3tupw1zard-apt-noble.asc https://s3tupw1zard.github.io/repo/public-key.asc
```

Add the noble repository to apt:

```
echo "deb [signed-by=/etc/apt/keyrings/s3tupw1zard-apt-noble.asc] https://s3tupw1zard.github.io/repo/ noble main" | sudo tee /etc/apt/sources.list.d/s3tupw1zard-apt-noble.list
```

### Debian

#### Debian 12 Bookworm

Create `/etc/apt/keyrings` if not existing:

```bash
sudo mkdir -p /etc/apt/keyrings
```

Download gpg key file into `/etc/apt/keyrings`:

```bash
sudo wget -O /etc/apt/keyrings/s3tupw1zard-apt-bookworm.asc https://s3tupw1zard.github.io/repo/public-key.asc
```

Add the noble repository to apt:

```
echo "deb [signed-by=/etc/apt/keyrings/s3tupw1zard-apt-bookworm.asc] https://s3tupw1zard.github.io/repo/ bookworm main" | sudo tee /etc/apt/sources.list.d/s3tupw1zard-apt-bookworm.list
```
