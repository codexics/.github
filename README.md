# TL;DR
Codexics is an experimental theory for storing signal-derived data at scale; By writing raw data as compositional representations of its collectively redundant fragments, controlled approximations of the original data can be reconstructed accordingly.

# Utilizations

## Media Database

A codexical database is a storage system that behaves like a database at the interface level, but stores reconstructive recipes of fragments from a shared dictionary of them instead of raw data, while operating with controlled loss, evolution, and optimization.

A database will take form as a folder containing the following files:

### .codex

.codex is a specifications file that defines the nature of data being stored, primarily on its linearity and storage format.

### .codex.py or any executable types

.codex.py is an executable that (re)generates the storage by appending optimized fragments.

### .codec

.codec is a specification file that defines the convertion between the format of raw data and recipes of fragments.

### .codec.py or any executable types

.codec.py is an executable that take queries, performs conversion and appends recipes to the storage.

### .db or any storage types

.db is the actual storage of data as recipes of fragments, and will contain two datasets:

#### fragments.csv or any dataset types

fragments.csv is a dataset file containing all fragments referenced in recipes for reconstruction.

#### recipes.csv or any dataset types

recipes.csv is a dataset file containing all entries of data encoded as aggregations of transformed fragments.

# Design Principles

## No entries are stored in full

Entries may become increasingly lossy over optimizations, despite offsetting anchors.

## Scaling is only optimized upwards

Performance and efficiency drop significantly with large withdrawals of entries.

## Processing power is traded off

Optimizations and computational overhead is expected to surpass compression by orders of magnitudes.
