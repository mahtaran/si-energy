# SI Energy

The Intermod System of Energy Units

Yet another one of these mods. But why should you choose for this one?
Well, this mod does some things I have not seen in any other mods yet:
- It makes converting energy types extremely easy to do, requiring only one block to convert any type to any type.
- It has two types of converters:
    - Converter block
    - Converter cable (adaptive & focussed)
- These converters will scan all connected energy-enabled blocks, and equally distribute and take energy to and from them, using the scaled values.
    - For example, if you connect it to two machines which can take an extremely large amount of energy (higher than the total energy going into the converter), each will get exactly 50% of the inputted energy, even if one uses a type of energy which is worth less than the other. See the [Example Input-Output Scenarios](#example-io) for more examples.

Additionally, it uses the double type for energy, allowing for a theoretical maximum energy flow of 179,769,313,486,231,570,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000.00 FE/tick. That is 17,976,931,348,623,157 followed by 292 zeroes. For reference: even if you strip away all the zeroes, it is still roughly 8000 times the number of galaxies in our universe.

## <a name="example-io"></a> Example Input-Output Scenarios (Will be improved later I swear)
### Scenario 1
#### Configuration values

1 FE = 0.25 EU = 2.5 J = 0.1 MJ
Maximum buffer size = -1 (Max)

#### Inputs (Maximum suppliable energy)

- Input 1: 20 FE
- Input 2: 10 EU (= 40 FE)

#### Outputs (Maximum takeable energy)

- Output 1: 75 J (= 30 FE)
- Output 2: 5 MJ (= 50 FE)

#### Results

Maximum input: 20 + 40 = 60
Maximum output: 30 + 50 = 80
Actual output: 30 + 30 = 60
Actual input: 20 + 40 = 60

### Scenario 2
#### Configuration values

1 FE = 0.25 EU = 2.5 J = 0.1 MJ
Maximum buffer size = -1 (Max)

#### Inputs (Maximum suppliable energy)

- Input 1: 55 FE
- Input 2: 20 EU (= 80 FE)

#### Outputs (Maximum takeable energy)

- Output 1: 25 J (= 10 FE)
- Output 2: 2 MJ (= 20 FE)

#### Results

Maximum input: 55 + 80 = 135
Maximum output: 10 + 20 = 30
Actual output: 10 + 20 = 30
Actual input: 15 + 15 = 30
