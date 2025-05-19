# FedRAMP-20x KSI Materials

The presentation by @sunstonesecure-robert was not recorded.  The slides and supplemental materials are added here.

## Summary of Discussion

From recall - others can add/edit appropriately - the main themes of the discussion that ocurred were:

- Using a catalog and/or profile is the easiest path, and an example of such a catalog was submitted to this repo for review by attendees.
- Using Component Definition control groups as security capabilities was not widely understood/accepted.  The main problem seemed to be
  that many thought that the KSIs should WERE controls, although some understood the SunStone position that metrics should reflect the
  *effectiveness* of controls (as @sunstonesecure-robert remarked based on experience volunteering on the CSA Metrics project).  AWS participants
  noted that this would give buyers the ability to rank sort CSPs based on their KSI metrics (if sortable, eg integer/decimal/categorical vs. simmply boolean)
  and choose the CSPs based on that performance ranking.
- Using the prototype mapping model was appealing to some, in light of IBM's presentation about their implementation and use of it in the COMPASS/trestle projects.
  This seems attractive if other vendors/projects support it - but currently only IBM does :( Also, as with the rest, some catalog or dummy controls are needed
  so this isn't really so much an alternative as an additional layer to a solution. NOTE: FedRAMP 20x discussions from FedRAMP staff seem to suggest they are
  not particularly interested in KSI defintions that *solely* derive their results as a mapping to/from only static controls.  (Again this seems to reinforce the opinion
  that metrics are NOT controls.)
- The final idea about using Assessment Plan and Assessment Results to "MEASURE" KSIs was moderately well understood - but as noted in the slides everyone
  highlighted that some form of catalog or dummy controls is needed anyway, and/or the mapping to the other underlying controls.
  Thus, if used with the corresponding Component Definition security capabilities definition, and/or the mapping,
  this becomes a very useful abstraction.

In summary, everyone seems to be more or less interested in getting more guidance from FedRAMP PMO first.  OSCAL Foundation wants to hear from them more.
The main technical approaches reduce to effectiveley be:

1. Start with a catalog of "dummy" KSI controls
2. Then do one or more of the following
  - use the mappings model to map NIST 800-53, SOC2 or others to the KSIs
  - use the component definition groupings to define security "capabilities" and use these in the SSP, optionally mapping the "provided" controls using the mappings
  - add a novel "MEASURE" control-objective (eg add to NIST 800-53A types: INTERVIEW, TEST, EXAMINE) and report that on the Result for the dummy or mapped controls.
