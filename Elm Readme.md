
#Installation
Elm makes it really simple to install their software and provides everything a 
user made need within the installation bundle. First, the user chooses a link 
that corresponds with OS they have. Then they click it and Elm is installed.
Once installed, Elm provides several different tools for users:

>elm-repl — play with Elm expressions
>elm-reactor — get a project going quickly
>elm-make — compile Elm code directly
>elm-package — download packages

Elm also has different plugins within the text editors like prettifiers and syntax highlighting. 

Elm can also be easily injected into React by using these lines of code right under the rest of the
imported elements

import Elm from 'react-elm-components'
import { Todo } from '../dist/elm/todomvc.js'
 
function render() {
    return <Elm src={Todo} />
}

##Dependencies  
To install dependencies, users would have to enter: 
elm-package install /name of dependency/
For example if a user wanted to use NoRedInk/elm-decode-pipeline
They would write: elm-package install NoRedInk/elm-decode-pipeline

 To update dependecies, users would first have to run: 
 elm-package diff elm-lang/core 3.0.0 4.0.0
to see the differences between the version they have and the version they'd like to update to
just in case the updated version has things that might break their current apps. 3.0.0 is the code the user has
and 4.0.0 is the updated version.
Then, to update, the user would use change the version state in their package.json,
then run elm-package install elm-lang/core 4.0.0 which is the most current and updated version.

#React and Elm.
Elm is most similar to react in terms of what it is used for. They both create websites and web apps

![Timon&Pumbaa](Timon&Pumbaa.jpeg)


