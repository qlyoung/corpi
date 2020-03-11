# corpi

fuzzing corpuses

## About

This is a monorepo that tracks all of my fuzzing corpi for any targets I fuzz.

## Repo Layout

The general structure is

```
.
├── target-1
│   ├── subtarget-1
│   │   ├── gen
│   │   └── seed
│   └── subtarget-2
│       ├── gen
│       └── seed
└── target-2
    ├── subtarget-1
    │   ├── gen
    │   └── seed
    └── subtarget-2
        ├── gen
        └── seed

```

where:

- `target-x` is the name of the target program
- `subtarget-n` is the specific subsystem in the target being fuzzed
- `seed` is the initial input corpus first used to fuzz that subtarget
- `gen` is the generated corpus, or whatever I put in there last

