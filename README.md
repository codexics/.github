# TL;DR

Codexics is an experimental theory for a growth system that stores data adaptively; By writing raw data as compositional representations of its collectively redundant components, controlled approximations of the original data can be reconstructed accordingly.

# Components

A codexical system has 3 essential components, known as the trio: the codex, the codec, and the coder; Each component has its core functions, a hieracherical configuration, and optional extensions.

### Codex

*The codex is the storage of a codexical system.*

More than one codex may be needed:
- For identified sets of internally semi-redundant entries justifying segregation
- If reoptimization is designed to be triggered by merging instead of correction
- If more than one data types have misaligned indices or orders

Its core contains:
- The **codexicon** (the lexicon of codex): A dataset of **fragments**, which are equilibrized bases for approximated reconstructions.
- The **codexus** (the corpus of codex): A dataset of **recipes**, which are entries stored as representations of fragments.
  - An **approximation formula** is an encoded instruction to reconstruct the original entry using fragments.
  - A **corrective tensor** is an encoded tendency metric that describes deviation from the original entry.

Its configuration defines:
- The structure of the codexicon and the codexus
- The building of the data type being stored
- Any extensions and how to execute them

### Codec

*The codec is the interface of a codexical system.*

Here it stands for commit + decode, as it is unable to encode and append to the codexicon.

More than one codec:
- For more than one input or output formats

Its core functions are:
- (Re)representing entries as recipes
  - (Re)approximating entries as formulas
  - (Re)computing corrective tensors 
- Appending to the codexus when allowed
- Query handling and execution
- Bidirectional conversion
  - Representating entries by approximation
    - Decoding and decompressing from input format
  - Reconstructing from approximation formulas
    - Encoding and compressing into output format
    - Aligning multi-codex entries if necessary

Its configuration should define:
- Queries and responses
- Conversion instructions
- The method and syntax of
  - The approximation formulas
    - The compositions (placements, blending)
    - The transformations (distortions, filtering)
  - The corrective tensor
- The policy for appending to the codexus
- Any extensions and how to execute them

### Coder

*The coder is the controller of a codexical system.*

Despite traditionally being part of a codec, a codexical coder does as much heavy lifting as the rest of the codec, and is therefore separated.

Its core functions are:
- Determining if new fragments are needed
- Equilibrizing and approving fragments
- Appending to the codexicon if needed 
- Auditing to decide if reapproximations are needed

Its configuration defines:
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
