# eduview2 sets and tools
In this folder you will find working, precompiled datasets for use with eduview. Keep in mind the compilation process for several datasets can take from 30 seconds to 20 minutes depending on your hardware. It is preferable to use the tools folder and compile your own versions, however.
We cannot assure that these will be up-to-date with all the parser changes.

### Directory
1. **tools** > parsers and fetchers for datasets
2. **graduates.json** > virgin, structured set, non-matched. only restructured
3. **graduates-matched.json** > matched graduates set by matcher2
3. **schools.json** > schools directory, precompiled w schools.py

### Importing to MongoDB

    mongoimport --jsonArray --db datasets --collection graduates --drop --file graduates_matched.json
    mongoimport --jsonArray --db datasets --collection schools --drop --file schools.json
