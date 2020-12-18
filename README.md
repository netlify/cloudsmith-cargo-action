# cloudsmith-cargo-action

This sets up the credentials necessary to let `cargo` pull crates from
a private Cloudsmith repository.

### Usage

The only required input, `token`, is the *secret* for an entitlement token
with read access to the repo you're using.

```
    - uses: netlify/cloudsmith-cargo-action@v1
      with:
        token: ${{ secrets.CLOUDSMITH_TOKEN }}
```