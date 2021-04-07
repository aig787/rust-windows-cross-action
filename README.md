Rust Windows Builder Action
========================

GitHub action for building windows targeted rust binaries (x86_64-pc-windows-gnu). 

```yaml
- uses: aig787/rust-windows-cross-builder@v1.0
  with:
    args: build --release --all-features
    credentials: ${{ secrets.GIT_CREDENTIALS }}
```
### Inputs
| Variable | Description | Required | Default |
|----------|-------------|----------|---------|
| args     | Arguments passed to cargo | true | `build --release` | 
| credentials | If provided git will be configured to use these credentials and https | false | |
