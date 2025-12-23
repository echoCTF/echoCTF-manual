# echoCTF Manual

Repository for the development of the echoCTF Manual.

## Local devel

```bash
sudo apt install mkdocs-material
pip install mkdocs-glightbox --break-system-packages
pip install pymdown-extensions --break-system-packages
pip install mkdocs-pymdownx-material-extras  --break-system-packages
pip install mkdocs-snippets --break-system-packages
pip install mkdocs-exclude --break-system-packages
```

Once you have all the needed packages installed

```bash
mkdocs serve -f .mkdocs.yml
```

The website can be then accessed by visiting <http://127.0.0.1:8000/>

You can change the details by passing additional arguments to serve.

```
-a, --dev-addr <IP:PORT>      IP address and port to serve documentation locally (default: localhost:8000)
--dirty                       Only re-build files that have changed.
-s, --strict / --no-strict    Enable strict mode. This will cause MkDocs to abort the build on any warnings.
```

## Linting

The linting is done with the VScode extension `markdownlint`. Rule overrides are configured in the local `.markdownlint.yml`.
