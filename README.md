### To use, add this to your ~/.bashrc -

```bash
pyproj() {
    [[ -d .git ]] && echo "Existing git repo detected, aborting." && return 1
    git clone git@github.com:Luke4211/pyproj.git . && rm -rf .git && git init && sh init_env.sh && source /venv/bin/activate
}
```
