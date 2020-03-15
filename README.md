## How this code works

1. The index.js behaves as a node file, importing the required modules to call the model (IE: faceMesh)
2. Browserify has been run on the index.js file, which bundles together all the required pieces from the require statements
   into a standalone, vanilla javascipt file which can run in the browserDownloads
3. The HTML page feeds the video camera feed into the javascript functions, which in turn call the model


## Open Questions
1. Why is the model making network calls here? It should be loaded into the browser and make inferences from there. In the
[demo](https://storage.googleapis.com/tfjs-models/demos/facemesh/index.html), no network calls are being made and latency is very low
