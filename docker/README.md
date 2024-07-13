First copy the `.env.example` file to `.env` and update the values as needed.

```bash
cp .env.example .env
```

Then make a copy of adlists.list.txt to adlists.list

```bash
cp etc-pihole/adlists.list.txt etc-pihole/adlists.list
```

Run Docker compose using the following command:

```bash
make up
```

Import Adlists
