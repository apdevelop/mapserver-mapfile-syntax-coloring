# MapServer Mapfile keywords colorization for Visual Studio 2017 text editor
Syntax colorization for [MapServer](https://github.com/mapserver) [Mapfile](https://mapserver.org/mapfile/index.html) keywords. 
Implemented as `TextMate Grammar` file (JSON format) which is supported in Visual studio 2017 text editor.

### How it looks

![Coloring sample](https://github.com/apdevelop/mapserver-mapfile-syntax-coloring/blob/master/mapfile-sample.png)

### Installing

The base directory for custom TextMate Grammar files in Visual Studio 2017 is `%USERPROFILE%\.vs\Extensions\`.
In the most cases that path resolves to: `C:\Users\<yourusername>\.vs\Extensions\`
In this directory create directory named `MapServer`, then create `Syntaxes` inside it. Place `MapServer.json` file into that directory.

The final path will be: `C:\Users\<yourusername>\.vs\Extensions\MapServer\Syntaxes\MapServer.json`

Run Visual Studio, open MapServer text file (with `.map` extension), now it should display with syntax highlighting.

### Known issues
* Currently provides very basic set of MapServer Mapfile keywords and rules
* Visual studio crashes when cursor hovering collapsed blocks (similar to [](https://developercommunity.visualstudio.com/content/problem/550000/vs-2019-crashes-when-editing-json-file-missingmani.html) issue)