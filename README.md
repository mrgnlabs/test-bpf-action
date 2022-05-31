# Test BPF action
Github action for running Solana Rust tests

### Example
```yaml
test:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - name: Cargo Test BPF
        uses: mrgnlabs/test-bpf-action@v0.3
        with:
          args: '--features=test'
          thread_stack_size: '4096000' # 4Mb
```
