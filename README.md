# GA-HMM-Interface
Web-based interface for preprocessing for the GA-HMM peak calling algorithm

Overall
=======
- Visual interface for user to select pre-processing options for GA-HMM peak calling
- Generates log file with options that can be fed to GA-HMM peak caller
- Can load previous log file for modification
- Provides visual examples and guides
- Does NOT host data files, expects user to make genome browser session with data
- GA-HMM should require no user input except the logfile and full chr wig.

- Display default 7 state HMM model
- Display example peaks
- Display simple region selection example (run, test, model)
- Link to documentation

Selecting regions
=================
- User enters url to a genome browser session, have it appear in an iframe. Do not load until user hits "load" to reduce overhead (slow).
- Have user select regions, get coordinates from the page and store. 
- Allow user to load previously selected coordinates and cancel or confirm them. 
- Take screenshot of coordinates and display to user in a "previously selected peak" box. 
- Allow user to designate coordinates as "run" "test" or "model" region, and if model region designate as one of 7 peak states.

Other Possibilities
===================
- visual HMM constructor for non-7state HMM models
