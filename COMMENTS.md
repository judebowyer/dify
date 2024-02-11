## Self-hosted Installation

The [docs online](https://docs.dify.ai/getting-started/install-self-hosted/local-source-code) need some more detail to get this working. Principally, here are some missng steps:

- Edit `.env` if there are port clashes with services already running (and if you run some standard services, e.g. Jenkins, then there will be clashes)
- Set up postgres details that needed for the build script
```
sudo -i -u postgres
psql
\password postgres # create password for the default account
\q
createdb dify
```
