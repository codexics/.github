# TL;DR

Codexics is an experimental theory for a growth system that stores data adaptively; By storing data entries as formulaic representations of their collectively pseudo-redundant components, controlled approximations of the original data can be reconstructed accordingly.

# Components

A codexical system has 3 essential components, known as the trio: the codex, the codec, and the coder; Each component has its core functions, a hieracherical configuration, and optional extensions.

### Codex

Core (executable) functions:
- Wrapping of at least two datasets:
  - The **codexicon** (the lexicon of codex): A dataset of fragments, which are equilibrized bases for approximated reconstructions
    - A **fragment** is an optimally picked pseudo-redundant segment of 
  - The **codexus** (the corpus of codex): A dataset of recipes and metadata, which are entries stored as representations of fragments
    - A **recipe** is an approximation formula for approximated reconstruction of the original entry using fragments.
    - The metadata includes the selective extraction of that from the original entry's, as well as house-keeping data including the corrective tensor
      - The **corrective tensor** is an encoded tendency metric that describes deviation from the original entry.
- Handling interface queries:
  - Probing and counting (basic questions about the data)
  - Restricted queries (as permitted by the configuration)
    - Codexus reads and writes (usually calling codec)
    - Codexicon reads and writes (usually calling coder)
  - Intermediary queries (if compatible codec / coder found)
    - Manual requests for reoptimization

Configuration definitions:
- The structure of the codexicon and the codexus
- The building of the data type being stored
- Any extensions and how to execute them

Multiplicities:
- Within one codex:
  - More than one codexicon for distinct sets of fragments justifying segregation
  - Never more than one codexus, just have more than one codex if needed
- Stacked codices:
  - If reoptimization is designed to be triggered by merging instead of correction
  - If more than one data types that cannot be stored together exists within entries

### Codec

Core (executable) functions:
- Encode entries to recipes and output metadata
  - Deconstructing input format into recipes of existing fragments
    - Fragmentation of input data entry
    - Estimated search for useable fragments
    - Determining the best recipe formula
  - Recording and calculating deviations accumulated from the original
    - Determining if new fragments not needed
    - If deviation exceeds thresholds, call coder
  - Extraction and safe storage of selected original metadata
- Decode entries from recipes with metadata
  - Reconstructing output format according to recipes of fragments

Configuration definitions:
- The method and syntax of
  - The approximation formulas
    - The compositions (placements, blending)
    - The transformations (distortions, filtering)
  - The corrective tensor
- The policy for appending to the codexus
- Any extensions and how to execute them

Multiplicities:
- Stacked codecs:
  - For more than one input or output formats
- Nested codecs (external recommended):
  - If the output format is commands for other codecs

### Coder

Core (executable) functions:
- Determining if new fragments are needed
- Equilibrizing and approving fragments
- Appending to the codexicon if needed 
- Auditing to decide if reapproximations are needed

Configuration definitions:
- The acceptable thresholds of corrective tensors
- The policy for appending to the codexicon
- The invocation of auditing and reoptimization
- Any extensions and how to execute them

# Applications

## Media Platform

A codexical media database is a storage system that behaves like a conventional database via the codec, but stores only representations of media entries in the codex, which grows in conjunction with the appropriate use of the coder.

### Examples
- Music Collection
  - The decompressed data type of each original entry is a 3×L matrix = <sample time (index), frequency (value), amplitude (value)> × entry length L (sampling rate).
  - Can be converted into a codexical database of linear data, with the codex containing equilibrized audio fragments used in formulas approximating reconstruction
- Photo Album
  - The decompressed data type of each original entry is a 5×L matrix = <x-coordinate (index), y-coordinate (index), red (value), green (value), blue (value)> × entry length L (pixel count)
  - Can be converted into a linear codexical database of linear data, with the codex containing equilibrized image fragments used in formulas approximating reconstruction
- Video Library
  - The decompressed data type of the audio stream of each original entry is a 3×L matrix = <sameple time (index), frequency (value), amplitude (value)> × entry length L (sampling rate), as described above.
  - The decompressed data type of the video stream of each original entry is a 6×L<sub>P</sub>×L tensor = <frame time (index), x-coordinate (index), y-coordinate (index), frequency (value), amplitude (value)> × pixel count L<sub>P</sub> × entry length L (frame count).
  - Can be converted into a dual-codexical database of linear data, with two codices containing equilibrized audio and video stream fragments used in formulas approximating reconstruction

## Record Archival

A codexical record system can be applied to retrieved data streams from observations or sensors (e.g. geological) that are meant for detecting trends or irregularities out of the ordinary. Lossless entries can also be logged upon triggers by elevated corrective attempts as an extensional implementation to capture critical data.

## Content Delivery

A codexical CDN is accessible across networks, with the codexicon served as a ledger (e.g. blockchain); The codec is bundled with the client for approximated deliveries; The coder is also decentralizable (e.g. via mining).

This is expected to suffer from the delayed nature of ledgers, and should only be used for time-insensitive deliveries before the landscape improves.
 
## Document Archive

A codexical collection of rasterized documents uses the methodology of a codexical photo database, but with varied magnifying transformations and complex processing (e.g. background removal) of semi-redundant elements (e.g. glyphs) as fragments. The codexus contain recipes as approximations of rendering the original documents by mimicking visual typesetting based on unstandardized fragments instead of fonts and logo files.

## Pattern Recognition

A codexical system capable of identifying patterns or objects can be achieved by programming the coder to recognize fragments of entries as relations, stored as approximation of graphs and nodes non-linearly. This would require multiple codecs to work in conjunction, in reading and writing to multiple codices.

## Artificial Intelligence

A codexical memory could theoretically replace conventional memory system of large language models, grounding the model's grasp with established truths, while retaining contextual nuance. The memory usage on actively semi-redundant inferences may be drastically reduced, if the coder (along with the router) is able to identify optimized commision of what should become part of the codexicon.

# Principles

## Full Agnostism and Compatibility

Each core and configuration of any of the trio can be of any state and format. As long as the configurations are parsible, their definitions are interpreted on how the cores are executed, version matching for interoperation is therefore optionally implemented.

## Lossiness and Controlled Approximations

Instead of storing in complete or original form, entries are represented in fragmental bases, which retains lossiness over reoptimizations. While anchor fragments and deviation constraints may offset degradation, fidelity is not preserved as a static guarantee, but as a bounded, actively governed property.

## Accumulation Good, Deletion Bad

The system is designed for one-way accumulation of entries over time. Performance and efficiency improve as data volume and fragment reuse increase, but degrade when large-scale withdrawal or deletion occurs. 

## Computational and Storage Tradeoff

Processing power is traded for storage efficiency and quality. Fragment equilibration and reoptimization introduce substantial computational overhead, often exceeding conventional compression by orders of magnitude.

# Milestones

## Formulation (We are Here)

Standardize the general rules of codexics before experimentation, in order to preserve full compatibility down the line.

## Proof of Concept

Apply condexics to an existing dataset and observe results to determine viability and direction.

## Monocodexical System

Create a single-codex system and compare results with a conventional one, e.g. music collection, photo album.

## Additional Features

### Losslessness

- Create lossless version of codexical system, by
  - Storing error-corrective residuals
  - Overachieving approximation accuracy
  - Round to original entries with 100% confidence
  - Ensure reoptimizations retain corrective thresholds

## Multicodexical System

Create a multiple-codex system and compare results with a conventional one, e.g. video library, rasterized documents.

## Polycodexical System

Create a multiple-trio (stacked) system and compare results with a conventional one, e.g. pattern recognition, artificial intelligence.

## Metacodexical System

Create a codex-within-codex (nested) polycodexical system, e.g. controlled artificial general intelligence.
