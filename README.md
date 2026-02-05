# TL;DR

Codexics is an experimental theory for storing signal-derived data at scale; By writing raw data as compositional representations of its collectively redundant components, controlled approximations of the original data can be reconstructed accordingly.

# Components

A codexical system has 3 essential components, known as the trio: the codex, the codec, and the coder, each with an executable core, a hieracherical configuration, and optional extensions (e.g. losslessness on demand).

### Codex

The codex is the storage of a codexical system.
It is typically a directory containing at least one pair of two datasets: the codexicon and the codexus.

Its core contains:
- The codexicon (the lexicon of codex) is a dataset of fragments, which are optimally selected or created building blocks for approximated reconstruction.
- The codexus (the corpus of codex) is a dataset of recipes, which are entries stored as representations of fragments, which are approximation formulas and respective corrective tensors.
-- An approximation formula is an encoded instruction to reconstruct the original entry using fragments.
-- A corrective tensor is an encoded tendency metric that describes deviation from the original entry.

Its configuration defines:
- The building of the data type being stored
- The structure of the codexicon and the codexus
- The syntax of approximation
- Any extensions and how to execute them

### Codec

The codec is the interface of a codexical system. 

Here it stands for commit + decode, as it is unable to encode and append to the codexicon.

Its core functions are:
- (Re)representing entries as recipes
-- (Re)approximating entries as formulas
-- (Re)computing corrective tensors 
- Appending to the codexus when allowed
- Query handling and execution

Its configuration should define:
- Queries and responses
- Conversion instructions
- The method and syntax of
-- The approximation formulas
--- The compositions (placements, blending)
--- The transformations (distortions, filtering)
-- The corrective tensor
- The policy for appending to the codexus
- Any extensions and how to execute them

### Coder

The coder is the controller of a codexical system.

Despite traditionally being part of a codec, a codexical coder does as much heavy lifting as the rest of the codec, and is therefore separated.

Its core functions are:
- Determining if new fragments are needed
- Computing optimized new fragments
- Appending to the codexicon if needed 
- Auditing to decide if reapproximations are needed

Its configuration defines:
- The acceptable thresholds of corrective tensors
- The policy for appending to the codexicon
- The invocation of auditing and reapproximation
- Any extensions and how to execute them

# Applications

## Media Platform

A codexical media database is a storage system that behaves like a conventional database via the codec, but stores only approximations of media entries in the codex, and scales with the appropriate use of the coder.

Examples include:
- Audio Library, where the primitive data type is a 2-by-N matrix, with the 2 values being frequency and time, N being the duration of time by its units.
- Photo Library, where the primitive data type is a 5-by-N matrix, with the 5 values being the 2-dimensional coordinates along with the RGB colour values of the pixel, N being the size of the photo by its pixel count.
- Video Library, where the primitive data type is a 7-by-N matrix, aligning and conjoining the primitive data types of an audio entry and a video entry.

## Record Archival

A codexical record system is best applied to retrieved data streams from observations or sensors (e.g. geological) that are meant for detecting trends or irregularities out of the ordinary. Lossless entries can also be logged upon triggers by elevated corrective attempts as an extensional implementation to capture critical data.

## Content Delivery

A codexical CDN is univerally accessible, with the codexicon served as a ledger (e.g. blockchain); The codec is bundled with the client for approximated deliveries; The coder is also decentralizable (e.g. via mining).

 This is expected to suffer from the delayed nature of ledgers, and should only be used for time-insensitive deliveries before the landscape improves.
 
## Rasterized Documentation

A codexical collection of rasterized documents uses the methodology of a codexical photo database, but with varied magnifying transformations and complex processing (e.g. background removal) of semi-redundant elements (e.g. glyphs) as fragments. The codexus contain recipes as approximations of rendering the original documents by mimicking visual typesetting based on unstandardized fragments instead of fonts and logo files.

## Artificial Intelligence

A codexical memory could theoretically replace conventional memory system of large language models, grounding the model's grasp with established truths, while retaining contextual nuance. The memory usage on actively semi-redundant inferences may be drastically reduced, if the coder (along with the router) is able to identify optimized commision of what should become part of the codexicon.

# Principles

## Full Agnostism and Compatibility

Each core and configuration of any of the trio can be of any state and format. As long as the configurations are parsible, their definitions are interpreted on how the cores are executed, version matching for interoperation is therefore optionally implemented.

## No entries are stored in full

Entries may become increasingly lossy over optimizations, despite offsetting anchors.

## Scaling is only optimized upwards

Performance and efficiency drop significantly with large withdrawals of entries.

## Processing power is traded off

Optimizations and computational overhead is expected to surpass compression by orders of magnitudes.
