There seems to be a regression for `deno upgrade` (and maybe other tools as well) when one is in a "broken" workspace setting.

I was working on example repository to showcase new workspace functionality. While doing so, I also wanted to try discovery of
test files in `__tests__` directory. Created `test_discovery` dir with its files. Then:

```
cd test_discovery
# while being on v1.44.4
deno upgrade
error: Could not find package.json for workspace member in 'file:///Users/ib/dev/broken_deno_upgrade/buzz/'.

```