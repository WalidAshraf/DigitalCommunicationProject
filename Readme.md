# Digital Communication Project
Simulate the performance of different modulation schemes,[BPSK](#a), [QPSK](#b), [FSK](#c), [QAM16](#d),[QAM64](#e) in an AWGN environment 


# Raised Cosine Filter
 [BPSK with Raised Cosine](#f), [QPSK with Raised Cosine](#g), [QAM16 with Raised Cosine](#h), [QAM64 with Raised Cosine](#j)
 # To reproduce the result:
 1. Open matlab
 2. Choose simulink from the toolbar 
 3. Open the desired model 
 4. Write bertool in the command window and set Eb/N0 -10:1:10 in theoritcal and monte carlo 
 5. Press browse and choose the model.slx
 6. Ber variable Name = ber
 7. Press plot in theoritcal and run in monte carlo

# General Parameters:

## Random Integer Generator
    - Samples per frames =  100
    - Initial Seed = 37 
    - Sample Time = 1
 ## AWGN channel
    - Initial Seed = 67
    - Eb/No = EbNo
# <a id="a"></a>Binary Phase Shift Keying (BPSK)
## Definition: 
BPSK is a two phase modulation scheme, where the 0’s and 1’s in a binary message are represented by two different phase states in the carrier signal: θ = 0 degree for binary 1 and θ = 180 degree for binary 0

## Paramters:
    - Random Integer Generator size =  2
    - Phase offset = 0 
## Schematic:
![Schematic](Graphs/BPSKSchematic.png)
## Before Noise Scatter plot:
![BeforeNoise](Graphs/BPSKF1.png)
## After Noise Scatter plot:
![AfterNoise](Graphs/BPSKF2.png)
## Ber Graph
![BerGraph](Graphs/BPSKF3.png)


# <a id="b"></a> QPSK
## Definition: 
QPSK is a form of Phase Shift Keying in which two bits are modulated at once, selecting one of four possible carrier phase shifts (0, 90, 180, or 270 degrees)
## Paramters:
    - Random Integer Generator size =  4
    - Phase offset = pi/2
## Schematic:
![Schematic](Graphs/QPSKSchematic.png)
## Before Noise Scatter plot:
![BeforeNoiseQPSK](Graphs/QPSKF1.png)
## After Noise Scatter plot:
![AfterNoiseQPSK](Graphs/QPSKF2.png)
## Ber Graph
![BerGraphQPSK](Graphs/QPSKF3.png)



## <a id="c"></a>QAM16
### Definition: 
QAM is a technique used to transmit two digital bit streams or two analog signals by modulating or changing the amplitudes of two carrier waves so that they differ in phase by 90 degrees, a quarter of a cycle, hence the name quadrature. One signal is called the "I" signal and the other is the "Q" signal.
## Paramters:
    - Random Integer Generator size =  16
    - M-ary number = 16
    - Normalization method = Average Power
## Schematic:
![QAM16Schematic](Graphs/QAM16Schematic.png)
## Before Noise Scatter plot:
![BeforeNoiseQPSK](Graphs/QAM16F1.png)
## After Noise Scatter plot:
![AfterNoiseQPSK](Graphs/QAM16F2.png)
## Ber Graph
![BerGraphQPSK](Graphs/QAM16F3.png)


## <a id="d"></a>QAM64
## Paramters:
    - Random Integer Generator size =  64
    - M-ary number = 64
    - Normalization method = Average Power
## Schematic:
![QAM16Schematic](Graphs/QAM64Schematic.png)
## Before Noise Scatter plot:
![BeforeNoiseQPSK](Graphs/QAM64F1.png)
## After Noise Scatter plot:
![AfterNoiseQPSK](Graphs/QAM64F2.png)
## Ber Graph
![BerGraphQPSK](Graphs/QAM64F3.png)

## <a id="e"></a> FSK
### Definition: 
FSK is a frequency modulation scheme in which digital information is transmitted through discrete frequency changes of a carrier signal.
## Paramters:
    - Random Integer Generator size =  8

## Schematic:
![FSKSchematic](Graphs/FSKSchematic.png)
## Before Noise Scatter plot:
![BeforeNoiseFSK](Graphs/FSKF1.png)
## After Noise Scatter plot:
![AfterNoiseFSK](Graphs/FSKF2.png)
## Ber Graph
![BerGraphFSK](Graphs/FSKF3.png)


# Raised Cosine Filter

## Parameters:
    - Rolloff factor = 0.2
    - Recieve delay = 2 

## <a id="f"></a> BPSK
## Schematic:
![BPSKRSchematic](Graphs/BPSKRSchema.png)
## Before Noise Scatter plot:
![BeforeNoiseBPSKR](Graphs/BPSKRF2.png)
## After Noise Scatter plot:
![AfterNoiseBPSKR](Graphs/BPSKRF1.png)
## Ber Graph
![BerGraphBPSKR](Graphs/BPSKRF3.png)


## <a id="g"></a> QPSK
## Schematic:
![QPSKRSchematic](Graphs/QPSKRSchema.png)
## Before Noise Scatter plot:
![BeforeNoiseQPSKR](Graphs/QPSKRF1.png)
## After Noise Scatter plot:
![AfterNoiseQPSKR](Graphs/QPSKRF2.png)
## Ber Graph
![BerGraphQPSKR](Graphs/QPSKRF3.png)


## <a id="h"></a>QAM16
## Schematic:
![QAM16RSchematic](Graphs/QAM16R.png)
## Before Noise Scatter plot:
![BeforeNoiseQAM16R](Graphs/QAM16RF1.png)
## After Noise Scatter plot:
![AfterNoiseQAM16R](Graphs/QAM16RF2.png)
## Ber Graph
![BerGraphQAM16R](Graphs/QAM16RF3.png)

## <a id="j"></a>QAM64
## Schematic:
![QAM64RSchematic](Graphs/QAM64RSchema.png)
## Before Noise Scatter plot:
![BeforeNoiseQAM64R](Graphs/QAM64RF1.png)
## After Noise Scatter plot:
![AfterNoiseQAM64R](Graphs/QAM64RF2.png)
## Ber Graph
![BerGraphQAM64R](Graphs/QAM64RF3.png)