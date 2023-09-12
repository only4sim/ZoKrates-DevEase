## Add Pedersen Commitment library

Here we provide the library and how to use this library. Pedersen_Test is used to prove and validate the results of a Pedersen commitment based on EVM. Then we will show how to build and excute this project.

A simple experimental approach could be to directly upload the Pedersen_Commitment.zok and Pedersen_Test.zok file to the Remix online IDE, install the ZoKrates plugin, and sequentially perform the compilation, computation, setup, proof generation, and export of the verifier for the Pedersen_Test.

During the compuation, according to the prompt, you can provide the input value and the random number r. This two values should be submitted in the unsigned integer form.

The following is an example. You can check if the ZoKrates returns the same Pedersen Commitment as here:
```
input: 2023
r: 100007

Pedersen Commitment:
[
  "20850275905078636534173652351693189784865178257748520923164502745863728411148",
  "11221839714337003948710340586708936710216024907408808149770870142730170826822"
]
```