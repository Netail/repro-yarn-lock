# Turbo Repro Yarn Lock

1. Make sure you have Yarn v1 installed
2. Check yarn.lock -> `string-width-cjs@npm:string-width` & `string-width` should be separate entries
3. Run `yarn turbo prune @org/web`
4. Check the yarn.lock in the `out` dir of the pruned output (`string-width-cjs@npm:string-width` & `string-width` are merged)
