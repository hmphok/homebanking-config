# homebanking-config

Runs the `homebanking` job container using Docker Compose.

Image: `ghcr.io/hmphok/homebanking`

## First-time setup (on the host)

```sh
# clone this repo
git clone <THIS_REPO_URL> homebanking-config
cd homebanking-config

# create local env file
cp .env.example .env
nano .env

# create folders (keys/ and data/)
docker compose run --rm init
