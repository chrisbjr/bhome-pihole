First copy the `.env.example` file to `.env` and update the values as needed.

```bash
cp .env.example .env
```

Change the contents of the .env file to match your environment.

Copy the pre-configured `pihole/adlists.list` file and `pihole/whitelist.txt` to the etc-pihole directory.

```bash
cp pihole/adlists.list etc-pihole/adlists.list && cp pihole/whitelist.txt etc-pihole/whitelist.txt
```

Run Docker compose using the following command:

```bash
make up
```
