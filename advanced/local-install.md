---
description: Install Naas in your local environment.
cover: ../.gitbook/assets/Untitled Design.png
coverY: 0
---

# Local installation

## Is your local env ready?

Open a new notebook and check if the required env is set :

```python
import os
print('Yes' if (os.getenv('NB_USER') and os.getenv('JUPYTERHUB_USER') and os.getenv('JUPYTERHUB_API_TOKEN')) else 'No')
print(os.getenv('NB_USER'), os.getenv('JUPYTERHUB_USER'), os.getenv('JUPYTERHUB_API_TOKEN'))
```

#### Env requirements

* `NB_USER` => Should be set as your notebook user, probably `joyvan`
* `JUPYTERHUB_USER` => Should be set as your machine user, not root
* `JUPYTERHUB_API_TOKEN` => should be auto-set by your hub

## Install

Naas is a python module, install it with:

```python
!pip install naas
```

{% hint style="warning" %}
You can test on your local computer only the Scheduler feature.
{% endhint %}

{% hint style="danger" %}
Full install needs Kubernetes and Docker. Let's talk.
{% endhint %}

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

## Start

Start the server in your Jupyter singleuser machine:&#x20;

```bash
!python -m naas.runner &
```

{% hint style="info" %}
You can now delete previous cells
{% endhint %}

It will run until you stop your Jupyter server, go back to:

{% content-ref url="../" %}
[..](../)
{% endcontent-ref %}

