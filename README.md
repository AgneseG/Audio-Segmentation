<div class="container-fluid main-container">

<div id="header" class="fluid-row">

</div>

Relevant code & data have been stored with the following structure:
=================================================================================================

<div id="mp3-download-folder" class="section level3">

### **mp3 download folder** 

<div id="code-to-retrieve-files-from-remote-websites"
class="section level6">

###### Code to retrieve files from remote websites

-   *Radio commercial download.ipynb*
-   *30sec Music Download.ipynb*
-   *Dutch Speech Downloads.ipynb*
-   *Podcast download.ipynb*
-   *Artists2.txt* → list of artists from the Million Song Dataset

</div>

</div>

<div id="data-folder" class="section level3">

### **Data folder** 

<div
id="contains-all-mp3-files-the-chunked-streams-used-in-the-predictions"
class="section level6">

###### Contains all *mp3* files + the chunked streams used in the predictions

-   Commercials
-   Music
-   Speech
-   Streams
    -   Stream 1 chunks → *.npy* files (each one corresponds to a chunk)
    -   Stream 1 chunks - 3 sec → *.npy* files
    -   Stream 2 chunks → *.npy* files
    -   Stream 2 chunks - 3 sec → *.npy* files

</div>

</div>

<div id="chunks-2sec-folder" class="section level3">

###  **Chunks 2sec folder** 

-   ######  **Chunking process** 

    -   *Chunking process - Commercial.ipynb*
    -   *Chunking process - Music.ipynb*
    -   *Chunking process - Speech.ipynb*

-   ######  **Train-Test split** 

    -   *Train-Test split.ipynb* → code used to split test-train
        datasets for each category
    -   Train → contains all *.npy* train files (each one corresponds to
        a chunk)
    -   Test → contains all *.npy* test files
    -   Speech over Music - Train → contains all *.npy* train files for
        the category Speech over Music
    -   Speech over Music - Test → contains all *.npy* test files for
        the category Speech over Music
    -   *Train\_chunks.npy* → array with train files’ names
    -   *Train\_labels.npy* → array with the corresponding labels
    -   *Test\_chunks.npy* → array with test files’ names
    -   *Test\_labels.npy* → array with the corresponding labels

        *Note*: the last four .npy files were created to get suitable
        inputs to feed the Keras generator afterwards

-   ######  **NN model** 

    -    **Speech - Music - Commercial** 
        -   **Model building**
            -   *Sequential NN.ipynb* → NN with dense layers only
            -   *CNN 2D.ipynb* → Convolution 2D NN
            -   *CNN\_2D.h5* → final Keras model
        -   **Predictions**
            -   *Stream 1 chunking process.ipynb*
            -   *Stream 1 predictions.ipynb*
            -   *Stream 2 chunking process.ipynb*
            -   *Stream 2 predictions.ipynb*
            -   *Stream 1 predictions.pdf* → plot with Stream 1
                predictions based on 3-categories model (true labels are
                attached on top of plot)
            -   *Stream 2 predictions.pdf*

</div>

<div id="chunks-3sec-folder" class="section level3">

###  **Chunks 3sec folder** 

    Same structure as 'Chunks 2sec' with a further sub-division of the folder 'NN model' in
    'Speech - Music - Commercial' and 'Speech - Music - Commercial - Speech over Music':

-   ######  **Chunking process** 

    -   *Chunking process - Commercial.ipynb*
    -   *Chunking process - Music.ipynb*
    -   *Chunking process - Speech.ipynb*
    -   *Speech over music.ipynb* → code to create speech over music
        chunks

-   ######  **Train-Test split** 

    -   *Train-Test split.ipynb* → code used to split test-train
        datasets for each category
    -   Train → contains all *.npy* train files (each one corresponds to
        a chunk)
    -   Test → contains all *.npy* test files (each one corresponds to a
        chunk)
    -   Speech over Music - Train → contains all *.npy* train files for
        the category Speech over Music
    -   Speech over Music - Test → contains all *.npy* test files for
        the category Speech over Music
    -   *Train\_chunks.npy* → array with train files’ names
    -   *Train\_labels.npy* → array with the corresponding labels
    -   *Test\_chunks.npy* → array with test files’ names
    -   *Test\_labels.npy* → array with the corresponding labels
    -   *Train\_chunks\_4categories.npy* → same as above but for the 4
        categories
    -   *Train\_labels\_4categories.npy*
    -   *Test\_chunks\_4categories.npy*
    -   *Test\_labels\_4categories.npy*

        *Note*: the last eight .npy files were created to get suitable
        inputs to feed the Keras generator afterwards

-   ######  **NN model** 

    -    **Speech - Music - Commercial** 
        -   **Model building**
            -   *CNN 2D.ipynb* → Convolution 2D NN
            -   *CNN\_2D\_3sec.h5* → final Keras model
        -   **Predictions**
            -   *Stream 1 chunking process + predictions.ipynb*
            -   *Stream 2 chunking process + predictions.ipynb*
            -   *Stream1\_3sec.pdf* → plot with Stream 1 predictions
                based on 3-categories model (true labels are attached on
                top of plot)
    -    **Speech - Music - Commercial - Speech over Music**
        Same structure as ‘Speech - Music - Commercial’.

<div
id="each-notebook-containes-further-explanations-of-the-steps-done."
class="section level5">

##### Each notebook containes further explanations of the steps done.

</div>

</div>

</div>

