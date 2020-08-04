# hl-server

Fast asynchronous server for buffers tokenizing.
Nowadays it support tokenizing `c` and `cpp` buffers (based on `clang`).
As example here realized `polyndrom` tokenizing for buffers

__supported version protocols__: v1, v1.1

See [test hl client](test/simple_hl_client)

See [vim-hl-client](https://github.com/andrejlevkovitch/vim-hl-client)

## Bugs

For some reason you can get `ASTReadError` with using flags:

```
-isystem
/some/third/party/library
```

Just change it to:

```
-I/some/third/pary/library
```
