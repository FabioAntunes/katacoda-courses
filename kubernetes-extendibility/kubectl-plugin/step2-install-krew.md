There are a [few ways to install Krew](https://krew.sigs.k8s.io/docs/user-guide/setup/install/) based on your environment, but for this Katacoda scenario we will choose the recommended commands for Bash.

Install Krew as a plugin for kubectl.

```
pushd "$(mktemp -d)" &&
curl -fsSLO "https://github.com/kubernetes-sigs/krew/releases/latest/download/krew.{tar.gz,yaml}" &&
tar zxvf krew.tar.gz &&
KREW=./krew-"$(uname | tr '[:upper:]' '[:lower:]')_amd64" &&
"$KREW" install --manifest=krew.yaml --archive=krew.tar.gz &&
"$KREW" update &&
popd
```{{execute}}

This will take a moment to complete. If you did this on a local machine you might want to add this to you system path.

`export PATH="${KREW_ROOT:-$HOME/.krew}/bin:$PATH"`{{execute}}

Krew is now available so verify its version.

`kubectl krew version`{{execute}}

First and foremost, Krew is a collector of close to 84 plugins.

`kubectl krew search | wc -l`{{execute}}

Explore the plugin list look at the list.

`kubectl krew search`{{execute}}

There are **so many helpful plugins** in this list and it hard to single out just one, but lets explore a few.



