## [Analog to Digital Converter (ADC) - Computer Science](https://youtu.be/UNsZ1TzyMEk?si=rTAoz8YUntnGSWPz)

## [Link to Slides](https://data.audio.dev/talks/2023/practical-dsp-and-audio-programming/slides.pdf) link to slides
----------------------

- `signals` change wrt some other param ( time for eg. )

- computers cant process continuos signals .. hence we discrete them 
- done using `Analog to Digital converters`
- generating these samples artificially == `synthesizers`
- with signals we 
    - scale == amplify `(2Sin(x))`
    - change duration of sound `sin(9x) / sin (0.2x)`
    - shift time `cos(x + a)`
    - we can sum / multiply these signals to get a complex signal

- `DSP syst` == system that provides output signal wrt some input signal
    - for a `anolog signal ( continuous ) == analog synthesizer`
    - for a `discrete signal ( discrete ) == software synthesizer`

## important stuff : 

    - oscilltors produce these waves ( sinne waves which act as our signals )
    - input = audio signal + envelope
    - synthesizer processes it ( passes it to filter)
    - output gets processed with envelope

--------------

## Max Mathews brought the idea of this thoery to computers ( sound synthesizer )

- brought idea of unit genrators to programming lang
- some programming kanguages are :
`FAUST , C MAJOR , chuck`
   
--------------

## see how directed graphs are used to represente communicaation in audio engines / tensorflow
## see y imperatives programming isnt used 
## see differenc in directed graph n imperative design in programing  

------------

## learning Cmajor

- all cmajor examples are taken from here : [https://github.com/cmajor-lang/cmajor/tree/main/examples](https://github.com/cmajor-lang/cmajor/tree/main/examples)
- `2HelloWorld.cmajor`
- `3ElectricPiano.cmajor`

### every `.cmajor` file needs a `.cmajorpatch` file
### ctrl+shift+p -> makes a .cmajorpatch file automatically   

- use the cmajor extension in vscode to get familiar with it
- synatx is : 
`<direction> <type> <data type> <name> <optional size> <optional annotation>`

- direction can be : 
    - `input` 
    - `output`

- type can be : 
    - `stream`
    - `event`
    - `value`

- eg. : `input stream float in`

