To generate the following files

1.
run `node ../minimal-demo.js`

2. 
get the result of `const proofData = await websnarkUtils.genWitnessAndProve(groth16, input, circuit, proving_key)`
the `publicSignals` field of `proofData` object is the data for `public.json`

3.
The `verification_key.json` downloaded by tornado-core is in different format of `snarkjs` asked for.
Therefore we need to rename `alfa` to `alpha`, which ensure snarkjs works well.
