1. Create a config

Place a JSON configuration with cloud credentials in cfg.json in the root of
this repo.

2. Start viam-server

Run the following command and leave it running in the background.

```bash
mise r run-server
```

2. Perform some operations

Load app and create some resources, interact with them from the control tab,
etc.

3. Start Jaeger

This assumes you already have Docker installed and running on your system. Run
the following command and leave it running in the background.

```bash
mise r run-jaeger
```

4. Import traces from viam-server to docker

```bash
mise r import-traces
```

5. View traces in Jaeger

Navigate to [localhost:16686](http://localhost:16686/).
